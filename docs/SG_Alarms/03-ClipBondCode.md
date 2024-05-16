# 03-ClipBondCode die bonding alarm code

| ID   | Name    | Description                                                 | setEventID | clearEventID | alarm code | Text                                    |
| ---- | ------- | ------------------------------------------------------------ | ---------- | ------------ | ---------- | --------------------------------------- |
| 1    | AC0301  | Abnormal position of binding head Z!                         | 1001       | 2001         | 6          | 绑头Z位置异常！                         |
| 2    | AC0302  | Abnormal position of binding head Y!                         | 1001       | 2001         | 6          | 绑头Y位置异常！                         |
| 3    | AC0303  | Binding buffer exited abnormally!                            | 1001       | 2001         | 6          | 绑头Buffer异常退出！                    |
| 4    | AC0304  | Abnormal leak detection of suction nozzle!                   | 1001       | 2001         | 6          | 吸嘴检漏异常！                          |
| 5    | AC0305  | Abnormal blockage of suction nozzle!                         | 1001       | 2001         | 6          | 吸嘴堵塞异常！                          |
| 6    | AC0306  | Binding buffer received pause command!                       | 1001       | 2001         | 6          | 绑头Buffer收到暂停命令！                |
| 7    | AC0307  | The binding force encoder reading is abnormal!               | 1001       | 2001         | 6          | 绑头Force编码器读数异常！               |
| 8    | AC0308  | The number of times the suction nozzle has been used has reached the maximum limit! | 1001       | 2001         | 6          | 吸嘴使用次数已到上限！                  |
| 9    | AC0309  | The number of times the thimble has been used has reached the maximum limit! | 1001       | 2001         | 6          | 顶针使用次数已到上限！                  |
| 10   | AC0310  | The production capacity has reached the upper limit!         | 1001       | 2001         | 6          | 产能已到上限！                          |
| 11   | AC0311  | Camera Y Buffer exited abnormally!                           | 1001       | 2001         | 6          | 相机Y Buffer异常退出！                  |
| 13   | AC0313  | Abnormal PR detection after solidification!                  | 1001       | 2001         | 6          | 固晶后PR检测异常！                      |
| 14   | AC0314  | Solid crystal detection camera timeout!                      | 1001       | 2001         | 6          | 固晶检测相机超时！                      |
| 15   | AC0315  | Abnormal framework positioning PR detection!                 | 1001       | 2001         | 6          | 框架定位PR检测异常！                    |
| 16   | AC0316  | Abnormal glue point PR detection!                            | 1001       | 2001         | 6          | 胶点PR检测异常！                        |
| 17   | AC0317  | Binding buffer exit timeout!                                 | 1001       | 2001         | 6          | 绑头Buffer退出超时！                    |
| 18   | AC0318  | Abnormal position of binding head Z!                         | 1001       | 2001         | 6          | 绑头Z位置异常！                         |
| 19   | AC0319  | Camera Y Buffer exit timeout!                                | 1001       | 2001         | 6          | 相机Y Buffer退出超时！                  |
| 20   | AC0320  | Waiting for chip positioning timeout!                        | 1001       | 2001         | 6          | 等待晶片定位超时！                      |
| 21   | AC0321  | There are grains detected on the suction nozzle!             | 1001       | 2001         | 6          | 吸嘴上检测有晶粒！                      |
| 24   | AC0324  | Binding head X back to origin failed!                        | 1001       | 2001         | 6          | 绑头X回原点失败！                       |
| 25   | AC0325  | Binding head Y back to origin failed!                        | 1001       | 2001         | 6          | 绑头Y回原点失败！                       |
| 26   | AC0326  | Binding head Z back to origin failed!                        | 1001       | 2001         | 6          | 绑头Z回原点失败！                       |
| 27   | AC0327  | Camera axis return to origin failed!                         | 1001       | 2001         | 6          | 相机轴回原点失败！                      |
| 28   | AC0328  | Welding head rotation back to origin failed!                 | 1001       | 2001         | 6          | 焊头旋转回原点失败！                    |
| 29   | AC0329  | The binding station is automatically running& please stop before operating! | 1001       | 2001         | 6          | 绑头工位自动运行中&请停止后在操作！   |
| 30   | AC0330  | Cutter return to origin failed!                              | 1001       | 2001         | 6          | 切刀回原点失败！                        |
| 31   | AC0331  | Please stop before proceeding!                               | 1001       | 2001         | 6          | 请停止后在操作！                        |
| 32   | AC0332  | Please initialize before proceeding!                         | 1001       | 2001         | 6          | 请初始化后在操作！                      |
| 33   | AC0333  | The distance between the binding head suction nozzle hole and the image center Y is greater than 5mm! | 1001       | 2001         | 6          | 绑头吸嘴孔与图像中心Y距离大于5mm！    |
| 34   | AC0334  | The distance between the binding head suction nozzle hole and the image center X is greater than 5mm! | 1001       | 2001         | 6          | 绑头吸嘴孔与图像中心X距离大于5mm！    |
| 35   | AC0335  | Welding head Z is not in safe position!                      | 1001       | 2001         | 6          | 焊头Z不在安全位！                      |
| 36   | AC0336  | Abnormal acquisition of solid crystal coordinates!           | 1001       | 2001         | 6          | 固晶坐标获取异常！                      |
| 37   | AC0337  | Please select the correct coordinate point!                  | 1001       | 2001         | 6          | 请选着正确的坐标点！                    |
| 38   | AC0338  | Welding head XY is not in the specified position!            | 1001       | 2001         | 6          | 焊头XY不在指定位置！                    |
| 39   | AC0339  | Head binding Z height measurement failed!                    | 1001       | 2001         | 6          | 绑头Z测高失败！                        |
| 40   | AC0340  | Punching height measurement failed!                          | 1001       | 2001         | 6          | 冲切测高失败！                          |
| 41   | AC0341  | Abnormality of height measurement encoder!                   | 1001       | 2001         | 6          | 测高编码器异常！                        |
| 42   | AC0342  | The welding head has reached the last one                    | 1001       | 2001         | 6          | 焊头已到达最后一颗                    |
| 43   | AC0343  | The welding head has reached the first one                   | 1001       | 2001         | 6          | 焊头已到达第一颗                      |
| 44   | AC0344  | Camera Y has reached the last one                            | 1001       | 2001         | 6          | 相机Y已到达最后一颗                   |
| 45   | AC0345  | Camera Y has reached the first one                           | 1001       | 2001         | 6          | 相机Y已到达第一颗                     |



