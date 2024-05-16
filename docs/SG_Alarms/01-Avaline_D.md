# 01-Avaline_D die bonding alarm code

| ID | Name   | description                        | setEventID | clearEventID | alarm code | Text                                                        |
|----|--------|-------------------------------------|------------|--------------|------------|-------------------------------------------------------------|
| 1  | AC0101 | 请停止设备后在操作！               | 1001       | 2001         | 6          | Please stop the device before proceeding!                  |
| 2  | AC0102 | 输入非法参数                        | 1001       | 2001         | 6          | Entering illegal parameters                                |
| 3  | AC0103 | 相机初始化失败&程序无法启动.....  | 1001       | 2001         | 6          | Camera initialization failed& program cannot start....     |
| 4  | AC0104 | 运动控制卡初始化失败&程序无法启动..... | 1001  | 2001         | 6          | The initialization of the motion control card failed& and the program cannot start.... |
| 5  | AC0105 | 链接ACS驱动器失败&程序无法启动.....  | 1001   | 2001         | 6          | Failed to link ACS drive& program cannot start....        |
| 6  | AC0106 | 门开关异常&设备暂停！                | 1001   | 2001         | 6          | Door switch abnormal& device paused!                       |
| 7  | AC0107 | 焊头Y马达温度异常&设备暂停！         | 1001   | 2001         | 6          | Abnormal temperature of welding head Y motor& equipment paused! |
| 8  | AC0108 | 请关闭门后在启动！                    | 1001   | 2001         | 6          | Please close the door before starting!                     |
| 10 | AC0110 | 启动失败&在清轨道！                  | 1001   | 2001         | 6          | Start failed& clearing the track!                          |
| 11 | AC0111 | 启动失败&请复位后再启动！            | 1001   | 2001         | 6          | Startup failed& please reset before restarting!            |
| 12 | AC0112 | 窗口已打开&无需重复打开               | 1001   | 2001         | 6          | The window is already open& there is no need to open it again |
| 13 | AC0113 | 创建PR失败&检测模块未初始化！        | 1001   | 2001         | 6          | Failed to create PR& the detection module is not initialized! |
| 14 | AC0114 | 入料Y轴不在安全位                     | 1001   | 2001         | 6          | Feed Y-axis not in safe position                           |
| 15 | AC0115 | 请先绑头初始化                        | 1001   | 2001         | 6          | Please bind the header first for initialization            |
| 16 | AC0116 | 请先条带初始化                        | 1001   | 2001         | 6          | Please initialize the stripe first                         |
| 17 | AC0117 | 请关闭门后在操作！                    | 1001   | 2001         | 6          | Please close the door before proceeding!                   |
| 18 | AC0118 | 暂停按钮按下！                        | 1001   | 2001         | 6          | Pause button pressed!                                      |
| 19 | AC0119 | 伺服电机加使能中&请稍等！            | 1001   | 2001         | 6          | Servo motor enable& please wait!                           |
| 20 | AC0120 | 复位失败！                            | 1001   | 2001         | 6          | Reset failed!                                              |
| 21 | AC0121 | 请停止后再复位！                      | 1001   | 2001         | 6          | Please stop before resetting!                              | 
| 22 | AC0122 | 请先登录                              | 1001   | 2001         | 6          | Please log in first                                        |
| 23 | AC0123 | 无权限                                | 1001   | 2001         | 6          | No permissions                                             |


