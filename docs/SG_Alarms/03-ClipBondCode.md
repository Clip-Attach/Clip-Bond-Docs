# 03-ClipBondCode die bonding alarm code(OK)


| ID   | Name   | Description                                                  | setEventID | clearEventID | alarm code | Text                                 |
| ---- | ------ | ------------------------------------------------------------ | ---------- | ------------ | ---------- | ------------------------------------ |
| 1    | AC0301 | The P&P Buffer exited abnormally!                            | 1001       | 2001         | 6          | 绑头Buffer异常退出！                 |
| 2    | AC0302 | Abnormal nozzle detection!                                   | 1001       | 2001         | 6          | 吸嘴检测异常！                       |
| 3    | AC0303 | The suction nozzle detects the camera timeout!               | 1001       | 2001         | 6          | 吸嘴检测相机超时！                   |
| 4    | AC0304 | The P&P Buffer receives a pause command!                     | 1001       | 2001         | 6          | 绑头Buffer收到暂停命令！             |
| 5    | AC0305 | Waiting for the camera to detect the axis timeout!           | 1001       | 2001         | 6          | 等待相机检测轴超时！                 |
| 6    | AC0306 | Clip pickup force detection anomaly!                         | 1001       | 2001         | 6          | Clip拾取力探测异常！                 |
| 7    | AC0307 | Clip weld force detection anomaly!                           | 1001       | 2001         | 6          | Clip焊接力探测异常！                 |
| 8    | AC0308 | P&P contact detection is abnormal!                           | 1001       | 2001         | 6          | 焊头触点检测异常！                   |
| 9    | AC0309 | The number of times the cutter has been used has reached its limit! | 1001       | 2001         | 6          | 切刀使用次数已到上限！               |
| 10   | AC0310 | Solid ClipPR Buffer exited abnormally!                       | 1001       | 2001         | 6          | 固ClipPR Buffer异常退出！            |
| 11   | AC0311 | The P&P Buffer receives a pause command!                     | 1001       | 2001         | 6          | 绑头Buffer收到暂停命令！             |
| 12   | AC0312 | Waiting for P&P Y to move to the safe bit timeout!           | 1001       | 2001         | 6          | 等待绑头Y移动到安全位超时！          |
| 13   | AC0313 | P&P detects camera timeout!                                  | 1001       | 2001         | 6          | 焊头检测相机超时！                   |
| 14   | AC0314 | P&P framework positioning anomaly!                           | 1001       | 2001         | 6          | 焊头框架定位异常！                   |
| 15   | AC0315 | P&P frame glue spot detection abnormality!                   | 1001       | 2001         | 6          | 焊头框架胶点检测异常！               |
| 16   | AC0316 | P&P Framework Clip Detection Exception!                      | 1001       | 2001         | 6          | 焊头框架Clip检测异常！               |
| 17   | AC0317 | P&P Buffer exit timeout!                                     | 1001       | 2001         | 6          | 绑头Buffer退出超时！                 |
| 18   | AC0318 | Solid ClipPR Buffer exit timeout!                            | 1001       | 2001         | 6          | 固ClipPR Buffer退出超时！            |
| 19   | AC0319 | P&P Z is not in a safe position!                             | 1001       | 2001         | 6          | 绑头Z不在安全位！                    |
| 20   | AC0320 | Wait for the strip positioning timeout!                      | 1001       | 2001         | 6          | 等待条带定位超时！                   |
| 21   | AC0321 | The suction nozzle detects the camera timeout!               | 1001       | 2001         | 6          | 吸嘴检测相机超时！                   |
| 22   | AC0322 | Abnormal nozzle detection!                                   | 1001       | 2001         | 6          | 吸嘴检测异常！                       |
| 23   | AC0323 | Please stop and then operate!                                | 1001       | 2001         | 6          | 请停止后在操作！                     |
| 24   | AC0324 | Please initialize it before operation!                       | 1001       | 2001         | 6          | 请初始化后再操作！                   |
| 25   | AC0325 | P&P X back to the origin failed!                             | 1001       | 2001         | 6          | 绑头X回原点失败！                    |
| 26   | AC0326 | P&P Y back to the origin failed!                             | 1001       | 2001         | 6          | 绑头Y回原点失败！                    |
| 27   | AC0327 | P&P Z back to the origin failed!                             | 1001       | 2001         | 6          | 绑头Z回原点失败！                    |
| 28   | AC0328 | Camera axis return to home position failed!                  | 1001       | 2001         | 6          | 相机轴回原点失败！                   |
| 29   | AC0329 | The P&P station is running automatically;please stop before operating! | 1001       | 2001         | 6          | 绑头工位自动运行中，请停止后在操作！ |
| 30   | AC0330 | Cutter return to home position failed!                       | 1001       | 2001         | 6          | 切刀回原点失败！                     |
| 31   | AC0331 | P&P Rotate back to home position failed!                     | 1001       | 2001         | 6          | 焊头旋转回原点失败！                 |
| 32   | AC0332 | Camera Y Back to Home failed!                                | 1001       | 2001         | 6          | 相机Y回原点失败！                    |
| 33   | AC0333 | Solid crystal coordinates are acquired abnormally!           | 1001       | 2001         | 6          | 固晶坐标获取异常！                   |
| 35   | AC0335 | Please pick the correct coordinate point!                    | 1001       | 2001         | 6          | 请选着正确的坐标点！                 |
| 36   | AC0336 | P&P XY is not in the specified position!                     | 1001       | 2001         | 6          | 焊头XY不在指定位置！                 |
| 37   | AC0337 | The altimetry contact is abnormal!                           | 1001       | 2001         | 6          | 测高触点异常！                       |
| 38   | AC0338 | P&P Z altimetry failed!                                      | 1001       | 2001         | 6          | 绑头Z测高失败！                      |
| 39   | AC0339 | Punch-cut altimetry failed!                                  | 1001       | 2001         | 6          | 冲切测高失败！                       |
| 40   | AC0340 | Camera Y has reached the first one.                          | 1001       | 2001         | 6          | 相机Y已到达第一颗                    |
| 41   | AC0341 | Camera Y has reached the last one.                           | 1001       | 2001         | 6          | 相机Y已到达最后一颗                  |
| 42   | AC0342 | P&P Z is not in a safe position!                             | 1001       | 2001         | 6          | 焊头Z不在安全位！                    |
| 43   | AC0343 | P&P Y axis is not in the safe position!                      | 1001       | 2001         | 6          | 焊头Y轴不在安全位！                  |
| 44   | AC0344 | The camera Y-axis is not in the safe position!               | 1001       | 2001         | 6          | 相机Y轴不在安全位！                  |
| 45   | AC0345 | P&P has reached the first one.                               | 1001       | 2001         | 6          | 焊头已到达第一颗                     |
| 46   | AC0346 | P&P has reached the last one.                                | 1001       | 2001         | 6          | 焊头已到达最后一颗                   |