```sh
8301=AC0301,Abnormal position of binding head Z!,Abnormal position of binding head Z!,1001,2001,6,
8302=AC0302,Abnormal position of binding head Y!,Abnormal position of binding head Y!,1001,2001,6,
8303=AC0303,Binding buffer exited abnormally!,Binding buffer exited abnormally!,1001,2001,6,
8304=AC0304,Abnormal leak detection of suction nozzle!,Abnormal leak detection of suction nozzle!,1001,2001,6,
8305=AC0305,Abnormal blockage of suction nozzle!,Abnormal blockage of suction nozzle!,1001,2001,6,
8306=AC0306,Binding buffer received pause command!,Binding buffer received pause command!,1001,2001,6,
8307=AC0307,The binding force encoder reading is abnormal!,The binding force encoder reading is abnormal!,1001,2001,6,
8308=AC0308,The number of times the suction nozzle has been used has reached the maximum limit!,The number of times the suction nozzle has been used has reached the maximum limit!,1001,2001,6,
8309=AC0309,The number of times the thimble has been used has reached the maximum limit!,The number of times the thimble has been used has reached the maximum limit!,1001,2001,6,
8310=AC0310,The production capacity has reached the upper limit!,The production capacity has reached the upper limit!,1001,2001,6,
8311=AC0311,Camera Y Buffer exited abnormally!,Camera Y Buffer exited abnormally!,1001,2001,6,
8313=AC0313,Abnormal PR detection after solidification!,Abnormal PR detection after solidification!,1001,2001,6,
8314=AC0314,Solid crystal detection camera timeout!,Solid crystal detection camera timeout!,1001,2001,6,
8315=AC0315,Abnormal framework positioning PR detection!,Abnormal framework positioning PR detection!,1001,2001,6,
8316=AC0316,Abnormal glue point PR detection!,Abnormal glue point PR detection!,1001,2001,6,
8317=AC0317,Binding buffer exit timeout!,Binding buffer exit timeout!,1001,2001,6,
8318=AC0318,Abnormal position of binding head Z!,Abnormal position of binding head Z!,1001,2001,6,
8319=AC0319,Camera Y Buffer exit timeout!,Camera Y Buffer exit timeout!,1001,2001,6,
8320=AC0320,Waiting for chip positioning timeout!,Waiting for chip positioning timeout!,1001,2001,6,
8321=AC0321,There are grains detected on the suction nozzle!,There are grains detected on the suction nozzle!,1001,2001,6,
8324=AC0324,Binding head X back to origin failed!,Binding head X back to origin failed!,1001,2001,6,
8325=AC0325,Binding head Y back to origin failed!,Binding head Y back to origin failed!,1001,2001,6,
8326=AC0326,Binding head Z back to origin failed!,Binding head Z back to origin failed!,1001,2001,6,
8327=AC0327,Camera axis return to origin failed!,Camera axis return to origin failed!,1001,2001,6,
8328=AC0328,Welding head rotation back to origin failed!,Welding head rotation back to origin failed!,1001,2001,6,
8329=AC0329,The binding station is automatically running& please stop before operating!,The binding station is automatically running& please stop before operating!,1001,2001,6,
8330=AC0330,Cutter return to origin failed!,Cutter return to origin failed!,1001,2001,6,
8331=AC0331,Please stop before proceeding!,Please stop before proceeding!,1001,2001,6,
8332=AC0332,Please initialize before proceeding!,Please initialize before proceeding!,1001,2001,6,
8333=AC0333,The distance between the binding head suction nozzle hole and the image center Y is greater than 5mm!,The distance between the binding head suction nozzle hole and the image center Y is greater than 5mm!,1001,2001,6,
8334=AC0334,The distance between the binding head suction nozzle hole and the image center X is greater than 5mm!,The distance between the binding head suction nozzle hole and the image center X is greater than 5mm!,1001,2001,6,
8335=AC0335,Welding head Z is not in safe position!,Welding head Z is not in safe position!,1001,2001,6,
8336=AC0336,Abnormal acquisition of solid crystal coordinates!,Abnormal acquisition of solid crystal coordinates!,1001,2001,6,
8337=AC0337,Please select the correct coordinate point!,Please select the correct coordinate point!,1001,2001,6,
8338=AC0338,Welding head XY is not in the specified position!,Welding head XY is not in the specified position!,1001,2001,6,
8339=AC0339,Head binding Z height measurement failed!,Head binding Z height measurement failed!,1001,2001,6,
8340=AC0340,Punching height measurement failed!,Punching height measurement failed!,1001,2001,6,
8341=AC0341,Abnormality of height measurement encoder!,Abnormality of height measurement encoder!,1001,2001,6,
8342=AC0342,The welding head has reached the last one,The welding head has reached the last one,1001,2001,6,
8343=AC0343,The welding head has reached the first one,The welding head has reached the first one,1001,2001,6,
8344=AC0344,Camera Y has reached the last one,Camera Y has reached the last one,1001,2001,6,
8345=AC0345,Camera Y has reached the first one,Camera Y has reached the first one,1001,2001,6,
```