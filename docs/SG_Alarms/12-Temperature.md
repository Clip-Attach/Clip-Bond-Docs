# 12-Temperature die bonding alarm code

| ID   | Name   | description                        | setEventID | clearEventID | alarm code | Text                                    |
| ---- | ------ | ---------------------------------- | ---------- | ------------ | ---------- | --------------------------------------- |
| 1    | AC1201 | 灯光串口初始化失败！              | 1001       | 2001         | 6          | Light serial port initialization failed! |
| 2    | AC1202 | 灯光串口没有打开&请打开串口！   | 1001       | 2001         | 6          | The light serial port is not open& please open the serial port! |
| 3    | AC1203 | 读取XML文件有误                   | 1001       | 2001         | 6          | Error reading XML file                  |
| 4    | AC1204 | 输入非法参数！                    | 1001       | 2001         | 6          | Illegal parameter input!                |
| 5    | AC1205 | 串口没有打开&请打开串口！       | 1001       | 2001         | 6          | The serial port is not open& please open it! |
| 6    | AC1206 | 设定温度失败&请重新操作         | 1001       | 2001         | 6          | Failed to set temperature& please try again |
| 7    | AC1207 | 设定AT失败&请重新操作           | 1001       | 2001         | 6          | Failed to set AT& please try again      |
| 8    | AC1208 | 设定参数失败&请重新操作         | 1001       | 2001         | 6          | Failed to set parameters& please try again |



```sh
9201=AC1201,Light serial port initialization failed!,Light serial port initialization failed!,1001,2001,6,
9202=AC1202,The light serial port is not open& please open the serial port!,The light serial port is not open& please open the serial port!,1001,2001,6,
9203=AC1203,Error reading XML file,Error reading XML file,1001,2001,6,
9204=AC1204,Illegal parameter input!,Illegal parameter input!,1001,2001,6,
9205=AC1205,The serial port is not open& please open it!,The serial port is not open& please open it!,1001,2001,6,
9206=AC1206,Failed to set temperature& please try again,Failed to set temperature& please try again,1001,2001,6,
9207=AC1207,Failed to set AT& please try again,Failed to set AT& please try again,1001,2001,6,
9208=AC1208,Failed to set parameters& please try again,Failed to set parameters& please try again,1001,2001,6,
```