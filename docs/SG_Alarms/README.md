

## Alarm code table (ALCD)  

| ID   | Name                       | Translate      |
| ---- | -------------------------- | -------------- |
| 0    | Unused                     | 未使用         |
| 1    | Personal Safety            | 个人安全       |
| 2    | Equipment Safety           | 设备安全       |
| 3    | Parameter Control  Warning | 参数控制警告   |
| 4    | Parameter Control  Error   | 参数控制错误   |
| 5    | Irrecoverable Error        | 不能挽回的错误 |
| 6    | Equipment Status  Warning  | 设备状态警告   |
| 7    | Attention Flags            | 注意标志       |
| 8    | Data Integrity             | 数据完整性     |
| >8   | Reserved                   | 保留           |


!!! note
    - `ID`：序号
    - `Name`：名称
    - `description`：描述
    - 1、显示：服务器页面【Alarms】报警内容
    - 2、赋值：代码传值
    - `setEventID`：设置事件ID （报警信息）
    - `clearEventID`：清空事件ID （报警信息）
    - `alarm code (ALCD)`：报警码
    - `Text`：报警内容
    - 1、显示：服务器页面【Alarms History】报警记录列表
    - 2、赋值：.epj文件配置

## GPT 引导1

- 帮我转换表格中的内容：

- 把下面的表格

| ID   | Alarm code | Information  English                                         | Information  Chinese                    |
| ---- | ---------- | ------------------------------------------------------------ | --------------------------------------- |
| 1    | AC0101     | Please stop the device before proceeding!                    | 请停止设备后在操作！                    |
| 2    | AC0102     | Entering illegal parameters                                  | 输入非法参数                            |
| 3    | AC0103     | Camera initialization failed, program cannot start....       | 相机初始化失败，程序无法启动.....       |

- 转换成，

| ID   | Name   | description                             | setEventID | clearEventID | alarm code | Text                                                         |
| ---- | ------ | --------------------------------------- | ---------- | ------------ | ---------- | ------------------------------------------------------------ |
| 1    | AC0101 | 请停止设备后在操作！                    | 1001       | 2001         | 6          | Please stop the device before proceeding!                    |
| 2    | AC0102 | 输入非法参数                            | 1001       | 2001         | 6          | Entering illegal parameters                                  |
| 3    | AC0103 | 相机初始化失败，程序无法启动.....         | 1001       | 2001         | 6          | Camera initialization failed, program cannot start....                               |




## GPT 引导2

- 帮我转换并翻译表格中的内容：
- 把下面的表格

```sh
| ID   | Name   | description                             | setEventID | clearEventID | alarm code | Text                                                         |
| ---- | ------ | --------------------------------------- | ---------- | ------------ | ---------- | ------------------------------------------------------------ |
| 1    | AC0101 | 请停止设备后在操作！                    | 1001       | 2001         | 6          | Please stop the device before proceeding!                    |
| 2    | AC0102 | 输入非法参数                            | 1001       | 2001         | 6          | Entering illegal parameters                                  |
| 3    | AC0103 | 左点胶X故障                             | 1001       | 2001         | 6          | Left dispensing X malfunction                                |
| 39   | AC0139 | 伺服电机加使能中 & 请稍等！              | 1001       | 2001         | 6          | Servo motor enable & please wait!                             |
```

- 转换成 

```sh
[id=name, description, text, setEventID, clearEventID, alarm code (ALCD), ]
8101=AC0101,Please stop the equipment before operating!,Please stop the device before proceeding!,1001,2001,6,
8102=AC0102,Entering illegal parameters,Entering illegal parameters,1001,2001,6,
8103=AC0103,Left dispensing X malfunction,Left dispensing X malfunction,1001,2001,6,
8139=AC0139,Servo motor enable & please wait!,Servo motor enable & please wait!,1001,2001,6,
```

- 注意事项
- 1、其中 | description | 列的内容,需要翻译
- 2、其中 | Text | 列的内容,不要出现中文
- 3、输出内容去除掉  [id=name, description, text, setEventID, clearEventID, alarm code (ALCD), ]


## GPT 引导3

- 帮我转换并翻译表格中的内容：
- 把下面的表格

```sh
| ID   | Name   | description                                           | setEventID | clearEventID | alarm code | Text                                              |
| ---- | ------ | ----------------------------------------------------- | ---------- | ------------ | ---------- | ------------------------------------------------- |
| 1    | AC1701 | 请先选择文件&再加载                                | 1001       | 2001         | 6          | Please select a file before loading               |
| 2    | AC1702 | 请选择正确文件&再加载                              | 1001       | 2001         | 6          | Please select the correct file before loading     |
| 3    | AC1703 | 请先选择文件&再删除                                | 1001       | 2001         | 6          | Please select a file before deleting it           |
| 4    | AC1704 | 请先选择参数文件&再加载                            | 1001       | 2001         | 6          | Please select a parameter file before loading     |
| 5    | AC1705 | 请选择正确参数文件&再加载                          | 1001       | 2001         | 6          | Please select the correct parameter file before loading |
| 6    | AC1706 | 请输入新的文件名                                    | 1001       | 2001         | 6          | Please enter a new file name                      |
| 7    | AC1707 | 请先选择正确参数文件&再复制                        | 1001       | 2001         | 6          | Please select the correct parameter file before copying |
| 8    | AC1708 | 请先选择参数文件&再复制                            | 1001       | 2001         | 6          | Please select the parameter file first before copying |
| 9    | AC1709 | 请先选择参数文件&再删除                            | 1001       | 2001         | 6          | Please select the parameter file first before deleting it |
```

- 转换成 

```sh
[id=name, description, text, setEventID, clearEventID, alarm code (ALCD), ]
9701=AC1701,Please select a file before loading,Please select a file before loading,1001,2001,6,
9702=AC1702,Please select the correct file before loading,Please select the correct file before loading,1001,2001,6,
9703=AC1703,Please select a file before deleting it,Please select a file before deleting it,1001,2001,6,
9704=AC1704,Please select a parameter file before loading,Please select a parameter file before loading,1001,2001,6,
9705=AC1705,Please select the correct parameter file before loading,Please select the correct parameter file before loading,1001,2001,6,
9706=AC1706,Please enter a new file name,Please enter a new file name,1001,2001,6,
9707=AC1707,Please select the correct parameter file before copying,Please select the correct parameter file before copying,1001,2001,6,
9708=AC1708,Please select the parameter file first before copying,Please select the parameter file first before copying,1001,2001,6,
9709=AC1709,Please select the parameter file first before deleting it,Please select the parameter file first before deleting it,1001,2001,6,
```

- 注意事项
[id=name, description, text, setEventID, clearEventID, alarm code (ALCD), ]
- 1、[description] 列的内容,中文需要翻译成英文
- 2、[text] 列的内容,中文需要翻译成英文
- 3、[id] 列的内容,以9开头
- 4、输出内容去除掉  [id=name, description, text, setEventID, clearEventID, alarm code (ALCD), ]




