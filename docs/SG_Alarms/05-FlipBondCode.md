# 05-FlipBondCode die bonding alarm code

| ID   | Name    | Description                                                 | setEventID | clearEventID | alarm code | Text                                    |
| ---- | ------- | ------------------------------------------------------------ | ---------- | ------------ | ---------- | --------------------------------------- |
| 1    | AC0501  | The Flip Buffer exits unexpectedly. Procedure!               | 1001       | 2001         | 6          | Flip Buffer异常退出！                |
| 2    | AC0502  | Flip detects camera timeouts!                                | 1001       | 2001         | 6          | Flip检测相机超时！                   |
| 3    | AC0503  | Flip pick grain detection anomaly!                           | 1001       | 2001         | 6          | Flip拾取晶粒检测异常！               |
| 4    | AC0504  | Weld head occluded to Flip detection camera!                 | 1001       | 2001         | 6          | 焊头遮挡到Flip检测相机！             |
| 5    | AC0505  | Flip tip detected abnormal!                                  | 1001       | 2001         | 6          | Flip吸嘴检测异常！                   |
| 6    | AC0506  | The Flip Buffer exit timed out!                              | 1001       | 2001         | 6          | Flip Buffer退出超时！                |
| 7    | AC0507  | Flip Z position is abnormal!                                 | 1001       | 2001         | 6          | Flip Z位置异常！                     |
| 8    | AC0508  | Waiting for chip positioning timeout!                        | 1001       | 2001         | 6          | 等待晶片定位超时！                   |
| 9    | AC0509  | Flip Z back to origin failed!                                | 1001       | 2001         | 6          | Flip Z回原点失败！                   |
| 10   | AC0510  | Flip T back to origin failed!                                | 1001       | 2001         | 6          | Flip T回原点失败！                   |
| 11   | AC0511  | The binding station is automatically running& please stop before operating! | 1001       | 2001         | 6          | 绑头工位自动运行中&请停止后在操作！ |
| 12   | AC0512  | Please stop before proceeding!                               | 1001       | 2001         | 6          | 请停止后在操作！                     |
| 13   | AC0513  | Please initialize before proceeding!                         | 1001       | 2001         | 6          | 请初始化后在操作！                   |
| 14   | AC0514  | Welding head Z is not in safe position!                      | 1001       | 2001         | 6          | 焊头Z不在安全位！                    |
| 15   | AC0515  | Flip Z is not in safe position!                              | 1001       | 2001         | 6          | Flip Z不在安全位！                   |
| 16   | AC0516  | Flip Z height measurement failed!                            | 1001       | 2001         | 6          | Flip Z测高失败！                     |
| 17   | AC0517  | The Ejector failed to measure altitude!                      | 1001       | 2001         | 6          | Ejector测高失败！                    |



```sh
8501=AC0501,The Flip Buffer exits unexpectedly. Procedure!,The Flip Buffer exits unexpectedly. Procedure!,1001,2001,6,
8502=AC0502,Flip detects camera timeouts!,Flip detects camera timeouts!,1001,2001,6,
8503=AC0503,Flip pick grain detection anomaly!,Flip pick grain detection anomaly!,1001,2001,6,
8504=AC0504,Weld head occluded to Flip detection camera!,Weld head occluded to Flip detection camera!,1001,2001,6,
8505=AC0505,Flip tip detected abnormal!,Flip tip detected abnormal!,1001,2001,6,
8506=AC0506,The Flip Buffer exit timed out!,The Flip Buffer exit timed out!,1001,2001,6,
8507=AC0507,Flip Z position is abnormal!,Flip Z position is abnormal!,1001,2001,6,
8508=AC0508,Waiting for chip positioning timeout!,Waiting for chip positioning timeout!,1001,2001,6,
8509=AC0509,Flip Z back to origin failed!,Flip Z back to origin failed!,1001,2001,6,
8510=AC0510,Flip T back to origin failed!,Flip T back to origin failed!,1001,2001,6,
8511=AC0511,The binding station is automatically running& please stop before operating!,The binding station is automatically running& please stop before operating!,1001,2001,6,
8512=AC0512,Please stop before proceeding!,Please stop before proceeding!,1001,2001,6,
8513=AC0513,Please initialize before proceeding!,Please initialize before proceeding!,1001,2001,6,
8514=AC0514,Welding head Z is not in safe position!,Welding head Z is not in safe position!,1001,2001,6,
8515=AC0515,Flip Z is not in safe position!,Flip Z is not in safe position!,1001,2001,6,
8516=AC0516,Flip Z height measurement failed!,Flip Z height measurement failed!,1001,2001,6,
8517=AC0517,The Ejector failed to measure altitude!,The Ejector failed to measure altitude!,1001,2001,6,
```