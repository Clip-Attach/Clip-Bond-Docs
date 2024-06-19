
# Summary

## 1.2.Operator_Interface

### epj 文件

```ini title=".epj"
[COMMON VARIABLES]
#varTypes DV,SV,EC
#valTypes I1, I2, I4, I8, U1, U2, U4, U8, F4, F8, A, Bo, Bi, L, J, W
#id=name, description, units, varType, valType, eventID, private, persistant, min, max, default, 
#Add your equipment definitions here

100=ConnStat,Example user defined data variable.,,DV,U4,,0,0,,,U4 1,

```

### C# 使用

#### 1、初始化

```c# title="Demo.cs"
/// <summary>
/// 操作界面
/// </summary>
Form_Operator form_Operator;

/// <summary>
/// 初始化
/// </summary>
 void init_Operator()
 {
     form_Operator = new Form_Operator();
     form_Operator.FormBorderStyle = FormBorderStyle.None;   //无边框
     form_Operator.Dock = DockStyle.Fill;
     form_Operator.TopLevel = false;
     form_Operator.Show();
     panel1.Controls.Add(form_Operator);

     form_Operator.Initialize(1 == 1 ? IsOpen.ON : IsOpen.OFF, "CIMConnectCSVS2019.epj");
 }

```

#### 2、销毁回调函数

```c# title="Demo.cs"
/// <summary>
/// 销毁回调函数
/// </summary>
void clos_Operator()
{
    form_Operator.GEMClosing();
}
```

#### 3、State Machine 未完成


### 验证测试

![](https://easyimage.ghuang.top/i/2024/06/09/190511-1.webp)

![](https://easyimage.ghuang.top/i/2024/06/09/190842-1.webp)



## 3.3.Equipment_Constants

### epj 文件

```ini title=".epj"
[COMMON VARIABLES]
#varTypes DV,SV,EC
#valTypes I1, I2, I4, I8, U1, U2, U4, U8, F4, F8, A, Bo, Bi, L, J, W
#id=name, description, units, varType, valType, eventID, private, persistant, min, max, default, 
#Add your equipment definitions here
38001=EC38001,Equipment ID,,EC,A,,0,0,,,A 32767,
38010=EC38010,Production Statistics,,EC,I4,,0,0,,,I4 0,
```

### C# 使用

#### 1、初始化

```c# title="Demo.cs"

/// <summary>
/// 设备ID
/// </summary>
public EquipmentConstants<string> EquipmentID;

/// <summary>
/// 生产统计
/// </summary>
public EquipmentConstants<int> ProductionStatistics;

/// <summary>
/// 初始化
/// </summary>
public void init_EquipmentConstants()
{
   EquipmentID = new EquipmentConstants<string>(38001, "EC38001", call_EquipmentID);
   ProductionStatistics = new EquipmentConstants<int>(38010, "EC38010", call_ProductionStatistics);
}

/// <summary>
/// `EquipmentID` 值修改触发的回调
/// </summary>
void call_EquipmentID(string value)
{
   MessageBox.Show(value);
}

/// <summary>
///  `ProductionStatistics` 值修改触发的回调
/// </summary>
void call_ProductionStatistics(int value)
{
   MessageBox.Show(value.ToString());
}

```

#### 2、销毁回调函数

```c# title="Demo.cs"
/// <summary>
/// 销毁回调函数
/// </summary>
public void clos_EquipmentConstants()
{
   EquipmentID.Dispose();
   ProductionStatistics.Dispose();
}
```

#### 3、操作参数

```c# title="Demo.cs"
private void button1_Click(object sender, EventArgs e)
{
   CMyTools.SendVariable(0, "EC38001", "123");
   string value1 = EquipmentID.Variable;
   EquipmentID.Variable = "456";
   string value2 = EquipmentID.Variable;


   CMyTools.SendVariable(0, "EC38010", 123);
   int value3 = ProductionStatistics.Variable;
   ProductionStatistics.Variable = 456;
   int value4 = ProductionStatistics.Variable;
}
```

### 验证测试

- Debug

![](https://easyimage.ghuang.top/i/2024/06/18/191141-1.webp)

![](https://easyimage.ghuang.top/i/2024/06/18/191235-1.webp)

![](https://easyimage.ghuang.top/i/2024/06/18/191655-1.webp)


## 4.2.Remote_Commands

### C# 使用

#### 1、初始化

```c# title="Demo.cs"

/// <summary>
/// 远程锁定机器
/// </summary>
RemoteCommand reLockMachine;

/// <summary>
/// 远程启动机器
/// </summary>
RemoteCommand reStartMachine;

/// <summary>
/// 初始化
/// </summary>
void init_RemoteCommand()
{
    reLockMachine = new RemoteCommand("LockMachine", "1. Lock machine.", act_LockMachine);
    reStartMachine = new RemoteCommand("StartMachine", "2. Start machine.", act_StartMachine);
}

/// <summary>
/// `reLockMachine` 远程锁定机器时，触发的回调
/// </summary>
void act_LockMachine()
{
    MessageBox.Show("1. Lock machine.");
}

/// <summary>
/// `reStartMachine` 远程启动机器时，触发的回调
/// </summary>
void act_StartMachine()
{
    MessageBox.Show("2. Start machine.");
}

```

#### 2、销毁回调函数

```c# title="Demo.cs"
/// <summary>
/// 销毁回调函数
/// </summary>
void clos_RemoteCommand()
{
    reLockMachine.Dispose();
    reStartMachine.Dispose();
}
```

#### 3、远程作业时，自动触发的回调

```c# title="Demo.cs"
/// <summary>
/// `reLockMachine` 远程锁定机器时，触发的回调
/// </summary>
void act_LockMachine()
{
    // 加入业务逻辑
}

/// <summary>
/// `reStartMachine` 远程启动机器时，触发的回调
/// </summary>
void act_StartMachine()
{
    // 加入业务逻辑
}

```

### 验证测试

- S2F41
- token:clip-attach

#### 1、GEM Host

- Command: `LockMachine`
- Name: `token`
- Value: `clip-attach`

![](https://easyimage.ghuang.top/i/2024/06/18/194832-1.webp)

![](https://easyimage.ghuang.top/i/2024/06/18/195021-1.webp)


#### 2、Software Application

![](https://easyimage.ghuang.top/i/2024/06/18/195232-1.webp)


```c# title="Demo.cs"
void act_LockMachine()
{
    // 加入业务逻辑
    MessageBox.Show("1. Lock machine.");
}
```