```sh
8101=AC0101,Please stop the equipment before operating!,Please stop the device before proceeding!,1001,2001,6,
8102=AC0102,Entering illegal parameters,Entering illegal parameters,1001,2001,6,
8103=AC0103,Camera initialization failed& program cannot start....,Camera initialization failed& program cannot start....,1001,2001,6,
8104=AC0104,The initialization of the motion control card failed& and the program cannot start....,The initialization of the motion control card failed& and the program cannot start....,1001,2001,6,
8105=AC0105,Failed to link ACS drive& program cannot start....,Failed to link ACS drive& program cannot start....,1001,2001,6,
8106=AC0106,Door switch abnormal& device paused!,Door switch abnormal& device paused!,1001,2001,6,
8107=AC0107,Abnormal temperature of welding head Y motor& equipment paused!,Abnormal temperature of welding head Y motor& equipment paused!,1001,2001,6,
8108=AC0108,Please close the door before starting!,Please close the door before starting!,1001,2001,6,
8110=AC0110,Start failed& clearing the track!,Start failed& clearing the track!,1001,2001,6,
8111=AC0111,Startup failed& please reset before restarting!,Startup failed& please reset before restarting!,1001,2001,6,
8112=AC0112,The window is already open& there is no need to open it again,The window is already open& there is no need to open it again,1001,2001,6,
8113=AC0113,Failed to create PR& the detection module is not initialized!,Failed to create PR& the detection module is not initialized!,1001,2001,6,
8114=AC0114,Feed Y-axis not in safe position,Feed Y-axis not in safe position,1001,2001,6,
8115=AC0115,Please bind the header first for initialization,Please bind the header first for initialization,1001,2001,6,
8116=AC0116,Please initialize the stripe first,Please initialize the stripe first,1001,2001,6,
8117=AC0117,Please close the door before proceeding!,Please close the door before proceeding!,1001,2001,6,
8118=AC0118,Pause button pressed!,Pause button pressed!,1001,2001,6,
8119=AC0119,Servo motor enable& please wait!,Servo motor enable& please wait!,1001,2001,6,
8120=AC0120,Reset failed!,Reset failed!,1001,2001,6,
8121=AC0121,Please stop before resetting!,Please stop before resetting!,1001,2001,6,
8122=AC0122,Please log in first,Please log in first,1001,2001,6,
8123=AC0123,No permissions,No permissions,1001,2001,6,
```

## LimitP (71)

| ID | Name     | description        | setEventID | clearEventID | alarm code | Text                                     |
|----|----------|--------------------|-----------|--------------|-----------|-----------------------------------------|
| 1  | LimitP1  | 左点胶X正限位      | 1001      | 2001         | 6         | Left dispensing X positive limit        |
| 2  | LimitP2  | 左点胶Y正限位      | 1001      | 2001         | 6         | Left dispensing Y positive limit        |
| 3  | LimitP3  | 左点胶Z正限位      | 1001      | 2001         | 6         | Left dispensing Z positive limit        |
| 4  | LimitP4  | 入料Y轴正限位      | 1001      | 2001         | 6         | Positive limit of feeding Y-axis        |
| 5  | LimitP5  | null               | 1001      | 2001         | 6         | null                                    |
| 6  | LimitP6  | null               | 1001      | 2001         | 6         | null                                    |
| 7  | LimitP7  | null               | 1001      | 2001         | 6         | null                                    |
| 8  | LimitP8  | 手指B电机正限位    | 1001      | 2001         | 6         | Finger B motor positive limit           |
| 9  | LimitP9  | 手指C电机正限位    | 1001      | 2001         | 6         | Finger C motor positive limit           |
| 10 | LimitP10 | 手指D电机正限位    | 1001      | 2001         | 6         | Finger D motor positive limit           |
| 11 | LimitP11 | null               | 1001      | 2001         | 6         | null                                    |
| 12 | LimitP12 | null               | 1001      | 2001         | 6         | null                                    |
| 13 | LimitP13 | 右点胶X正限位      | 1001      | 2001         | 6         | Right dispensing X positive limit       |
| 14 | LimitP14 | 右点胶Y正限位      | 1001      | 2001         | 6         | Right dispensing Y positive limit       |
| 15 | LimitP15 | 右点胶Z正限位      | 1001      | 2001         | 6         | Right dispensing Z positive limit       |
| 16 | LimitP16 | null               | 1001      | 2001         | 6         | null                                    |
| 17 | LimitP17 | null               | 1001      | 2001         | 6         | null                                    |
| 18 | LimitP18 | 入料推料正限位     | 1001      | 2001         | 6         | Positive limit of feeding and pushing   |
| 19 | LimitP19 | Wafer扩片正限位    | 1001      | 2001         | 6         | Wafer expansion positive limit          |
| 20 | LimitP20 | 晶圆盘旋转正限位   | 1001      | 2001         | 6         | Positive limit of crystal disc rotation |
| 21 | LimitP21 | null               | 1001      | 2001         | 6         | null                                    |
| 22 | LimitP22 | Wafer加载料框Z正限位 | 1001    | 2001         | 6         | Wafer loading frame Z positive limit    |
| 23 | LimitP23 | null                | 1001     | 2001         | 6         | null                                    |
| 24 | LimitP24 | null                | 1001     | 2001         | 6         | null                                    |


