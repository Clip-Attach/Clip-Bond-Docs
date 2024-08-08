# 01-Avaline_D die bonding alarm code

| ID   | Name   | Description                                         | setEventID | clearEventID | alarm code | Text                       |
| ---- | ------ | --------------------------------------------------- | ---------- | ------------ | ---------- | -------------------------- |
| 1    | AC0101 | Door switch detection is abnormal!                  | 1001       | 2001         | 6          | 门开关检测异常！           |
| 2    | AC0102 | Window already open, no need to open it again       | 1001       | 2001         | 6          | 窗口已打开,无需重复打开    |
| 3    | AC0103 | Startup failed, please reset and start again!       | 1001       | 2001         | 6          | 启动失败，请复位后再启动！ |
| 4    | AC0104 | Failed to load power supply!                        | 1001       | 2001         | 6          | 加载电源失败！             |
| 5    | AC0105 | Please wait while the servo motor is being enabled! | 1001       | 2001         | 6          | 伺服电机加使能中，请稍等！ |
| 6    | AC0106 | Emergency stop button pressed!                      | 1001       | 2001         | 6          | 急停按钮按下！             |
| 7    | AC0107 | Please initialize the P&P first.                    | 1001       | 2001         | 6          | 请先绑头初始化             |
| 8    | AC0108 | Please initialize the strip first.                  | 1001       | 2001         | 6          | 请先条带初始化             |
| 9    | AC0109 | Please reset after stopping!                        | 1001       | 2001         | 6          | 请停止后再复位！           |
| 10   | AC0110 | Reset failed!                                       | 1001       | 2001         | 6          | 复位失败！                 |
| 11   | AC0111 | Failed to start, on clear track!                    | 1001       | 2001         | 6          | 启动失败，在清轨道！       |
| 12   | AC0112 | Please stop the unit and then operate it!           | 1001       | 2001         | 6          | 请停止设备后在操作！       |



```sh
8101=AC0101,Please stop the equipment before operating!,Please stop the device before proceeding!,1001,2001,6,
8102=AC0102,Entering illegal parameters,Entering illegal parameters,1001,2001,6,
8103=AC0103,Camera initialization failed& program cannot start....,Camera initialization failed& program cannot start....,1001,2001,6,

```

## LimitP (71)(OK)

| ID   | Name     | description                       | setEventID | clearEventID | alarm code | Text            |
| ---- | -------- | --------------------------------- | ---------- | ------------ | ---------- | --------------- |
| 1    | LimitP1  | Left dispensing X positive limit  | 1001       | 2001         | 6          | 左点胶X正限位   |
| 2    | LimitP2  | Left dispensing Y positive limit  | 1001       | 2001         | 6          | 左点胶Y正限位   |
| 3    | LimitP3  | Left dispensing Z positive limit  | 1001       | 2001         | 6          | 左点胶Z正限位   |
| 4    | LimitP4  | null                              | 1001       | 2001         | 6          | null            |
| 5    | LimitP5  | null                              | 1001       | 2001         | 6          | null            |
| 6    | LimitP6  | null                              | 1001       | 2001         | 6          | null            |
| 7    | LimitP7  | null                              | 1001       | 2001         | 6          | null            |
| 8    | LimitP8  | Finger B motor positive limit     | 1001       | 2001         | 6          | 手指B电机正限位 |
| 9    | LimitP9  | Finger C motor positive limit     | 1001       | 2001         | 6          | 手指C电机正限位 |
| 10   | LimitP10 | Finger D motor positive limit     | 1001       | 2001         | 6          | 手指D电机正限位 |
| 11   | LimitP11 | null                              | 1001       | 2001         | 6          | null            |
| 12   | LimitP12 | null                              | 1001       | 2001         | 6          | null            |
| 13   | LimitP13 | Right dispensing X positive limit | 1001       | 2001         | 6          | 右点胶X正限位   |
| 14   | LimitP14 | Right dispensing Y positive limit | 1001       | 2001         | 6          | 右点胶Y正限位   |
| 15   | LimitP15 | Right dispensing Z positive limit | 1001       | 2001         | 6          | 右点胶Z正限位   |
| 16   | LimitP16 | null                              | 1001       | 2001         | 6          | null            |
| 17   | LimitP17 | null                              | 1001       | 2001         | 6          | null            |
| 18   | LimitP18 | null                              | 1001       | 2001         | 6          | null            |


```sh
7101=LimitP1,Left dispensing X positive limit,Left dispensing X positive limit,1001,2001,6,
7102=LimitP2,Left dispensing Y positive limit,Left dispensing Y positive limit,1001,2001,6,
7103=LimitP3,Left dispensing Z positive limit,Left dispensing Z positive limit,1001,2001,6,

```

## LimitN (72)（OK）

