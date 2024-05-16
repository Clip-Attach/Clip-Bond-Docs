# 14-TinAUI die bonding alarm code

| ID   | Name   | description                                           | setEventID | clearEventID | alarm code | Text                                                   |
| ---- | ------ | ----------------------------------------------------- | ---------- | ------------ | ---------- | ------------------------------------------------------ |
| 1    | AC1401 | 输入非法参数！                                       | 1001       | 2001         | 6          | Illegal parameter input!                               |
| 2    | AC1402 | 提示&输入非法参数！                                 | 1001       | 2001         | 6          | Prompt& input illegal parameter!                      |
| 3    | AC1403 | 提示&整体修改设定了非法参数！                       | 1001       | 2001         | 6          | Reminder& the overall modification has set illegal parameters! |
| 4    | AC1404 | 请初始化后在操作！                                   | 1001       | 2001         | 6          | Please initialize before proceeding!                   |
| 5    | AC1405 | 请停止后在操作！                                     | 1001       | 2001         | 6          | Please stop before proceeding!                         |
| 6    | AC1406 | 请选择坐标点！                                       | 1001       | 2001         | 6          | Please select a coordinate point!                      |
| 7    | AC1407 | 左点胶XY电机运动超时！                             | 1001       | 2001         | 6          | Left dispensing XY motor movement timeout!             |
| 8    | AC1408 | 提示&请暂停后在操作！                             | 1001       | 2001         | 6          | Prompt& please pause before proceeding!                |
| 9    | AC1409 | 提示&左点胶Z不在原位                              | 1001       | 2001         | 6          | Reminder& left dispensing Z is not in place            |
| 10   | AC1410 | 提示&窗口已打开&请勿重复操作                   | 1001       | 2001         | 6          | Prompt& the window is already open& please do not repeat the operation |
| 11   | AC1411 | 左点胶Z不在原位                                    | 1001       | 2001         | 6          | Left dispensing Z not in place                         |
| 12   | AC1412 | 左点胶测高信号异常！                               | 1001       | 2001         | 6          | Left glue dispensing height measurement signal abnormal! |
| 13   | AC1413 | 获取左点胶图像Mark点十字中心异常&标定失败！       | 1001       | 2001         | 6          | The center of the Mark dot cross in obtaining the left glue image is abnormal& calibration failed! |
| 14   | AC1414 | Z下降时间不能大于1000ms                            | 1001       | 2001         | 6          | Z descent time cannot exceed 1000ms                    |
| 15   | AC1415 | Z下降时间不能小于10ms                              | 1001       | 2001         | 6          | Z descent time cannot be less than 10ms                |
| 16   | AC1416 | Z上升时间不能大于1000ms                            | 1001       | 2001         | 6          | Z rise time cannot exceed 1000ms                       |
| 17   | AC1417 | Z上升时间不能小于10ms                              | 1001       | 2001         | 6          | Z rise time cannot be less than 10ms                   |
| 18   | AC1418 | XYZ数据整体修改设定了非法参数！                    | 1001       | 2001         | 6          | The overall modification of XYZ data has set illegal parameters! |
| 19   | AC1419 | 点胶1Z不在原位                                     | 1001       | 2001         | 6          | Glue dispensing 1Z not in place                        |
| 20   | AC1420 | X偏移不能大于8mm                                   | 1001       | 2001         | 6          | X offset cannot be greater than 8mm                   |
| 21   | AC1421 | X偏移不能小于-8mm                                  | 1001       | 2001         | 6          | The X offset cannot be less than -8mm                  |
| 22   | AC1422 | Y偏移不能大于8mm                                   | 1001       | 2001         | 6          | Y offset cannot be greater than 8mm                   |
| 23   | AC1423 | Y偏移不能小于-8mm                                  | 1001       | 2001         | 6          | Y offset cannot be less than -8mm                     |
| 24   | AC1424 | X整体偏移不能大于8mm                               | 1001       | 2001         | 6          | The overall offset of X cannot be greater than 8mm    |
| 25   | AC1425 | X整体偏移不能小于-8mm                              | 1001       | 2001         | 6          | The overall offset of X cannot be less than -8mm      |
| 26   | AC1426 | Y整体偏移不能大于8mm                               | 1001       | 2001         | 6          | The overall offset of Y cannot be greater than 8mm    |
| 27   | AC1427 | Y整体偏移不能小于-8mm                              | 1001       | 2001         | 6          | The overall offset of Y cannot be less than -8mm      |
| 28   | AC1428 | Z整体偏移向上不能大于2mm                           | 1001       | 2001         | 6          | The overall offset of Z cannot exceed 2mm upwards     |
| 29   | AC1429 | Z整体偏移向上偏移最小0mm                           | 1001       | 2001         | 6          | Z overall offset with a minimum upward offset of 0mm  |
| 30   | AC1430 | 窗口已打开&请勿重复操作！                        | 1001       | 2001         | 6          | The window is already open& please do not repeat the operation |
| 31   | AC1431 | 相机采集图片超时&标定失败！                       | 1001       | 2001         | 6          | The camera image collection timed out and the calibration failed! |
| 32   | AC1432 | 夹角超出±10°&标定失败！                           | 1001       | 2001         | 6          | The included angle exceeds ± 10 °& calibration failed! |