```sh
7101=LimitP1,Left dispensing X positive limit,Left dispensing X positive limit,1001,2001,6,
7102=LimitP2,Left dispensing Y positive limit,Left dispensing Y positive limit,1001,2001,6,
7103=LimitP3,Left dispensing Z positive limit,Left dispensing Z positive limit,1001,2001,6,
7104=LimitP4,Positive limit of feeding Y-axis,Positive limit of feeding Y-axis,1001,2001,6,
7105=LimitP5,null,null,1001,2001,6,
7106=LimitP6,null,null,1001,2001,6,
7107=LimitP7,null,null,1001,2001,6,
7108=LimitP8,Finger B motor positive limit,Finger B motor positive limit,1001,2001,6,
7109=LimitP9,Finger C motor positive limit,Finger C motor positive limit,1001,2001,6,
7110=LimitP10,Finger D motor positive limit,Finger D motor positive limit,1001,2001,6,
7111=LimitP11,null,null,1001,2001,6,
7112=LimitP12,null,null,1001,2001,6,
7113=LimitP13,Right dispensing X positive limit,Right dispensing X positive limit,1001,2001,6,
7114=LimitP14,Right dispensing Y positive limit,Right dispensing Y positive limit,1001,2001,6,
7115=LimitP15,Right dispensing Z positive limit,Right dispensing Z positive limit,1001,2001,6,
7116=LimitP16,null,null,1001,2001,6,
7117=LimitP17,null,null,1001,2001,6,
7118=LimitP18,Positive limit of feeding and pushing,Positive limit of feeding and pushing,1001,2001,6,
7119=LimitP19,Wafer expansion positive limit,Wafer expansion positive limit,1001,2001,6,
7120=LimitP20,Positive limit of crystal disc rotation,Positive limit of crystal disc rotation,1001,2001,6,
7121=LimitP21,null,null,1001,2001,6,
7122=LimitP22,Wafer loading frame Z positive limit,Wafer loading frame Z positive limit,1001,2001,6,
7123=LimitP23,null,null,1001,2001,6,
7124=LimitP24,null,null,1001,2001,6,
```

## LimitN (72)

| ID | Name     | description        | setEventID | clearEventID | alarm code | Text                                      |
|----|----------|--------------------|-----------|--------------|-----------|--------------------------------------------|
| 1  | LimitN1  | 左点胶X负限位      | 1001      | 2001         | 6         | Left dispensing X negative limit           |
| 2  | LimitN2  | 左点胶Y负限位      | 1001      | 2001         | 6         | Left dispensing Y negative limit           |  
| 3  | LimitN3  | 左点胶Z负限位      | 1001      | 2001         | 6         | Left dispensing Z negative limit           |
| 4  | LimitN4  | 入料Y轴负限位      | 1001      | 2001         | 6         | Negative limit of feeding Y-axis           | 
| 5  | LimitN5  | null               | 1001      | 2001         | 6         | null                                       |
| 6  | LimitN6  | null               | 1001      | 2001         | 6         | null                                       |
| 7  | LimitN7  | null               | 1001      | 2001         | 6         | null                                       |
| 8  | LimitN8  | 手指B电机负限位    | 1001      | 2001         | 6         | Finger B motor negative limit              |
| 9  | LimitN9  | 手指C电机负限位    | 1001      | 2001         | 6         | Finger C motor negative limit              |
| 10 | LimitN10 | 手指D电机负限位    | 1001      | 2001         | 6         | Finger D motor negative limit              |
| 11 | LimitN11 | null               | 1001      | 2001         | 6         | null                                       |
| 12 | LimitN12 | null               | 1001      | 2001         | 6         | null                                       |
| 13 | LimitN13 | 右点胶X负限位      | 1001      | 2001         | 6         | Right dispensing X negative limit          |
| 14 | LimitN14 | 右点胶Y负限位      | 1001      | 2001         | 6         | Right dispensing Y negative limit          |
| 15 | LimitN15 | 右点胶Z负限位      | 1001      | 2001         | 6         | Right dispensing Z negative limit          |
| 16 | LimitN16 | null               | 1001      | 2001         | 6         | null                                       |
| 17 | LimitN17 | null               | 1001      | 2001         | 6         | null                                       |
| 18 | LimitN18 | 入料推料负限位     | 1001      | 2001         | 6         | Negative limit for feeding and pushing     |
| 19 | LimitN19 | Wafer扩片负限位    | 1001      | 2001         | 6         | Wafer expansion negative limit             |
| 20 | LimitN20 | 晶圆盘旋转负限位   | 1001      | 2001         | 6         | Negative limit of crystal disc rotation    |
| 21 | LimitN21 | null               | 1001      | 2001         | 6         | null                                       |
| 22 | LimitN22 | Wafer加载料框Z负限位 | 1001    | 2001         | 6         | Wafer loading frame Z negative limit       |
| 23 | LimitN23 | null                | 1001     | 2001         | 6         | null                                       |
| 24 | LimitN24 | null                | 1001     | 2001         | 6         | null                                       |


