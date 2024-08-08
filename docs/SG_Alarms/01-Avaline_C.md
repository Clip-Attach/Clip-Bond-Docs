# 01-Avaline_C die bonding alarm code

| ID   | Name   | Description                                         | setEventID | clearEventID | alarm code | Text                       |
| ---- | ------ | --------------------------------------------------- | ---------- | ------------ | ---------- | -------------------------- |
| 1    | AC0101 | Door switch detection is abnormal!                  | 1001       | 2001         | 6          | 门开关检测异常！           |
| 2    | AC0102 | Window already open;no need to open it again        | 1001       | 2001         | 6          | 窗口已打开,无需重复打开    |
| 3    | AC0103 | Startup failed;please reset and start again!        | 1001       | 2001         | 6          | 启动失败，请复位后再启动！ |
| 4    | AC0104 | Failed to load power supply!                        | 1001       | 2001         | 6          | 加载电源失败！             |
| 5    | AC0105 | Please wait while the servo motor is being enabled! | 1001       | 2001         | 6          | 伺服电机加使能中，请稍等！ |
| 6    | AC0106 | Emergency stop button pressed!                      | 1001       | 2001         | 6          | 急停按钮按下！             |
| 7    | AC0107 | Please initialize the P&P first.                    | 1001       | 2001         | 6          | 请先绑头初始化             |
| 8    | AC0108 | Please initialize the strip first.                  | 1001       | 2001         | 6          | 请先条带初始化             |
| 9    | AC0109 | Please reset after stopping!                        | 1001       | 2001         | 6          | 请停止后再复位！           |
| 10   | AC0110 | Reset failed!                                       | 1001       | 2001         | 6          | 复位失败！                 |
| 11   | AC0111 | Failed to start;on clear track!                     | 1001       | 2001         | 6          | 启动失败，在清轨道！       |
| 12   | AC0112 | Please stop the unit and then operate it!           | 1001       | 2001         | 6          | 请停止设备后在操作！       |



```sh
8101=AC0101,Door switch detection is abnormal!,Door switch detection is abnormal!,1001,2001,6,
8102=AC0102,Window already open;no need to open it again,Window already open;no need to open it again,1001,2001,6,
8103=AC0103,Startup failed;please reset and start again!,Startup failed;please reset and start again!,1001,2001,6,
8104=AC0104,Failed to load power supply!,Failed to load power supply!,1001,2001,6,
8105=AC0105,Please wait while the servo motor is being enabled!,Please wait while the servo motor is being enabled!,1001,2001,6,
8106=AC0106,Emergency stop button pressed!,Emergency stop button pressed!,1001,2001,6,
8107=AC0107,Please initialize the P&P first.,Please initialize the P&P first.,1001,2001,6,
8108=AC0108,Please initialize the strip first.,Please initialize the strip first.,1001,2001,6,
8109=AC0109,Please reset after stopping!,Please reset after stopping!,1001,2001,6,
8110=AC0110,Reset failed!,Reset failed!,1001,2001,6,
8111=AC0111,Failed to start;on clear track!,Failed to start;on clear track!,1001,2001,6,
8112=AC0112,Please stop the unit and then operate it!,Please stop the unit and then operate it!,1001,2001,6,

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
7104=LimitP4,null,null,1001,2001,6,
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
7118=LimitP18,null,null,1001,2001,6,

```

## LimitN (72)（OK）

| ID   | Name     | description                       | setEventID | clearEventID | alarm code | Text            |
| ---- | -------- | --------------------------------- | ---------- | ------------ | ---------- | --------------- |
| 1    | LimitN1  | Left dispensing X negative limit  | 1001       | 2001         | 6          | 左点胶X负限位   |
| 2    | LimitN2  | Left dispensing Y negative limit  | 1001       | 2001         | 6          | 左点胶Y负限位   |
| 3    | LimitN3  | Left dispensing Z negative limit  | 1001       | 2001         | 6          | 左点胶Z负限位   |
| 4    | LimitN4  | null                              | 1001       | 2001         | 6          | null            |
| 5    | LimitN5  | null                              | 1001       | 2001         | 6          | null            |
| 6    | LimitN6  | null                              | 1001       | 2001         | 6          | null            |
| 7    | LimitN7  | Finger A motor negative limit     | 1001       | 2001         | 6          | 手指A电机负限位 |
| 8    | LimitN8  | Finger B motor negative limit     | 1001       | 2001         | 6          | 手指B电机负限位 |
| 9    | LimitN9  | Finger C motor negative limit     | 1001       | 2001         | 6          | 手指C电机负限位 |
| 10   | LimitN10 | Finger D motor negative limit     | 1001       | 2001         | 6          | 手指D电机负限位 |
| 11   | LimitN11 | null                              | 1001       | 2001         | 6          | null            |
| 12   | LimitN12 | null                              | 1001       | 2001         | 6          | null            |
| 13   | LimitN13 | Right dispensing X negative limit | 1001       | 2001         | 6          | 右点胶X负限位   |
| 14   | LimitN14 | Right dispensing Y negative limit | 1001       | 2001         | 6          | 右点胶Y负限位   |
| 15   | LimitN15 | Right dispensing Z negative limit | 1001       | 2001         | 6          | 右点胶Z负限位   |
| 16   | LimitN16 | null                              | 1001       | 2001         | 6          | null            |
| 17   | LimitN17 | null                              | 1001       | 2001         | 6          | null            |
| 18   | LimitN18 | null                              | 1001       | 2001         | 6          | null            |



