
### 一、EPJ File

#### 1.E142MapDataUploadFormat （EC）

- 上传 `Map` 数据使用的格式 【0:二进制】【1:ASCII】

```C#
switch (_E142MapDataUploadFormat)
{
	case eE142ItemPartFormat.ASCII:
		{
			mapDataDVName = new string[] { "E142MapData", "E142SubstrateType", "E142SubstrateID" };
			dataValues = new Cimetrix.Value.CxValue[] {
				new AValue(mapdata),
				new AValue(substrateType),
				new AValue(substrateID)
			};
		}
		break;
	case eE142ItemPartFormat.BINARY:
	default:
		{
			mapDataDVName = new string[] { "E142MapData", "E142SubstrateType", "E142SubstrateID" };
			dataValues = new Cimetrix.Value.CxValue[] {
				new BiValue(UTF8Encoding.UTF8.GetBytes(mapdata)),
				new AValue(substrateType),
				new AValue(substrateID)
			};
		}
		break; 
}
```

#### 2.E142MapDataDownloadFormat （EC）

- 允许下载的 `Map` 数据格式 【0:二进制】【1:ASCII】【2:二进制或 ASCII】

```C#
switch (vtype)
{
	case VALUELib.ValueType.Bi | VALUELib.ValueType.valueARRAY:
		if (_E142MapDataDownloadFormat == eE142ItemPartFormat.ASCII)
		{
			string errorMessage = "S14F2 message format is wrong. Second item in level 4 (the map data) is a binary array but E142MapDataDownloadFormat is configured for ASCII. "; 
			OnMapDataErrorHandler(OBJID, errorMessage);
			Log.WriteIfEnabled(LogCategory.Error, Source, errorMessage);
			return;
		}
		message.ArrayAt(listhandle4, 2, out var arrayHandle);
		message.ItemCount(arrayHandle, out var mapsize);
		message.ArrayValuesAtBinary(arrayHandle, 0, mapsize, out var oMapData);
		sMapData = UTF8Encoding.UTF8.GetString((byte[])oMapData); 
		break;

	case VALUELib.ValueType.A:
		if (_E142MapDataDownloadFormat == eE142ItemPartFormat.ASCII)
		{
			string errorMessage = "S14F2 message format is wrong. Second item in level 4 (the map data) is ASCII but E142MapDataDownloadFormat is configured for BINARY. ";
			OnMapDataErrorHandler(OBJID, errorMessage);
			Log.WriteIfEnabled(LogCategory.Error, Source, errorMessage);
			return;
		}
		message.GetValueAscii(listhandle4, 2, out sMapData); 
		break;

	default:
		{
			string errorMessage = "S14F2 message format is wrong. Second item in level 4 (the map data) is not a binary array or ASCII string. ";
			OnMapDataErrorHandler(OBJID, errorMessage );
			Log.WriteIfEnabled(LogCategory.Error, Source, errorMessage);
			return;
		}
}
```

#### 3.SendMapToHost (DV)

- E142MapData：E142MapDataUploadFormat 为 ASCII 或 BINARY 时的 `Map` 数据
- E142SubstrateType：`Map` 数据的基底 类型
- E142SubstrateID：`Map` 数据的基底 ID

```C# title="CC142.cs"
public bool SendMapToHost(string mapdata, string substrateType, string substrateID)
{
	try
	{
		switch (_E142MapDataUploadFormat)
		{
			case eE142ItemPartFormat.ASCII:
				{
					mapDataDVName = new string[] { "E142MapData", "E142SubstrateType", "E142SubstrateID" };
					dataValues = new Cimetrix.Value.CxValue[] {
						new AValue(mapdata),
						new AValue(substrateType),
						new AValue(substrateID)
					};
				}
				break;
			case eE142ItemPartFormat.BINARY:
			default:
				{
					mapDataDVName = new string[] { "E142MapData", "E142SubstrateType", "E142SubstrateID" };
					dataValues = new Cimetrix.Value.CxValue[] {
						new BiValue(UTF8Encoding.UTF8.GetBytes(mapdata)),
						new AValue(substrateType),
						new AValue(substrateID)
					};
				}
				break; 
		}

		SendCollectionEventWithData(0, mapDataDVName, dataValues, "E142MapDataReady");
		return true;
	}
	catch (Exception ex)
	{
		Log.WriteExceptionCatch(Source, ex);
		return false;
	}
}
```

#### 4.E142MapDataReady (Event)