| ID | Name     | description        | setEventID | clearEventID | alarm code | Text                                      |
|----|----------|--------------------|-----------|--------------|-----------|--------------------------------------------|
| 1  | LimitN1  | Left dispensing X negative limit | 1001      | 2001         | 6         | 左点胶X负限位    |
| 2  | LimitN2  | Left dispensing Y negative limit | 1001      | 2001         | 6         | 左点胶Y负限位    |
| 3  | LimitN3  | Left dispensing Z negative limit | 1001      | 2001         | 6         | 左点胶Z负限位    |
| 4  | LimitN4  | null  | 1001      | 2001         | 6         | null       |
| 5  | LimitN5  | null               | 1001      | 2001         | 6         | null                                       |
| 6  | LimitN6  | null               | 1001      | 2001         | 6         | null                                       |
| 7  | LimitN7  | Finger A motor negative limit | 1001      | 2001         | 6         | 手指A电机负限位  |
| 8  | LimitN8  | Finger B motor negative limit | 1001      | 2001         | 6         | 手指B电机负限位      |
| 9  | LimitN9  | Finger C motor negative limit | 1001      | 2001         | 6         | 手指C电机负限位      |
| 10 | LimitN10 | Finger D motor negative limit | 1001      | 2001         | 6         | 手指D电机负限位      |
| 11 | LimitN11 | null               | 1001      | 2001         | 6         | null                                       |
| 12 | LimitN12 | null               | 1001      | 2001         | 6         | null                                       |
| 13 | LimitN13 | Right dispensing X negative limit | 1001      | 2001         | 6         | 右点胶X负限位   |
| 14 | LimitN14 | Right dispensing Y negative limit | 1001      | 2001         | 6         | 右点胶Y负限位   |
| 15 | LimitN15 | Right dispensing Z negative limit | 1001      | 2001         | 6         | 右点胶Z负限位   |
| 16 | LimitN16 | null               | 1001      | 2001         | 6         | null                                       |
| 17 | LimitN17 | null               | 1001      | 2001         | 6         | null                                       |
| 18 | LimitN18 | null | 1001      | 2001         | 6         | null |


```sh
7201=LimitN1,Left dispensing X negative limit,Left dispensing X negative limit,1001,2001,6,
7202=LimitN2,Left dispensing Y negative limit,Left dispensing Y negative limit,1001,2001,6,
7203=LimitN3,Left dispensing Z negative limit,Left dispensing Z negative limit,1001,2001,6,

```


## Alm (73)（OK）

| ID | Name  | description        | setEventID | clearEventID | alarm code | Text                              |
|----|-------|--------------------|-----------|--------------|-----------|------------------------------------|
| 1  | Alm1  | Left dispensing X malfunction | 1001      | 2001         | 6         | 左点胶X故障 |
| 2  | Alm2  | Left dispensing Y malfunction | 1001      | 2001         | 6         | 左点胶Y故障 |
| 3  | Alm3  | Left dispensing Z malfunction | 1001      | 2001         | 6         | 左点胶Z故障 |
| 4  | Alm4  | null               | 1001      | 2001         | 6         | null                               |
| 5  | Alm5  | null               | 1001      | 2001         | 6         | null                               |
| 6  | Alm6  | null               | 1001      | 2001         | 6         | null                               |
| 7  | Alm7  | Finger A motor malfunction | 1001      | 2001         | 6         | 手指A电机故障 |
| 8  | Alm8  | Finger B motor malfunction | 1001      | 2001         | 6         | 手指B电机故障 |
| 9  | Alm9  | Finger C motor malfunction | 1001      | 2001         | 6         | 手指C电机故障 |
| 10 | Alm10 | Finger D motor malfunction | 1001      | 2001         | 6         | 手指D电机故障 |
| 11 | Alm11 | null               | 1001      | 2001         | 6         | null                               |
| 12 | Alm12 | null               | 1001      | 2001         | 6         | null                               |
| 13 | Alm13 | Right dispensing X malfunction | 1001      | 2001         | 6         | 右点胶X故障 |
| 14 | Alm14 | Right dispensing Y malfunction | 1001      | 2001         | 6         | 右点胶Y故障 |
| 15 | Alm15 | Right dispensing Z malfunction | 1001      | 2001         | 6         | 右点胶Z故障 |
| 16 | Alm16 | null               | 1001      | 2001         | 6         | null                               |
| 17 | Alm17 | null               | 1001      | 2001         | 6         | null                               |
| 18 | Alm18 | null               | 1001      | 2001         | 6         | null                               |


```sh
7301=Alm1,Left dispensing X malfunction,Left dispensing X malfunction,1001,2001,6,
7302=Alm2,Left dispensing Y malfunction,Left dispensing Y malfunction,1001,2001,6,
7303=Alm3,Left dispensing Z malfunction,Left dispensing Z malfunction,1001,2001,6,

```


## ALimitP (74)（OK）

