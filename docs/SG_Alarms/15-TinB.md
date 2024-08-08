# 15-TinB die bonding alarm code(OK)

| ID   | Name   | Description                                                  | setEventID | clearEventID | alarm code | Text                               |
| ---- | ------ | ------------------------------------------------------------ | ---------- | ------------ | ---------- | ---------------------------------- |
| 1    | AC1501 | The melting speed of the welding line exceeds the maximum value: | 1001       | 2001         | 6          | 焊线熔化速度超出最大值:            |
| 2    | AC1502 | Failed to update the data of solder wire B!                  | 1001       | 2001         | 6          | 更新送焊线B数据失败！              |
| 3    | AC1503 | No frame information read!                                   | 1001       | 2001         | 6          | 未读取到框架信息！                 |
| 4    | AC1504 | The number of tin point positions exceeds the upper limit of 60 coordinate points! | 1001       | 2001         | 6          | 点锡位置的数量超出上限60个坐标点！ |
| 5    | AC1505 | The dispensing position exceeds the upper limit by 20 points | 1001       | 2001         | 6          | 点胶位超出上限20个点位             |
| 6    | AC1506 | Failed to read framework data!                               | 1001       | 2001         | 6          | 框架数据读取失败！                 |
| 7    | AC1507 | Frame Pad bit exceeds the upper limit of 690                 | 1001       | 2001         | 6          | 框架Pad位超出上限690               |
| 8    | AC1508 | Drawtin B data write failure                                 | 1001       | 2001         | 6          | 画锡B数据写入失败                  |
| 9    | AC1509 | Abnormal detection signal of welding line B                  | 1001       | 2001         | 6          | 焊线B探测信号异常                  |
| 10   | AC1510 | Welding line B detection timeout                             | 1001       | 2001         | 6          | 焊线B探测超时                      |
| 11   | AC1511 | Left dispensing detection abnormal!                          | 1001       | 2001         | 6          | 右点胶预点胶位置满！               |
| 12   | AC1512 | Abnormal right dispensing detection!                         | 1001       | 2001         | 6          | 右点胶检测异常！                   |
| 13   | AC1513 | The right glue dispensing camera is disconnected!            | 1001       | 2001         | 6          | 右点胶相机掉线！                   |
| 14   | AC1514 | The right glue image search for Mark points is abnormal!     | 1001       | 2001         | 6          | 右点胶图像搜索Mark点异常！         |
| 15   | AC1515 | Dot tin Z is not in the pre hold position                    | 1001       | 2001         | 6          | 点锡Z不在预停留位                  |
| 16   | AC1516 | Right dispensing X failed to return to the original point!   | 1001       | 2001         | 6          | 右点胶X回原点失败！                |
| 17   | AC1517 | Right dispensing Y failed to return to the original point!   | 1001       | 2001         | 6          | 右点胶Y回原点失败！                |
| 18   | AC1518 | Right dispensing Z return to origin failed!                  | 1001       | 2001         | 6          | 右点胶Z回原点失败！                |
| 19   | AC1519 | The workstation is automatically running;please stop before operating! | 1001       | 2001         | 6          | 工位自动运行中，请停止后在操作！   |
| 20   | AC1520 | Please initialize before proceeding!                         | 1001       | 2001         | 6          | 请初始化后在操作！                 |
| 21   | AC1521 | Please stop before proceeding!                               | 1001       | 2001         | 6          | 请停止后在操作！                   |
| 22   | AC1522 | Please select a coordinate point!                            | 1001       | 2001         | 6          | 请选择坐标点！                     |
| 23   | AC1523 | Tin point Z is not in place                                  | 1001       | 2001         | 6          | 点锡Z不在原位                      |
| 24   | AC1524 | Soldering line B search timeout!                             | 1001       | 2001         | 6          | 焊线B搜索超时！                    |
| 25   | AC1525 | Glue dispensing Z is not in place                            | 1001       | 2001         | 6          | 点胶Z不在原位                      |
| 26   | AC1526 | Right dispensing Z is not in the safe position!              | 1001       | 2001         | 6          | 右点胶Z不在安全位！                |
| 27   | AC1527 | Right dispensing height measurement failed!                  | 1001       | 2001         | 6          | 右点胶测高失败！                   |
| 28   | AC1528 | Right dispensing Z not in place                              | 1001       | 2001         | 6          | 右点胶Z不在原位                    |
| 29   | AC1529 | The right glue dispensing height measurement signal is abnormal! | 1001       | 2001         | 6          | 右点胶测高信号异常！               |
| 30   | AC1530 | Right pre dispensing height measurement failed!              | 1001       | 2001         | 6          | 右预点胶测高失败！                 |
| 31   | AC1531 | Please initialize the right workstation before starting!     | 1001       | 2001         | 6          | 右工位请初始化后再启动！           |
| 32   | AC1532 | Right dispensing controller parameter write failure          | 1001       | 2001         | 6          | 右点胶控制器参数写入失败           |
| 33   | AC1533 | XY has moved to the starting point!                          | 1001       | 2001         | 6          | XY已移到起点！                     |
| 34   | AC1534 | XY has moved to the endpoint!                                | 1001       | 2001         | 6          | XY已移到终点！                     |
| 35   | AC1535 | Connecting Dispensing Controller Serial port open failed!    | 1001       | 2001         | 6          | 连接点胶控制器 串口打开失败！      |