```C# title="Form1.cs"
private void buttonWaferMapUpload_Click(object sender, EventArgs e)
{
	string mapData = E142.MapDataConverter.Serialize(_MapData);
	_CC142.SendMapToHost(mapData, cmbSbType.Text, txtStripId.Text);

	SaveMapToDisk("Strip", txtStripId.Text + "_" + DateTime.Now.ToString("HHmmss"), mapData);
}
```

- E142MapDataReady

```C# title="CC142.cs"
public bool SendMapToHost(string mapdata, string substrateType, string substrateID)
{
	try
	{
		switch (_E142MapDataUploadFormat)
		{
			case eE142ItemPartFormat.ASCII:
				{
					mapDataDVName = new string[] { "E142MapData", "E142SubstrateType", "E142SubstrateID" };
					dataValues = new Cimetrix.Value.CxValue[] {
						new AValue(mapdata),
						new AValue(substrateType),
						new AValue(substrateID)
					};
				}
				break;
			case eE142ItemPartFormat.BINARY:
			default:
				{
					mapDataDVName = new string[] { "E142MapData", "E142SubstrateType", "E142SubstrateID" };
					dataValues = new Cimetrix.Value.CxValue[] {
						new BiValue(UTF8Encoding.UTF8.GetBytes(mapdata)),
						new AValue(substrateType),
						new AValue(substrateID)
					};
				}
				break; 
		}

		SendCollectionEventWithData(0, mapDataDVName, dataValues, "E142MapDataReady");
		return true;
	}
	catch (Exception ex)
	{
		Log.WriteExceptionCatch(Source, ex);
		return false;
	}
}
```


### 二、Equipment 向 Host 请求 Map 数据

- 1、初始化时 注册 S14F2

```C# title="Register S14F2"
// Register to be notified when S14F2 is received
_CxClientClerk.RegisterMsgHandler(_Connection, SFtoMsgID(14, 2), this);
```

- 2、（S14F1）Equipment 向 Host 请求 Map 数据

```c# title="Equipment → Host"

SubstrateType = "Strip";
SubstrateId = "ToSiPStrip";

_CxClientClerk.SendMessage(_Connection, SFtoMsgID(14, 1), message, true, true, ref TID, this);
```

- 3、（S14F2）接收 Host 发送的消息 

```C# title="Host → Equipment"
void ICxEMAppCallback.MessageReceived(int connectionID, int messageID, CxValueObject message, bool replyExpected, int transactionID, ref int replyMessageID, CxValueObject replyMessage, ref MessageResults result)
{
	try
	{
		MsgIDtoSF(messageID, out var s, out var f);

		var msgString = message.CopyToSMNStringN(0, 0, 256);
		Log.WriteIfEnabled(LogCategory.Information, Source, $"Message Received: S{s.ToString()},F {f.ToString()} :{msgString}");

		result = MessageResults.mReplyLater;
		switch (messageID)
		{
			case 0xe02: //S14F2
				HandleS14F2(transactionID, message);
				replyMessageID = 0;
				result = MessageResults.mNoReply;
				break; 
		}
		OnMyMessageReceived(connectionID, s, f, replyExpected, transactionID, message);
	}
	catch (Exception ex)
	{
		Log.WriteExceptionCatch(Source, ex);
	}
}
```


在SEMI标准中，**S14F1** 和 **S14F2** 是与设备通信有关的SECS-II（Semiconductor Equipment Communication Standard, Second Edition）消息对，用于特定服务的请求和响应。它们通常与对象服务（Object Services）相关联。以下是它们的基本定义：

- **S14F1 (Request for Object Attributes):**  
  这是对象服务中的请求消息，用于向设备请求特定对象的属性。主机（Host）发送这条消息，要求设备返回某个对象的属性数据。

- **S14F2 (Object Attributes):**  
  这是对 **S14F1** 消息的响应消息。设备在收到 **S14F1** 请求后，返回相应的对象属性数据。

在SEMI E142标准中，这些消息对通常用于设备与主机之间的数据交换，特别是在对象相关的服务操作中，例如获取基板的属性信息或映射数据。

### 如何使用：

- **S14F1（请求对象属性）**: 
  主机可以使用 **S14F1** 消息向设备请求 Strip 或 Wafer Map 的属性。这条消息会告诉设备，主机希望获取特定对象（例如，Strip 或 Wafer Map）的相关数据。