```sh
7201=LimitN1,Left dispensing X negative limit,Left dispensing X negative limit,1001,2001,6,
7202=LimitN2,Left dispensing Y negative limit,Left dispensing Y negative limit,1001,2001,6,
7203=LimitN3,Left dispensing Z negative limit,Left dispensing Z negative limit,1001,2001,6,
7204=LimitN4,Negative limit of feeding Y-axis,Negative limit of feeding Y-axis,1001,2001,6,
7205=LimitN5,null,null,1001,2001,6,
7206=LimitN6,null,null,1001,2001,6,
7207=LimitN7,null,null,1001,2001,6,
7208=LimitN8,Finger B motor negative limit,Finger B motor negative limit,1001,2001,6,
7209=LimitN9,Finger C motor negative limit,Finger C motor negative limit,1001,2001,6,
7210=LimitN10,Finger D motor negative limit,Finger D motor negative limit,1001,2001,6,
7211=LimitN11,null,null,1001,2001,6,
7212=LimitN12,null,null,1001,2001,6,
7213=LimitN13,Right dispensing X negative limit,Right dispensing X negative limit,1001,2001,6,
7214=LimitN14,Right dispensing Y negative limit,Right dispensing Y negative limit,1001,2001,6,
7215=LimitN15,Right dispensing Z negative limit,Right dispensing Z negative limit,1001,2001,6,
7216=LimitN16,null,null,1001,2001,6,
7217=LimitN17,null,null,1001,2001,6,
7218=LimitN18,Negative limit for feeding and pushing,Negative limit for feeding and pushing,1001,2001,6,
7219=LimitN19,Wafer expansion negative limit,Wafer expansion negative limit,1001,2001,6,
7220=LimitN20,Negative limit of crystal disc rotation,Negative limit of crystal disc rotation,1001,2001,6,
7221=LimitN21,null,null,1001,2001,6,
7222=LimitN22,Wafer loading frame Z negative limit,Wafer loading frame Z negative limit,1001,2001,6,
7223=LimitN23,null,null,1001,2001,6,
7224=LimitN24,null,null,1001,2001,6,
```


## Alm (73)