```sh
9401=AC1401,Illegal parameter input!,Illegal parameter input!,1001,2001,6,
9402=AC1402,Prompt& input illegal parameter!,Prompt& input illegal parameter!,1001,2001,6,
9403=AC1403,Reminder& the overall modification has set illegal parameters!,Reminder& the overall modification has set illegal parameters!,1001,2001,6,
9404=AC1404,Please initialize before proceeding!,Please initialize before proceeding!,1001,2001,6,
9405=AC1405,Please stop before proceeding!,Please stop before proceeding!,1001,2001,6,
9406=AC1406,Please select a coordinate point!,Please select a coordinate point!,1001,2001,6,
9407=AC1407,Left dispensing XY motor movement timeout!,Left dispensing XY motor movement timeout!,1001,2001,6,
9408=AC1408,Prompt& please pause before proceeding!,Prompt& please pause before proceeding!,1001,2001,6,
9409=AC1409,Reminder& left dispensing Z is not in place,Reminder& left dispensing Z is not in place,1001,2001,6,
9410=AC1410,Prompt& the window is already open& please do not repeat the operation,Prompt& the window is already open& please do not repeat the operation,1001,2001,6,
9411=AC1411,Left dispensing Z not in place,Left dispensing Z not in place,1001,2001,6,
9412=AC1412,Left glue dispensing height measurement signal abnormal!,Left glue dispensing height measurement signal abnormal!,1001,2001,6,
9413=AC1413,The center of the Mark dot cross in obtaining the left glue image is abnormal& calibration failed!,The center of the Mark dot cross in obtaining the left glue image is abnormal& calibration failed!,1001,2001,6,
9414=AC1414,Z descent time cannot exceed 1000ms,Z descent time cannot exceed 1000ms,1001,2001,6,
9415=AC1415,Z descent time cannot be less than 10ms,Z descent time cannot be less than 10ms,1001,2001,6,
9416=AC1416,Z rise time cannot exceed 1000ms,Z rise time cannot exceed 1000ms,1001,2001,6,
9417=AC1417,Z rise time cannot be less than 10ms,Z rise time cannot be less than 10ms,1001,2001,6,
9418=AC1418,The overall modification of XYZ data has set illegal parameters!,The overall modification of XYZ data has set illegal parameters!,1001,2001,6,
9419=AC1419,Glue dispensing 1Z not in place,Glue dispensing 1Z not in place,1001,2001,6,
9420=AC1420,X offset cannot be greater than 8mm,X offset cannot be greater than 8mm,1001,2001,6,
9421=AC1421,The X offset cannot be less than -8mm,The X offset cannot be less than -8mm,1001,2001,6,
9422=AC1422,Y offset cannot be greater than 8mm,Y offset cannot be greater than 8mm,1001,2001,6,
9423=AC1423,Y offset cannot be less than -8mm,Y offset cannot be less than -8mm,1001,2001,6,
9424=AC1424,The overall offset of X cannot be greater than 8mm,The overall offset of X cannot be greater than 8mm,1001,2001,6,
9425=AC1425,The overall offset of X cannot be less than -8mm,The overall offset of X cannot be less than -8mm,1001,2001,6,
9426=AC1426,The overall offset of Y cannot be greater than 8mm,The overall offset of Y cannot be greater than 8mm,1001,2001,6,
9427=AC1427,The overall offset of Y cannot be less than -8mm,The overall offset of Y cannot be less than -8mm,1001,2001,6,
9428=AC1428,The overall offset of Z cannot exceed 2mm upwards,The overall offset of Z cannot exceed 2mm upwards,1001,2001,6,
9429=AC1429,Z overall offset with a minimum upward offset of 0mm,Z overall offset with a minimum upward offset of 0mm,1001,2001,6,
9430=AC1430,The window is already open& please do not repeat the operation,The window is already open& please do not repeat the operation,1001,2001,6,
9431=AC1431,The camera image collection timed out and the calibration failed!,The camera image collection timed out and the calibration failed!,1001,2001,6,
9432=AC1432,The included angle exceeds ± 10 °& calibration failed!,The included angle exceeds ± 10 °& calibration failed!,1001,2001,6,
```