- **S14F2（返回对象属性）**:
  设备在收到 **S14F1** 请求后，会通过 **S14F2** 消息返回主机所请求的属性数据，例如 Strip 或 Wafer 的地图信息、坐标、布局等。

### 应用场景：

在半导体制造过程中，**S14F1** 和 **S14F2** 消息可以被用于以下场景：

- **获取基板映射数据**：主机向设备发送 **S14F1** 消息，要求获取特定基板（如 Wafer 或 Strip）的映射数据，设备则通过 **S14F2** 消息返回这些数据。

- **确认设备数据一致性**：在设备之间传输基板数据前，主机可以使用这对消息来确保设备所持有的基板地图与主机所期望的一致。

这些消息的使用依赖于 SECS-II 协议的实现，并且适用于需要对象服务（Object Services）的场景。


### 三、（S6,F11 ）Equipment  Host 

### 四、事件

#### 1.MapDataReceivedHandler

```C#
void HandleS14F2(int transactionID, CxValueObject message)
{
  OnMapDataReceivedHandler(OBJID, sMapData);
}
```

- 控件显示 map 

```C# title="_MapData"
private void CC142_onMapDataReceivedHandler(object sender, CC142.MapDataReceivedEventArgs e)
{
	if( e.SubstrateID == txtStripId.Text )
	{
		// DEMO Key
		SaveMapToDisk("Strip", txtStripId.Text + "_" + DateTime.Now.ToString("HHmmss"), e.MapData); //save the mapdata from secs ii message

		_MapData = E142.MapDataConverter.Deserialize(e.MapData);
		LogSafe($"MapData received for wafer substrate: {e.SubstrateID}");
		cbFromLayouts.DataSource = _MapData.SubstrateMaps.Select(m => m.LayoutSpecifier).ToList();
		cbFromLayouts.Enabled = _MapData.SubstrateMaps.Count > 1;
		mapControlTargetMap.Display(_MapData);
	}
}
```

#### 2.MapDataErrorHandler

```C#
void HandleS14F2(int transactionID, CxValueObject message)
{
  string errorMessage = "S14F2 message format is wrong. Not a list.";
  OnMapDataErrorHandler(OBJID, errorMessage);
}
```

- 记录`map`下载时出现的错误

```C#
private void CC142_onMapDataErrorHandler(object sender, CC142.MapDataErrorEventArgs e)
{
	if( e.ErrorList == null )
	{
		LogSafe(e.ErrorMessage);
	}
	else
	{
		string errorMessage = e.ErrorMessage;
		foreach( var tuple in e.ErrorList )
		{
			errorMessage += " " + tuple.Item2;
		}
		LogSafe(errorMessage);
	}
}
```

#### ItemReceivedHandler

```C#
void Handle21F6(int transactionID, CxValueObject message)
{
  OnItemReceivedHandler(ITEMTYPE, ITEMID, itemFileName, itemPartFormat);  
}
```

```C#
private void CC142_onItemReceivedHandler(object sender, CC142.ItemReceivedEventArgs e)
{
	if( InvokeRequired )
	{
		BeginInvoke(new CC142.ItemReceivedHandler(CC142_onItemReceivedHandler), new[] { sender, e });
		return;
	}
	LogSafe($"Item received: {e.ITEMTYPE}:{e.ITEMID} file:{e.FILENAME}");

	switch( e.ITEMTYPE )
	{
		case "SEMI:MAPDATALAYOUT":
			// Get the map layout from the file. 
			var E142LayoutData = E142.MapDataConverter.Deserialize(GetMapDataFromFile(e.FILENAME));

			//if( e.ITEMID == textBoxDestinationLayoutID.Text )
			//{
			//	_MapDataDestination.Layouts = E142LayoutData.Layouts;
			//	mapControlDestination.Display(_MapDataDestination);
			//}
			//if( e.ITEMID == textBoxSourceLayoutID.Text )
			//{
			//	_MapDataSource.Layouts = E142LayoutData.Layouts;
			//	mapControlSource.Display(_MapDataSource);
			//}
			break;

	}
}
```

#### ItemRequestErrorHandler

```C#
void Handle21F6(int transactionID, CxValueObject message)
{
  string errorMessage = "S12F6 message format is wrong. Not a list.";
  OnItemRequestErrorHandler(ITEMTYPE, ITEMID, errorMessage);
}
```

```C#
private void CC142_onItemRequestErrorHandler(object sender, CC142.ItemRequestErrorEventArgs e)
{
	LogSafe(e.ErrorMessage);
}
```