| ID | Name  | description        | setEventID | clearEventID | alarm code | Text                              |
|----|-------|--------------------|-----------|--------------|-----------|------------------------------------|
| 1  | Alm1  | 左点胶X故障        | 1001      | 2001         | 6         | Left dispensing X malfunction      |
| 2  | Alm2  | 左点胶Y故障        | 1001      | 2001         | 6         | Left dispensing Y malfunction      |
| 3  | Alm3  | 左点胶Z故障        | 1001      | 2001         | 6         | Left dispensing Z malfunction      |
| 4  | Alm4  | null               | 1001      | 2001         | 6         | null                               |
| 5  | Alm5  | null               | 1001      | 2001         | 6         | null                               |
| 6  | Alm6  | null               | 1001      | 2001         | 6         | null                               |
| 7  | Alm7  | 手指A电机故障      | 1001      | 2001         | 6         | Finger A motor malfunction        |
| 8  | Alm8  | 手指B电机故障      | 1001      | 2001         | 6         | Finger B motor malfunction        |
| 9  | Alm9  | 手指C电机故障      | 1001      | 2001         | 6         | Finger C motor malfunction        |
| 10 | Alm10 | 手指D电机故障      | 1001      | 2001         | 6         | Finger D motor malfunction        |
| 11 | Alm11 | null               | 1001      | 2001         | 6         | null                               |
| 12 | Alm12 | null               | 1001      | 2001         | 6         | null                               |
| 13 | Alm13 | 右点胶X故障        | 1001      | 2001         | 6         | Right dispensing X malfunction     |
| 14 | Alm14 | 右点胶Y故障        | 1001      | 2001         | 6         | Right dispensing Y malfunction     |
| 15 | Alm15 | 右点胶Z故障        | 1001      | 2001         | 6         | Right dispensing Z malfunction     |
| 16 | Alm16 | null               | 1001      | 2001         | 6         | null                               |
| 17 | Alm17 | null               | 1001      | 2001         | 6         | null                               |
| 18 | Alm18 | null               | 1001      | 2001         | 6         | null                               |
| 19 | Alm19 | null               | 1001      | 2001         | 6         | null                               |
| 20 | Alm20 | null               | 1001      | 2001         | 6         | null                               |
| 21 | Alm21 | null               | 1001      | 2001         | 6         | null                               |
| 22 | Alm22 | Wafer加载料框Z故障 | 1001      | 2001         | 6         | Wafer loading frame Z fault       |
| 23 | Alm23 | null               | 1001      | 2001         | 6         | null                               |
| 24 | Alm24 | null               | 1001      | 2001         | 6         | null                               |


```sh
7301=Alm1,Left dispensing X malfunction,Left dispensing X malfunction,1001,2001,6,
7302=Alm2,Left dispensing Y malfunction,Left dispensing Y malfunction,1001,2001,6,
7303=Alm3,Left dispensing Z malfunction,Left dispensing Z malfunction,1001,2001,6,
7304=Alm4,null,null,1001,2001,6,
7305=Alm5,null,null,1001,2001,6,
7306=Alm6,null,null,1001,2001,6,
7307=Alm7,Finger A motor malfunction,Finger A motor malfunction,1001,2001,6,
7308=Alm8,Finger B motor malfunction,Finger B motor malfunction,1001,2001,6,
7309=Alm9,Finger C motor malfunction,Finger C motor malfunction,1001,2001,6,
7310=Alm10,Finger D motor malfunction,Finger D motor malfunction,1001,2001,6,
7311=Alm11,null,null,1001,2001,6,
7312=Alm12,null,null,1001,2001,6,
7313=Alm13,Right dispensing X malfunction,Right dispensing X malfunction,1001,2001,6,
7314=Alm14,Right dispensing Y malfunction,Right dispensing Y malfunction,1001,2001,6,
7315=Alm15,Right dispensing Z malfunction,Right dispensing Z malfunction,1001,2001,6,
7316=Alm16,null,null,1001,2001,6,
7317=Alm17,null,null,1001,2001,6,
7318=Alm18,null,null,1001,2001,6,
7319=Alm19,null,null,1001,2001,6,
7320=Alm20,null,null,1001,2001,6,
7321=Alm21,null,null,1001,2001,6,
7322=Alm22,Wafer loading frame Z fault,Wafer loading frame Z fault,1001,2001,6,
7323=Alm23,null,null,1001,2001,6,
7324=Alm24,null,null,1001,2001,6,
```


## ALimitP (74)

