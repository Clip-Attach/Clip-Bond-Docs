

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

- 帮我把表格转换成 [id=name, description, text, setEventID, clearEventID, alarm code (ALCD), ]

例如：

- 把下面的表格

```sh
| ID   | Name   | Description                                         | setEventID | clearEventID | alarm code | Text                       |
| ---- | ------ | --------------------------------------------------- | ---------- | ------------ | ---------- | -------------------------- |
| 1    | AC0101 | Door switch detection is abnormal!                  | 1001       | 2001         | 6          | 门开关检测异常！           |
| 2    | AC0102 | Window already open;no need to open it again        | 1001       | 2001         | 6          | 窗口已打开,无需重复打开    |
| 3    | AC0103 | Startup failed;please reset and start again!        | 1001       | 2001         | 6          | 启动失败，请复位后再启动！ |
| 4    | AC0104 | Failed to load power supply!                        | 1001       | 2001         | 6          | 加载电源失败！             |
```

- 转换成 

```sh
[id=name, description, text, setEventID, clearEventID, alarm code (ALCD), ]
8101=AC0101,Door switch detection is abnormal!,Door switch detection is abnormal!,1001,2001,6,
8102=AC0102,Window already open;no need to open it again,Window already open;no need to open it again,1001,2001,6,
8103=AC0103,Startup failed;please reset and start again!,Startup failed;please reset and start again!,1001,2001,6,
8139=AC0104,Failed to load power supply!,Failed to load power supply!,1001,2001,6,
```

- 注意事项
- 1、输出内容去除掉  [id=name, description, text, setEventID, clearEventID, alarm code (ALCD), ]
- 2、description和text相同都是英文

最终输出内容：

```sh
8101=AC0101,Door switch detection is abnormal!,Door switch detection is abnormal!,1001,2001,6,
8102=AC0102,Window already open;no need to open it again,Window already open;no need to open it again,1001,2001,6,
8103=AC0103,Startup failed;please reset and start again!,Startup failed;please reset and start again!,1001,2001,6,
8139=AC0104,Failed to load power supply!,Failed to load power supply!,1001,2001,6,
```

很好，下面我提供给你表格。你帮我转换成固定的格式
[id=name, description, text, setEventID, clearEventID, alarm code (ALCD), ]