```sh
9501=AC1501,The melting speed of the welding line exceeds the maximum value:,The melting speed of the welding line exceeds the maximum value:,1001,2001,6,
9502=AC1502,Failed to update the data of solder wire B!,Failed to update the data of solder wire B!,1001,2001,6,
9503=AC1503,No frame information read!,No frame information read!,1001,2001,6,
9504=AC1504,The number of tin point positions exceeds the upper limit of 60 coordinate points!,The number of tin point positions exceeds the upper limit of 60 coordinate points!,1001,2001,6,
9505=AC1505,The dispensing position exceeds the upper limit by 20 points,The dispensing position exceeds the upper limit by 20 points,1001,2001,6,
9506=AC1506,Failed to read framework data!,Failed to read framework data!,1001,2001,6,
9507=AC1507,Frame Pad bit exceeds the upper limit of 690,Frame Pad bit exceeds the upper limit of 690,1001,2001,6,
9508=AC1508,Drawtin B data write failure,Drawtin B data write failure,1001,2001,6,
9509=AC1509,Abnormal detection signal of welding line B,Abnormal detection signal of welding line B,1001,2001,6,
9510=AC1510,Welding line B detection timeout,Welding line B detection timeout,1001,2001,6,
9511=AC1511,Left dispensing detection abnormal!,Left dispensing detection abnormal!,1001,2001,6,
9512=AC1512,Abnormal right dispensing detection!,Abnormal right dispensing detection!,1001,2001,6,
9513=AC1513,The right glue dispensing camera is disconnected!,The right glue dispensing camera is disconnected!,1001,2001,6,
9514=AC1514,The right glue image search for Mark points is abnormal!,The right glue image search for Mark points is abnormal!,1001,2001,6,
9515=AC1515,Dot tin Z is not in the pre hold position,Dot tin Z is not in the pre hold position,1001,2001,6,
9516=AC1516,Right dispensing X failed to return to the original point!,Right dispensing X failed to return to the original point!,1001,2001,6,
9517=AC1517,Right dispensing Y failed to return to the original point!,Right dispensing Y failed to return to the original point!,1001,2001,6,
9518=AC1518,Right dispensing Z return to origin failed!,Right dispensing Z return to origin failed!,1001,2001,6,
9519=AC1519,The workstation is automatically running;please stop before operating!,The workstation is automatically running;please stop before operating!,1001,2001,6,
9520=AC1520,Please initialize before proceeding!,Please initialize before proceeding!,1001,2001,6,
9521=AC1521,Please stop before proceeding!,Please stop before proceeding!,1001,2001,6,
9522=AC1522,Please select a coordinate point!,Please select a coordinate point!,1001,2001,6,
9523=AC1523,Tin point Z is not in place,Tin point Z is not in place,1001,2001,6,
9524=AC1524,Soldering line B search timeout!,Soldering line B search timeout!,1001,2001,6,
9525=AC1525,Glue dispensing Z is not in place,Glue dispensing Z is not in place,1001,2001,6,
9526=AC1526,Right dispensing Z is not in the safe position!,Right dispensing Z is not in the safe position!,1001,2001,6,
9527=AC1527,Right dispensing height measurement failed!,Right dispensing height measurement failed!,1001,2001,6,
9528=AC1528,Right dispensing Z not in place,Right dispensing Z not in place,1001,2001,6,
9529=AC1529,The right glue dispensing height measurement signal is abnormal!,The right glue dispensing height measurement signal is abnormal!,1001,2001,6,
9530=AC1530,Right pre dispensing height measurement failed!,Right pre dispensing height measurement failed!,1001,2001,6,
9531=AC1531,Please initialize the right workstation before starting!,Please initialize the right workstation before starting!,1001,2001,6,
9532=AC1532,Right dispensing controller parameter write failure,Right dispensing controller parameter write failure,1001,2001,6,
9533=AC1533,XY has moved to the starting point!,XY has moved to the starting point!,1001,2001,6,
9534=AC1534,XY has moved to the endpoint!,XY has moved to the endpoint!,1001,2001,6,
9535=AC1535,Connecting Dispensing Controller Serial port open failed!,Connecting Dispensing Controller Serial port open failed!,1001,2001,6,

```