| ID   | Name      | description                            | setEventID | clearEventID | alarm code | Text                               |
| ---- | --------- | -------------------------------------- | ---------- | ------------ | ---------- | ---------------------------------- |
| 1    | ALimitP1  | Welding head Z motor positive limit    | 1001       | 2001         | 6          | 焊头Z电机正限位                   |
| 2    | ALimitP2  | Welding head Y motor positive limit    | 1001       | 2001         | 6          | 焊头Y电机正限位                   |
| 3    | ALimitP3  | Camera Y motor positive limit          | 1001       | 2001         | 6          | 相机Y电机正限位                   |
| 4    | ALimitP4  | Welding head X motor positive limit    | 1001       | 2001         | 6          | 焊头X电机正限位                   |
| 5    | ALimitP5  | Pushing motor positive limit           | 1001       | 2001         | 6          | 推顶电机正限位                    |
| 6    | ALimitP6  | null                                   | 1001       | 2001         | 6          | null                               |
| 7    | ALimitP7  | Welding head A motor positive limit    | 1001       | 2001         | 6          | 焊头A电机正限位                   |
| 8    | ALimitP8  | null                                   | 1001       | 2001         | 6          | null                               |
| 9    | ALimitP9  | Crystal disc X motor positive limit    | 1001       | 2001         | 6          | 晶圆盘X电机正限位                 |
| 10   | ALimitP10 | null                                   | 1001       | 2001         | 6          | null                               |
| 11   | ALimitP11 | Positive limit of Y-motor on wafer disc | 1001       | 2001         | 6          | 晶圆盘Y电机正限位                 |
| 12   | ALimitP12 | null                                   | 1001       | 2001         | 6          | null                               |


```sh
7401=ALimitP1,Welding head Z motor positive limit,Welding head Z motor positive limit,1001,2001,6,
7402=ALimitP2,Welding head Y motor positive limit,Welding head Y motor positive limit,1001,2001,6,
7403=ALimitP3,Camera Y motor positive limit,Camera Y motor positive limit,1001,2001,6,
7404=ALimitP4,Welding head X motor positive limit,Welding head X motor positive limit,1001,2001,6,
7405=ALimitP5,Pushing motor positive limit,Pushing motor positive limit,1001,2001,6,
7406=ALimitP6,null,null,1001,2001,6,
7407=ALimitP7,Welding head A motor positive limit,Welding head A motor positive limit,1001,2001,6,
7408=ALimitP8,null,null,1001,2001,6,
7409=ALimitP9,Crystal disc X motor positive limit,Crystal disc X motor positive limit,1001,2001,6,
7410=ALimitP10,null,null,1001,2001,6,
7411=ALimitP11,Positive limit of Y-motor on wafer disc,Positive limit of Y-motor on wafer disc,1001,2001,6,
7412=ALimitP12,null,null,1001,2001,6,
```


## ALimitN (75)

| ID   | Name      | description                             | setEventID | clearEventID | alarm code | Text                               |
| ---- | --------- | --------------------------------------- | ---------- | ------------ | ---------- | ---------------------------------- |
| 1    | ALimitN1  | Crystal disc X motor positive limit     | 1001       | 2001         | 6          | 焊头Z电机负限位                   |
| 2    | ALimitN2  | Welding head Y motor negative limit     | 1001       | 2001         | 6          | 焊头Y电机负限位                   |
| 3    | ALimitN3  | Camera Y motor negative limit           | 1001       | 2001         | 6          | 相机Y电机负限位                   |
| 4    | ALimitN4  | Welding head X motor negative limit     | 1001       | 2001         | 6          | 焊头X电机负限位                   |
| 5    | ALimitN5  | Pushing motor negative limit            | 1001       | 2001         | 6          | 推顶电机负限位                    |
| 6    | ALimitN6  | null                                    | 1001       | 2001         | 6          | null                               |
| 7    | ALimitN7  | Welding head A motor negative limit     | 1001       | 2001         | 6          | 焊头A电机负限位                   |
| 8    | ALimitN8  | null                                    | 1001       | 2001         | 6          | null                               |
| 9    | ALimitN9  | Negative limit of crystal disc X motor  | 1001       | 2001         | 6          | 晶圆盘X电机负限位                 |
| 10   | ALimitN10 | null                                    | 1001       | 2001         | 6          | null                               |
| 11   | ALimitN11 | Negative limit of Y motor on wafer      | 1001       | 2001         | 6          | 晶圆盘Y电机负限位                 |
| 12   | ALimitN12 | null                                    | 1001       | 2001         | 6          | null                               |