```sh
7201=LimitN1,Left dispensing X negative limit,Left dispensing X negative limit,1001,2001,6,
7202=LimitN2,Left dispensing Y negative limit,Left dispensing Y negative limit,1001,2001,6,
7203=LimitN3,Left dispensing Z negative limit,Left dispensing Z negative limit,1001,2001,6,
7204=LimitN4,null,null,1001,2001,6,
7205=LimitN5,null,null,1001,2001,6,
7206=LimitN6,null,null,1001,2001,6,
7207=LimitN7,Finger A motor negative limit,Finger A motor negative limit,1001,2001,6,
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
7218=LimitN18,null,null,1001,2001,6,

```


## Alm (73)（OK）

| ID   | Name  | description                    | setEventID | clearEventID | alarm code | Text          |
| ---- | ----- | ------------------------------ | ---------- | ------------ | ---------- | ------------- |
| 1    | Alm1  | Left dispensing X malfunction  | 1001       | 2001         | 6          | 左点胶X故障   |
| 2    | Alm2  | Left dispensing Y malfunction  | 1001       | 2001         | 6          | 左点胶Y故障   |
| 3    | Alm3  | Left dispensing Z malfunction  | 1001       | 2001         | 6          | 左点胶Z故障   |
| 4    | Alm4  | null                           | 1001       | 2001         | 6          | null          |
| 5    | Alm5  | null                           | 1001       | 2001         | 6          | null          |
| 6    | Alm6  | null                           | 1001       | 2001         | 6          | null          |
| 7    | Alm7  | Finger A motor malfunction     | 1001       | 2001         | 6          | 手指A电机故障 |
| 8    | Alm8  | Finger B motor malfunction     | 1001       | 2001         | 6          | 手指B电机故障 |
| 9    | Alm9  | Finger C motor malfunction     | 1001       | 2001         | 6          | 手指C电机故障 |
| 10   | Alm10 | Finger D motor malfunction     | 1001       | 2001         | 6          | 手指D电机故障 |
| 11   | Alm11 | null                           | 1001       | 2001         | 6          | null          |
| 12   | Alm12 | null                           | 1001       | 2001         | 6          | null          |
| 13   | Alm13 | Right dispensing X malfunction | 1001       | 2001         | 6          | 右点胶X故障   |
| 14   | Alm14 | Right dispensing Y malfunction | 1001       | 2001         | 6          | 右点胶Y故障   |
| 15   | Alm15 | Right dispensing Z malfunction | 1001       | 2001         | 6          | 右点胶Z故障   |
| 16   | Alm16 | null                           | 1001       | 2001         | 6          | null          |
| 17   | Alm17 | null                           | 1001       | 2001         | 6          | null          |
| 18   | Alm18 | null                           | 1001       | 2001         | 6          | null          |



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

```


## ALimitP (74)（OK）

| ID   | Name      | description                   | setEventID | clearEventID | alarm code | Text            |
| ---- | --------- | ----------------------------- | ---------- | ------------ | ---------- | --------------- |
| 1    | ALimitP1  | P&P Z motor positive limit    | 1001       | 2001         | 6          | 绑头Z电机正限位 |
| 2    | ALimitP2  | P&P Y motor positive limit    | 1001       | 2001         | 6          | 绑头Y电机正限位 |
| 3    | ALimitP3  | null                          | 1001       | 2001         | 6          | null            |
| 4    | ALimitP4  | null                          | 1001       | 2001         | 6          | null            |
| 5    | ALimitP5  | P&P A motor positive limit    | 1001       | 2001         | 6          | 焊头A电机正限位 |
| 6    | ALimitP6  | P&P X motor positive limit    | 1001       | 2001         | 6          | 绑头X电机正限位 |
| 7    | ALimitP7  | Camera Y motor positive limit | 1001       | 2001         | 6          | 相机Y电机正限位 |
| 8    | ALimitP8  | Cutter motor positive limit   | 1001       | 2001         | 6          | 切刀电机正限位  |
| 9    | ALimitP9  | null                          | 1001       | 2001         | 6          | null            |
| 10   | ALimitP10 | null                          | 1001       | 2001         | 6          | null            |



```sh
7401=ALimitP1,P&P Z motor positive limit,P&P Z motor positive limit,1001,2001,6,
7402=ALimitP2,P&P Y motor positive limit,P&P Y motor positive limit,1001,2001,6,
7403=ALimitP3,null,null,1001,2001,6,
7404=ALimitP4,null,null,1001,2001,6,
7405=ALimitP5,P&P A motor positive limit,P&P A motor positive limit,1001,2001,6,
7406=ALimitP6,P&P X motor positive limit,P&P X motor positive limit,1001,2001,6,
7407=ALimitP7,Camera Y motor positive limit,Camera Y motor positive limit,1001,2001,6,
7408=ALimitP8,Cutter motor positive limit,Cutter motor positive limit,1001,2001,6,
7409=ALimitP9,null,null,1001,2001,6,
7410=ALimitP10,null,null,1001,2001,6,

