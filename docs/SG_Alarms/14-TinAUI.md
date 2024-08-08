# 14-TinAUI die bonding alarm code(OK)

| ID   | Name   | Description          | setEventID | clearEventID | alarm code | Text                              |
| ---- | ------ | -------------------- | ---------- | ------------ | ---------- | --------------------------------- |
| 1    | AC1401 | Illegal parameter input!   | 1001 | 2001 | 6 | 输入非法参数！                    |
| 2    | AC1402 | Prompt, input illegal parameter! | 1001 | 2001 | 6 | 提示，输入非法参数！              |
| 3    | AC1403 | Reminder, the overall modification has set illegal parameters! | 1001 | 2001 | 6 | 提示，整体修改设定了非法参数！    |
| 4    | AC1404 | Please initialize before proceeding! | 1001 | 2001 | 6 | 请初始化后在操作！                |
| 5    | AC1405 | Please stop before proceeding! | 1001 | 2001 | 6 | 请停止后在操作！                  |
| 6    | AC1406 | Please select a coordinate point! | 1001 | 2001 | 6 | 请选择坐标点！                    |
| 7    | AC1407 | Left dispensing XY motor movement timeout! | 1001 | 2001 | 6 | 左点胶XY电机运动超时！            |
| 8 | AC1408 | Prompt, please pause before proceeding! | 1001 | 2001 | 6 | 提示，请暂停后在操作！ |
| 9 | AC1409 | Reminder, left dispensing Z is not in place | 1001 | 2001 | 6 | 提示，左点胶Z不在原位 |
| 10 | AC1410 | Prompt, the window is already open, please do not repeat the operation | 1001 | 2001 | 6 | 提示，窗口已打开，请勿重复操作 |
| 11 | AC1411 | Left dispensing Z not in place | 1001 | 2001 | 6 | 左点胶Z不在原位 |
| 12   | AC1412 | Left glue dispensing height measurement signal abnormal!     | 1001       | 2001         | 6          | 左点胶测高信号异常！                         |
| 13   | AC1413 | The center of the Mark dot cross in obtaining the left glue image is abnormal, calibration failed! | 1001       | 2001         | 6          | 获取左点胶图像Mark点十字中心异常，标定失败！ |
| 14   | AC1414 | The included angle exceeds ± 10 °, calibration failed!       | 1001       | 2001         | 6          | 夹角超出±10°，标定失败！                     |
| 15   | AC1415 | Glue dispensing 1Z not in place | 1001 | 2001 | 6 | 点胶1Z不在原位                   |
| 16   | AC1416 | X offset cannot be greater than 8mm | 1001 | 2001 | 6 | X偏移不能大于8mm                  |
| 17   | AC1417 | X offset cannot be less than -8mm | 1001 | 2001 | 6 | X偏移不能小于-8mm                 |
| 18   | AC1418 | Y offset cannot be greater than 8mm | 1001 | 2001 | 6 | Y偏移不能大于8mm                  |
| 19   | AC1419 | Y offset cannot be less than -8mm | 1001 | 2001 | 6 | Y偏移不能小于-8mm                 |
| 20   | AC1420 | The overall offset of X cannot be greater than 8mm | 1001 | 2001 | 6 | X整体偏移不能大于8mm             |
| 21   | AC1421 | The overall offset of X cannot be less than -8mm | 1001 | 2001 | 6 | X整体偏移不能小于-8mm             |
| 22   | AC1422 | The overall offset of Y cannot be greater than 8mm | 1001 | 2001 | 6 | Y整体偏移不能大于8mm             |
| 23   | AC1423 | The overall offset of Y cannot be less than -8mm | 1001 | 2001 | 6 | Y整体偏移不能小于-8mm             |
| 24   | AC1424 | The overall offset of Z cannot exceed 2mm upwards | 1001 | 2001 | 6 | Z整体偏移向上不能大于2mm          |
| 25   | AC1425 | Z overall offset with a minimum upward offset of 0mm | 1001 | 2001 | 6 | Z整体偏移向上偏移最小0mm          |
| 26   | AC1426 | The window is already open, please do not repeat the operation | 1001 | 2001 | 6 | 窗口已打开，请勿重复操作           |
| 27   | AC1427 | Z descent time cannot exceed 1000ms | 1001 | 2001 | 6 | Z下降时间不能大于1000ms           |
| 28   | AC1428 | Z descent time cannot be less than 10ms | 1001 | 2001 | 6 | Z下降时间不能小于10ms            |
| 29   | AC1429 | Z rise time cannot exceed 1000ms | 1001 | 2001 | 6 | Z上升时间不能大于1000ms           |
| 30   | AC1430 | Z rise time cannot be less than 10ms | 1001 | 2001 | 6 | Z上升时间不能小于10ms            |
| 31 | AC1431 | The camera image collection timed out and the calibration failed! | 1001 | 2001 | 6 | 相机采集图片超时，标定失败！ |
| 32   | AC1432 | The overall modification of XYZ data has set illegal parameters! | 1001 | 2001 | 6 | XYZ数据整体修改设定了非法参数！  |




```sh
9401=AC1401,Illegal parameter input!,Illegal parameter input!,1001,2001,6,
9402=AC1402,Prompt& input illegal parameter!,Prompt& input illegal parameter!,1001,2001,6,
9403=AC1403,Reminder& the overall modification has set illegal parameters!,Reminder& the overall modification has set illegal parameters!,1001,2001,6,

```