```sh
7501=ALimitN1,Crystal disc X motor positive limit,Crystal disc X motor positive limit,1001,2001,6,
7502=ALimitN2,Welding head Y motor negative limit,Welding head Y motor negative limit,1001,2001,6,
7503=ALimitN3,Camera Y motor negative limit,Camera Y motor negative limit,1001,2001,6,
7504=ALimitN4,Welding head X motor negative limit,Welding head X motor negative limit,1001,2001,6,
7505=ALimitN5,Pushing motor negative limit,Pushing motor negative limit,1001,2001,6,
7506=ALimitN6,null,null,1001,2001,6,
7507=ALimitN7,Welding head A motor negative limit,Welding head A motor negative limit,1001,2001,6,
7508=ALimitN8,null,null,1001,2001,6,
7509=ALimitN9,Negative limit of crystal disc X motor,Negative limit of crystal disc X motor,1001,2001,6,
7510=ALimitN10,null,null,1001,2001,6,
7511=ALimitN11,Negative limit of Y motor on wafer,Negative limit of Y motor on wafer,1001,2001,6,
7512=ALimitN12,null,null,1001,2001,6,
```


## AAlm (76)


| ID   | Name    | description                         | setEventID | clearEventID | alarm code | Text                               |
| ---- | ------- | ----------------------------------- | ---------- | ------------ | ---------- | ---------------------------------- |
| 1    | AAlm1   | Welding head Z motor fault         | 1001       | 2001         | 6          | 焊头Z电机故障                     |
| 2    | AAlm2   | Welding head Y motor failure       | 1001       | 2001         | 6          | 焊头Y电机故障                     |
| 3    | AAlm3   | Camera Y motor fault               | 1001       | 2001         | 6          | 相机Y电机故障                     |
| 4    | AAlm4   | Welding head X motor failure       | 1001       | 2001         | 6          | 焊头X电机故障                     |
| 5    | AAlm5   | Pushing motor fault                | 1001       | 2001         | 6          | 推顶电机故障                      |
| 6    | AAlm6   | Welding head torque motor failure  | 1001       | 2001         | 6          | 焊头力扭电机故障                  |
| 7    | AAlm7   | Welding head A motor failure       | 1001       | 2001         | 6          | 焊头A电机故障                     |
| 8    | AAlm8   | null                               | 1001       | 2001         | 6          | null                               |
| 9    | AAlm9   | Crystal disc X motor failure       | 1001       | 2001         | 6          | 晶圆盘X电机故障                   |
| 10   | AAlm10  | null                               | 1001       | 2001         | 6          | null                               |
| 11   | AAlm11  | Wafer disk Y motor failure         | 1001       | 2001         | 6          | 晶圆盘Y电机故障                   |
| 12   | AAlm12  | null                               | 1001       | 2001         | 6          | null                               |



```sh
7601=AAlm1,Welding head Z motor fault,Welding head Z motor fault,1001,2001,6,
7602=AAlm2,Welding head Y motor failure,Welding head Y motor failure,1001,2001,6,
7603=AAlm3,Camera Y motor fault,Camera Y motor fault,1001,2001,6,
7604=AAlm4,Welding head X motor failure,Welding head X motor failure,1001,2001,6,
7605=AAlm5,Pushing motor fault,Pushing motor fault,1001,2001,6,
7606=AAlm6,Welding head torque motor failure,Welding head torque motor failure,1001,2001,6,
7607=AAlm7,Welding head A motor failure,Welding head A motor failure,1001,2001,6,
7608=AAlm8,null,null,1001,2001,6,
7609=AAlm9,Crystal disc X motor failure,Crystal disc X motor failure,1001,2001,6,
7610=AAlm10,null,null,1001,2001,6,
7611=AAlm11,Wafer disk Y motor failure,Wafer disk Y motor failure,1001,2001,6,
7612=AAlm12,null,null,1001,2001,6,
```