| ID   | Name      | description                            | setEventID | clearEventID | alarm code | Text                               |
| ---- | --------- | -------------------------------------- | ---------- | ------------ | ---------- | ---------------------------------- |
| 1    | ALimitP1  | Welding head Z motor positive limit    | 1001       | 2001         | 6          | 绑头Z电机正限位           |
| 2    | ALimitP2  | Welding head Y motor positive limit    | 1001       | 2001         | 6          | 绑头Y电机正限位           |
| 3    | ALimitP3  | null      | 1001       | 2001         | 6          | null               |
| 4    | ALimitP4  | null | 1001       | 2001         | 6          | null               |
| 5    | ALimitP5  | P&P A motor positive limit | 1001       | 2001         | 6          | 焊头A电机正限位            |
| 6    | ALimitP6  | P&P X motor positive limit         | 1001       | 2001         | 6          | 绑头X电机正限位                       |
| 7    | ALimitP7  | Camera Y motor positive limit       | 1001       | 2001         | 6          | 相机Y电机正限位 |
| 8    | ALimitP8  | Cutter motor positive limit         | 1001       | 2001         | 6          | 切刀电机正限位  |
| 9    | ALimitP9  | null                                | 1001       | 2001         | 6          | null            |
| 10   | ALimitP10 | null                                | 1001       | 2001         | 6          | null            |


```sh
7401=ALimitP1,Welding head Z motor positive limit,Welding head Z motor positive limit,1001,2001,6,
7402=ALimitP2,Welding head Y motor positive limit,Welding head Y motor positive limit,1001,2001,6,
7403=ALimitP3,Camera Y motor positive limit,Camera Y motor positive limit,1001,2001,6,

```


## ALimitN (75)

| ID   | Name      | description                             | setEventID | clearEventID | alarm code | Text                               |
| ---- | --------- | --------------------------------------- | ---------- | ------------ | ---------- | ---------------------------------- |
| 1    | ALimitN1  | P&P Z motor negative limit | 1001       | 2001         | 6          | 绑头Z电机负限位           |
| 2    | ALimitN2  | P&P Y motor negative limit | 1001       | 2001         | 6          | 绑头Y电机负限位           |
| 3    | ALimitN3  | null       | 1001       | 2001         | 6          | null               |
| 4    | ALimitN4  | null | 1001       | 2001         | 6          | null               |
| 5    | ALimitN5  | P&P A motor negative limit | 1001       | 2001         | 6          | 焊头A电机负限位            |
| 6    | ALimitN6  | P&P X motor negative limit    | 1001       | 2001         | 6          | 绑头X电机负限位 |
| 7    | ALimitN7  | Camera Y motor negative limit | 1001       | 2001         | 6          | 相机Y电机负限位 |
| 8    | ALimitN8  | Cutter motor negative limit   | 1001       | 2001         | 6          | 切刀电机负限位  |
| 9    | ALimitN9  | null                          | 1001       | 2001         | 6          | null            |
| 10   | ALimitN10 | null                          | 1001       | 2001         | 6          | null            |


```sh
7501=ALimitN1,Crystal disc X motor positive limit,Crystal disc X motor positive limit,1001,2001,6,
7502=ALimitN2,Welding head Y motor negative limit,Welding head Y motor negative limit,1001,2001,6,
7503=ALimitN3,Camera Y motor negative limit,Camera Y motor negative limit,1001,2001,6,

```


## AAlm (76)


| ID   | Name    | description                         | setEventID | clearEventID | alarm code | Text                               |
| ---- | ------- | ----------------------------------- | ---------- | ------------ | ---------- | ---------------------------------- |
| 1    | AAlm1   | P&P Z motor failure | 1001       | 2001         | 6          | 绑头Z电机故障              |
| 2    | AAlm2   | P&P Y motor failure | 1001       | 2001         | 6          | 绑头Y电机故障              |
| 3    | AAlm3   | null           | 1001       | 2001         | 6          | null                 |
| 4    | AAlm4   | null   | 1001       | 2001         | 6          | null                 |
| 5    | AAlm5   | P&P A motor failure | 1001       | 2001         | 6          | 焊头A电机故障               |
| 6    | AAlm6  | P&P X motor failure      | 1001       | 2001         | 6          | 绑头X电机故障  |
| 7    | AAlm7  | Camera Y motor failure   | 1001       | 2001         | 6          | 相机Y电机故障  |
| 8    | AAlm8  | Cutter motor failure     | 1001       | 2001         | 6          | 切刀电机故障   |
| 9    | AAlm9  | Strip feed motor failure | 1001       | 2001         | 6          | 送条带电机故障 |
| 10   | AAlm10 | null                     | 1001       | 2001         | 6          | null           |

```sh
7601=AAlm1,Welding head Z motor fault,Welding head Z motor fault,1001,2001,6,
7602=AAlm2,Welding head Y motor failure,Welding head Y motor failure,1001,2001,6,
7603=AAlm3,Camera Y motor fault,Camera Y motor fault,1001,2001,6,

```