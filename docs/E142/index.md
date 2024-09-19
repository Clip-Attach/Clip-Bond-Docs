
## 问题

1. E142 主要负责哪些功能？它是否仅用于上传和下载 Map？

2. E142 是否依赖于 ALPS 才能使用？在程序开发中，如果只有 E142 的 License 而没有 ALPS 的 License，E142 可以单独使用吗？

3. 在只使用 E142 而不使用 ALPS 的情况下，E142 是否具备基本的格式转换功能？它能否将其他类型的 Map 转换为 .xml（E142 标准协议）？如果不能，它具体能转换哪些格式？或者它能替我们减轻哪些转换任务？

4. 在只使用 E142 而不使用 ALPS 的情况下，如果仅需上传和下载 Map，需要兼容哪些 Map 格式转换？这些格式仅包括四种吗？（Ascii，Decimal，HexaDecimal，Integer2）

![](https://easyimage.ghuang.top/i/2024/09/05/103709-1.webp)


5. ALPS 支持哪些 Map 格式转换？是否支持下表中的格式？

- Source: Internet

![](https://easyimage.ghuang.top/i/2024/09/05/135605-1.webp)



6. 最终的软件配置应如何选择？

   - **可选项：SECS/GEM，E142，ALPS**
   - **E142：** 主要用于上传和下载。
   - **ALPS：** 支持可视化、格式转换、编辑 Map，以及追溯功能。

   **配置选项：**

   - 6.1 Basic
   - 6.2 Basic + SECS/GEM (VRO)
   - 6.3 Basic + SECS/GEM + E142
   - 6.4 Basic + SECS/GEM + ALPS (Map 格式转换)
   - 6.5 Basic + SECS/GEM + E142 + ALPS


- 7.如何使用 ALPS 来创建和编辑 Map？

![](https://easyimage.ghuang.top/i/2024/09/05/142426-1.webp)


## 开发步骤

### 一、E142的上传和下载

#### 1. E142.2 Single (基本的)
- S14, F1/F2 
- S6, F11/F12

| Service Name | Stream, Function | SECS II Message Name                                        |
| ------------ | ---------------- | ----------------------------------------------------------- |
| MapDownload  | S14,F1/2         | Object Services(SEMI E39.1) – GetAttr Request/ GetAttr Data |
| MapUpload    | S6,F11           | Data Collection(SEMI E5) – Event Report Send                |


#### 2. E142.4 Multi（大于16M的数据）
- S21 F1/F2
- S21 F3/F4
- S21 F5/F6
- S21 F15/F16
- S21 F17/F18

- **Equipment 上传下载** ✔️
- **Host 主动获取** ❌ （不常用）


| **Service Name**          | **Stream, Function**               | **SECS II Message Name**                                                                                                                                  | Supported                                                                                                                         |
|---------------------------|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| **MapDownload**           | Equipment Initiated Single Message | S21F5/6: Equipment sends S21F5 to request the map data. If accepted, the host returns the map data in the S21F6 reply message.                              | Yes                           |
|                           | Equipment Initiated Multiple Message | S21F15/16 and S21F17/18: Equipment sends S21F15 to request the map data. If accepted, the host sends the map data using S21F17 messages.                   | Yes                |
|                           | Host Initiated Single Message      | S21F1/F2 and S21F3/F4: Host sends S21F1 to request permission to send the map data to the equipment. If accepted, the host sends S21F3 with the map data.  | No |
|                           | Host Initiated Multiple Message    | S21F13/14 and S21F17/18: Host sends S21F13 to request permission to send the map data to the equipment. If accepted, the host sends the map data using S21F17 messages. | No |
| **MapUpload**             | Equipment Initiated Single Message | S21F1/F2 and S21F3/F4: Equipment sends S21F1 to request permission to send map data. If accepted, the equipment sends the map data using S21F3.            | Yes         |
|                           | Equipment Initiated Multiple Message | S21F13/14 and S21F17/18: Equipment sends S21F13 requesting permission to send map data. If accepted, the equipment sends the map data using S21F17 messages. | Yes |
|                           | Host Initiated Single Message      | S21F5/6: Host requests map data using S21F5. If accepted, the equipment returns the map data in the S21F6 reply message.                                    | No                                  |
|                           | Host Initiated Multiple Message    | S21F15/16 and S21F17/18: Host requests map data using S21F15. If accepted, the equipment sends map data using S21F17 messages.                              | No                            |


### 二、Map可视化

- 根据我们的Clip和Die设备，使用ALPS生成对应的 Map.xml 文件，导入到Demo中测试，包括测试coordinate和Map动画

#### 1. StripMap (Clip)
#### 2. WaferMap
#### 3. TransferMap (Strip ＋ Wafer) (Die)

![Demo Map](https://easyimage.ghuang.top/i/2024/09/04/165539-1.webp)

### 三、嵌入到现有软件

- 经过 二、Map可视化后测试后，我们就可以将 Map的功能嵌入到设备上
- 需要注意的是，在开发前期，我们需要选择好配置（SECS/GEM，E142，ALPS），因为这不仅涉及到成本，还涉及到软件的架构。后期修改软件架构会造成软件的不稳定性和大量不必要的开发工作。

#### 1. Die
#### 2. Clip

### 四、平面/凹口方向

- 晶圆的物理定位

![](https://easyimage.ghuang.top/i/2024/09/20/003049-1.webp)

### 四、原点位置及方向

- 晶圆在逻辑坐标系中的表示

![](https://easyimage.ghuang.top/i/2024/09/20/002940-1.webp)

1. **LowerLeft UpRight**  
   原点位于左下角，X 轴向右，Y 轴向上。

2. **UpperLeft DownRight**  
   原点位于左上角，X 轴向右，Y 轴向下。

3. **UpperRight DownLeft**  
   原点位于右上角，X 轴向左，Y 轴向下。

4. **LowerRight UpLeft**  
   原点位于右下角，X 轴向左，Y 轴向上。

5. **Center UpRight**  
   原点位于中心，X 轴向右，Y 轴向上。

这些类型显示了不同的坐标系设置，可以用于视觉或图像处理中的坐标变换和对齐问题。