```sh
8301=AC0301,The P&P Buffer exited abnormally!,The P&P Buffer exited abnormally!,1001,2001,6,
8302=AC0302,Abnormal nozzle detection!,Abnormal nozzle detection!,1001,2001,6,
8303=AC0303,The suction nozzle detects the camera timeout!,The suction nozzle detects the camera timeout!,1001,2001,6,
8304=AC0304,The P&P Buffer receives a pause command!,The P&P Buffer receives a pause command!,1001,2001,6,
8305=AC0305,Waiting for the camera to detect the axis timeout!,Waiting for the camera to detect the axis timeout!,1001,2001,6,
8306=AC0306,Clip pickup force detection anomaly!,Clip pickup force detection anomaly!,1001,2001,6,
8307=AC0307,Clip weld force detection anomaly!,Clip weld force detection anomaly!,1001,2001,6,
8308=AC0308,P&P contact detection is abnormal!,P&P contact detection is abnormal!,1001,2001,6,
8309=AC0309,The number of times the cutter has been used has reached its limit!,The number of times the cutter has been used has reached its limit!,1001,2001,6,
8310=AC0310,Solid ClipPR Buffer exited abnormally!,Solid ClipPR Buffer exited abnormally!,1001,2001,6,
8311=AC0311,The P&P Buffer receives a pause command!,The P&P Buffer receives a pause command!,1001,2001,6,
8312=AC0312,Waiting for P&P Y to move to the safe bit timeout!,Waiting for P&P Y to move to the safe bit timeout!,1001,2001,6,
8313=AC0313,P&P detects camera timeout!,P&P detects camera timeout!,1001,2001,6,
8314=AC0314,P&P framework positioning anomaly!,P&P framework positioning anomaly!,1001,2001,6,
8315=AC0315,P&P frame glue spot detection abnormality!,P&P frame glue spot detection abnormality!,1001,2001,6,
8316=AC0316,P&P Framework Clip Detection Exception!,P&P Framework Clip Detection Exception!,1001,2001,6,
8317=AC0317,P&P Buffer exit timeout!,P&P Buffer exit timeout!,1001,2001,6,
8318=AC0318,Solid ClipPR Buffer exit timeout!,Solid ClipPR Buffer exit timeout!,1001,2001,6,
8319=AC0319,P&P Z is not in a safe position!,P&P Z is not in a safe position!,1001,2001,6,
8320=AC0320,Wait for the strip positioning timeout!,Wait for the strip positioning timeout!,1001,2001,6,
8321=AC0321,The suction nozzle detects the camera timeout!,The suction nozzle detects the camera timeout!,1001,2001,6,
8322=AC0322,Abnormal nozzle detection!,Abnormal nozzle detection!,1001,2001,6,
8323=AC0323,Please stop and then operate!,Please stop and then operate!,1001,2001,6,
8324=AC0324,Please initialize it before operation!,Please initialize it before operation!,1001,2001,6,
8325=AC0325,P&P X back to the origin failed!,P&P X back to the origin failed!,1001,2001,6,
8326=AC0326,P&P Y back to the origin failed!,P&P Y back to the origin failed!,1001,2001,6,
8327=AC0327,P&P Z back to the origin failed!,P&P Z back to the origin failed!,1001,2001,6,
8328=AC0328,Camera axis return to home position failed!,Camera axis return to home position failed!,1001,2001,6,
8329=AC0329,The P&P station is running automatically;please stop before operating!,The P&P station is running automatically;please stop before operating!,1001,2001,6,
8330=AC0330,Cutter return to home position failed!,Cutter return to home position failed!,1001,2001,6,
8331=AC0331,P&P Rotate back to home position failed!,P&P Rotate back to home position failed!,1001,2001,6,
8332=AC0332,Camera Y Back to Home failed!,Camera Y Back to Home failed!,1001,2001,6,
8333=AC0333,Solid crystal coordinates are acquired abnormally!,Solid crystal coordinates are acquired abnormally!,1001,2001,6,
8335=AC0335,Please pick the correct coordinate point!,Please pick the correct coordinate point!,1001,2001,6,
8336=AC0336,P&P XY is not in the specified position!,P&P XY is not in the specified position!,1001,2001,6,
8337=AC0337,The altimetry contact is abnormal!,The altimetry contact is abnormal!,1001,2001,6,
8338=AC0338,P&P Z altimetry failed!,P&P Z altimetry failed!,1001,2001,6,
8339=AC0339,Punch-cut altimetry failed!,Punch-cut altimetry failed!,1001,2001,6,
8340=AC0340,Camera Y has reached the first one.,Camera Y has reached the first one.,1001,2001,6,
8341=AC0341,Camera Y has reached the last one.,Camera Y has reached the last one.,1001,2001,6,
8342=AC0342,P&P Z is not in a safe position!,P&P Z is not in a safe position!,1001,2001,6,
8343=AC0343,P&P Y axis is not in the safe position!,P&P Y axis is not in the safe position!,1001,2001,6,
8344=AC0344,The camera Y-axis is not in the safe position!,The camera Y-axis is not in the safe position!,1001,2001,6,
8345=AC0345,P&P has reached the first one.,P&P has reached the first one.,1001,2001,6,
8346=AC0346,P&P has reached the last one.,P&P has reached the last one.,1001,2001,6,

```