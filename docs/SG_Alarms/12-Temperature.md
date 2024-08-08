# 12-Temperature die bonding alarm code(OK)

| ID   | Name   | Description                                                  | setEventID | clearEventID | alarm code | Text                           |
| ---- | ------ | ------------------------------------------------------------ | ---------- | ------------ | ---------- | ------------------------------ |
| 1    | AC1201 | Light serial port initialization failed!                     | 1001       | 2001         | 6          | 灯光串口初始化失败！           |
| 2    | AC1202 | The light serial port is not open;please open the serial port! | 1001       | 2001         | 6          | 灯光串口没有打开，请打开串口！ |
| 3    | AC1203 | Illegal parameter input!                                     | 1001       | 2001         | 6          | 输入非法参数！                 |
| 4    | AC1204 | The serial port is not open;please open it!                  | 1001       | 2001         | 6          | 串口没有打开，请打开串口！     |
| 5    | AC1205 | Failed to set temperature;please try again                   | 1001       | 2001         | 6          | 设定温度失败，请重新操作       |
| 6    | AC1206 | Failed to set AT;please try again                            | 1001       | 2001         | 6          | 设定AT失败，请重新操作         |
| 7    | AC1207 | Failed to set parameters;please try again                    | 1001       | 2001         | 6          | 设定参数失败，请重新操作       |



```sh
9201=AC1201,Light serial port initialization failed!,Light serial port initialization failed!,1001,2001,6,
9202=AC1202,The light serial port is not open;please open the serial port!,The light serial port is not open;please open the serial port!,1001,2001,6,
9203=AC1203,Illegal parameter input!,Illegal parameter input!,1001,2001,6,
9204=AC1204,The serial port is not open;please open it!,The serial port is not open;please open it!,1001,2001,6,
9205=AC1205,Failed to set temperature;please try again,Failed to set temperature;please try again,1001,2001,6,
9206=AC1206,Failed to set AT;please try again,Failed to set AT;please try again,1001,2001,6,
9207=AC1207,Failed to set parameters;please try again,Failed to set parameters;please try again,1001,2001,6,

```