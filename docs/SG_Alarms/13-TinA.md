# 13-TinA die bonding alarm code

| ID   | Name   | description                                           | setEventID | clearEventID | alarm code | Text                                                   |
| ---- | ------ | ----------------------------------------------------- | ---------- | ------------ | ---------- | ------------------------------------------------------ |
| 1    | AC1301 | 未读取到框架信息！                                   | 1001       | 2001         | 6          | No frame information read!                             |
| 2    | AC1302 | 点锡位置的数量超出上限60个坐标点！                  | 1001       | 2001         | 6          | The number of tin point positions exceeds the upper limit of 60 coordinate points! |
| 3    | AC1303 | 点胶位超出上限20个点位                             | 1001       | 2001         | 6          | The dispensing position exceeds the upper limit by 20 points |
| 4    | AC1304 | 框架数据读取失败！                                   | 1001       | 2001         | 6          | Failed to read framework data!                         |
| 5    | AC1305 | 框架Pad位超出上限690                               | 1001       | 2001         | 6          | Frame Pad bit exceeds the upper limit of 690           |
| 6    | AC1306 | 画锡A数据写入失败                                    | 1001       | 2001         | 6          | Failed to write data for drawing tin A                 |
| 7    | AC1307 | 焊线A探测信号异常                                   | 1001       | 2001         | 6          | Abnormal detection signal of welding line A            |
| 8    | AC1308 | 焊线A探测超时                                       | 1001       | 2001         | 6          | Welding line A detection timeout                       |
| 9    | AC1309 | 预点胶位置满！                                       | 1001       | 2001         | 6          | Left dispensing detection abnormal!                    |
| 10   | AC1310 | 左点胶检测异常！                                     | 1001       | 2001         | 6          | Left dispensing detection abnormal!                    |
| 11   | AC1311 | 左点胶相机掉线！                                     | 1001       | 2001         | 6          | The left dispensing camera is disconnected!           |
| 12   | AC1312 | 左点胶图像搜索Mark点异常！                          | 1001       | 2001         | 6          | Left glue image search Mark point exception!           |
| 13   | AC1313 | 点锡Z不在预停留位                                  | 1001       | 2001         | 6          | Dot tin Z is not in the pre hold position             |
| 14   | AC1314 | 左点胶X回原点失败！                                 | 1001       | 2001         | 6          | Left dispensing X failed to return to the original point! |
| 15   | AC1315 | 左点胶Y回原点失败！                                 | 1001       | 2001         | 6          | Left dispensing Y failed to return to the original point! |
| 16   | AC1316 | 工位自动运行中&请停止后在操作！                   | 1001       | 2001         | 6          | The workstation is automatically running& please stop before operating! |
| 17   | AC1317 | 左点胶Z回原点失败！                                 | 1001       | 2001         | 6          | Left dispensing Z return to origin failed!             |
| 18   | AC1318 | 请初始化后在操作！                                   | 1001       | 2001         | 6          | Please initialize before proceeding!                   |
| 19   | AC1319 | 请停止后在操作！                                     | 1001       | 2001         | 6          | Please stop before proceeding!                         |
| 20   | AC1320 | 请选择坐标点！                                       | 1001       | 2001         | 6          | Please select a coordinate point!                      |
| 21   | AC1321 | 点锡Z不在原位                                        | 1001       | 2001         | 6          | Tin point Z is not in place                            |
| 22   | AC1322 | 焊线A搜索超时！                                     | 1001       | 2001         | 6          | Soldering line A search timeout!                       |
| 23   | AC1323 | 点胶Z不在原位                                        | 1001       | 2001         | 6          | Glue dispensing Z is not in place                      |
| 24   | AC1324 | 左点胶Z不在安全位！                                 | 1001       | 2001         | 6          | Left dispensing Z is not in the safe position!         |
| 25   | AC1325 | XY已移到起点！                                      | 1001       | 2001         | 6          | XY has moved to the starting point!                    |
| 26   | AC1326 | 左点胶测高失败！                                    | 1001       | 2001         | 6          | Left dispensing height measurement failed!             |
| 27   | AC1327 | 左点胶Z不在原位                                      | 1001       | 2001         | 6          | Left dispensing Z not in place                         |
| 28   | AC1328 | 左点胶测高信号异常！                                | 1001       | 2001         | 6          | Left glue dispensing height measurement signal abnormal! |
| 29   | AC1329 | 左预点胶测高失败！                                  | 1001       | 2001         | 6          | Left pre dispensing height measurement failed!         |
| 30   | AC1330 | 左工位请初始化后再启动！                            | 1001       | 2001         | 6          | Please initialize the left workstation before starting! |
| 31   | AC1331 | 更新送焊线A数据失败！                               | 1001       | 2001         | 6          | Failed to update welding line A data!                  |
| 32   | AC1332 | 左点胶控制器参数写入失败                             | 1001       | 2001         | 6          | Left dispensing Z not in place                         |
| 33   | AC1333 | XY已移到终点！                                      | 1001       | 2001         | 6          | XY has moved to the endpoint!                          |
| 34   | AC1334 | 焊线熔化速度超出最大值:                            | 1001       | 2001         | 6          | The melting speed of the welding line exceeds the maximum value: |