```


## ALimitN (75)

| ID   | Name      | description                   | setEventID | clearEventID | alarm code | Text            |
| ---- | --------- | ----------------------------- | ---------- | ------------ | ---------- | --------------- |
| 1    | ALimitN1  | P&P Z motor negative limit    | 1001       | 2001         | 6          | 绑头Z电机负限位 |
| 2    | ALimitN2  | P&P Y motor negative limit    | 1001       | 2001         | 6          | 绑头Y电机负限位 |
| 3    | ALimitN3  | null                          | 1001       | 2001         | 6          | null            |
| 4    | ALimitN4  | null                          | 1001       | 2001         | 6          | null            |
| 5    | ALimitN5  | P&P A motor negative limit    | 1001       | 2001         | 6          | 焊头A电机负限位 |
| 6    | ALimitN6  | P&P X motor negative limit    | 1001       | 2001         | 6          | 绑头X电机负限位 |
| 7    | ALimitN7  | Camera Y motor negative limit | 1001       | 2001         | 6          | 相机Y电机负限位 |
| 8    | ALimitN8  | Cutter motor negative limit   | 1001       | 2001         | 6          | 切刀电机负限位  |
| 9    | ALimitN9  | null                          | 1001       | 2001         | 6          | null            |
| 10   | ALimitN10 | null                          | 1001       | 2001         | 6          | null            |



```sh
7501=ALimitN1,P&P Z motor negative limit,P&P Z motor negative limit,1001,2001,6,
7502=ALimitN2,P&P Y motor negative limit,P&P Y motor negative limit,1001,2001,6,
7503=ALimitN3,null,null,1001,2001,6,
7504=ALimitN4,null,null,1001,2001,6,
7505=ALimitN5,P&P A motor negative limit,P&P A motor negative limit,1001,2001,6,
7506=ALimitN6,P&P X motor negative limit,P&P X motor negative limit,1001,2001,6,
7507=ALimitN7,Camera Y motor negative limit,Camera Y motor negative limit,1001,2001,6,
7508=ALimitN8,Cutter motor negative limit,Cutter motor negative limit,1001,2001,6,
7509=ALimitN9,null,null,1001,2001,6,
7510=ALimitN10,null,null,1001,2001,6,

```


## AAlm (76)


| ID   | Name   | description              | setEventID | clearEventID | alarm code | Text           |
| ---- | ------ | ------------------------ | ---------- | ------------ | ---------- | -------------- |
| 1    | AAlm1  | P&P Z motor failure      | 1001       | 2001         | 6          | 绑头Z电机故障  |
| 2    | AAlm2  | P&P Y motor failure      | 1001       | 2001         | 6          | 绑头Y电机故障  |
| 3    | AAlm3  | null                     | 1001       | 2001         | 6          | null           |
| 4    | AAlm4  | null                     | 1001       | 2001         | 6          | null           |
| 5    | AAlm5  | P&P A motor failure      | 1001       | 2001         | 6          | 焊头A电机故障  |
| 6    | AAlm6  | P&P X motor failure      | 1001       | 2001         | 6          | 绑头X电机故障  |
| 7    | AAlm7  | Camera Y motor failure   | 1001       | 2001         | 6          | 相机Y电机故障  |
| 8    | AAlm8  | Cutter motor failure     | 1001       | 2001         | 6          | 切刀电机故障   |
| 9    | AAlm9  | Strip feed motor failure | 1001       | 2001         | 6          | 送条带电机故障 |
| 10   | AAlm10 | null                     | 1001       | 2001         | 6          | null           |



```sh
7601=AAlm1,P&P Z motor failure,P&P Z motor failure,1001,2001,6,
7602=AAlm2,P&P Y motor failure,P&P Y motor failure,1001,2001,6,
7603=AAlm3,null,null,1001,2001,6,
7604=AAlm4,null,null,1001,2001,6,
7605=AAlm5,P&P A motor failure,P&P A motor failure,1001,2001,6,
7606=AAlm6,P&P X motor failure,P&P X motor failure,1001,2001,6,
7607=AAlm7,Camera Y motor failure,Camera Y motor failure,1001,2001,6,
7608=AAlm8,Cutter motor failure,Cutter motor failure,1001,2001,6,
7609=AAlm9,Strip feed motor failure,Strip feed motor failure,1001,2001,6,
7610=AAlm10,null,null,1001,2001,6,

```