```sh
9301=AC1301,No frame information read!,No frame information read!,1001,2001,6,
9302=AC1302,The number of tin point positions exceeds the upper limit of 60 coordinate points!,The number of tin point positions exceeds the upper limit of 60 coordinate points!,1001,2001,6,
9303=AC1303,The dispensing position exceeds the upper limit by 20 points,The dispensing position exceeds the upper limit by 20 points,1001,2001,6,
9304=AC1304,Failed to read framework data!,Failed to read framework data!,1001,2001,6,
9305=AC1305,Frame Pad bit exceeds the upper limit of 690,Frame Pad bit exceeds the upper limit of 690,1001,2001,6,
9306=AC1306,Failed to write data for drawing tin A,Failed to write data for drawing tin A,1001,2001,6,
9307=AC1307,Abnormal detection signal of welding line A,Abnormal detection signal of welding line A,1001,2001,6,
9308=AC1308,Welding line A detection timeout,Welding line A detection timeout,1001,2001,6,
9309=AC1309,Left dispensing detection abnormal!,Left dispensing detection abnormal!,1001,2001,6,
9310=AC1310,Left dispensing detection abnormal!,Left dispensing detection abnormal!,1001,2001,6,
9311=AC1311,The left dispensing camera is disconnected!,The left dispensing camera is disconnected!,1001,2001,6,
9312=AC1312,Left glue image search Mark point exception!,Left glue image search Mark point exception!,1001,2001,6,
9313=AC1313,Dot tin Z is not in the pre hold position,Dot tin Z is not in the pre hold position,1001,2001,6,
9314=AC1314,Left dispensing X failed to return to the original point!,Left dispensing X failed to return to the original point!,1001,2001,6,
9315=AC1315,Left dispensing Y failed to return to the original point!,Left dispensing Y failed to return to the original point!,1001,2001,6,
9316=AC1316,The workstation is automatically running& please stop before operating!,The workstation is automatically running& please stop before operating!,1001,2001,6,
9317=AC1317,Left dispensing Z return to origin failed!,Left dispensing Z return to origin failed!,1001,2001,6,
9318=AC1318,Please initialize before proceeding!,Please initialize before proceeding!,1001,2001,6,
9319=AC1319,Please stop before proceeding!,Please stop before proceeding!,1001,2001,6,
9320=AC1320,Please select a coordinate point!,Please select a coordinate point!,1001,2001,6,
9321=AC1321,Tin point Z is not in place,Tin point Z is not in place,1001,2001,6,
9322=AC1322,Soldering line A search timeout!,Soldering line A search timeout!,1001,2001,6,
9323=AC1323,Glue dispensing Z is not in place,Glue dispensing Z is not in place,1001,2001,6,
9324=AC1324,Left dispensing Z is not in the safe position!,Left dispensing Z is not in the safe position!,1001,2001,6,
9325=AC1325,XY has moved to the starting point!,XY has moved to the starting point!,1001,2001,6,
9326=AC1326,Left dispensing height measurement failed!,Left dispensing height measurement failed!,1001,2001,6,
9327=AC1327,Left dispensing Z not in place,Left dispensing Z not in place,1001,2001,6,
9328=AC1328,Left glue dispensing height measurement signal abnormal!,Left glue dispensing height measurement signal abnormal!,1001,2001,6,
9329=AC1329,Left pre dispensing height measurement failed!,Left pre dispensing height measurement failed!,1001,2001,6,
9330=AC1330,Please initialize the left workstation before starting!,Please initialize the left workstation before starting!,1001,2001,6,
9331=AC1331,Failed to update welding line A data!,Failed to update welding line A data!,1001,2001,6,
9332=AC1332,Left dispensing Z not in place,Left dispensing Z not in place,1001,2001,6,
9333=AC1333,XY has moved to the endpoint!,XY has moved to the endpoint!,1001,2001,6,
9334=AC1334,The melting speed of the welding line exceeds the maximum value:,The melting speed of the welding line exceeds the maximum value:,1001,2001,6,
```