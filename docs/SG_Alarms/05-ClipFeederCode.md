# 05-ClipFeederCode alarm code（OK）

| ID   | Name   | Description                                                  | setEventID | clearEventID | alarm code | Text                                 |
| ---- | ------ | ------------------------------------------------------------ | ---------- | ------------ | ---------- | ------------------------------------ |
| 1    | AC0501 | Waste detection full!                                        | 1001       | 2001         | 6          | 废料检测满！                         |
| 2    | AC0502 | Stripe detection is abnormal!                                | 1001       | 2001         | 6          | 条带检测异常！                       |
| 3    | AC0503 | Strip unwind timeout!                                        | 1001       | 2001         | 6          | 条带放卷超时！                       |
| 4    | AC0504 | Stripe Buffer exits abnormally!                              | 1001       | 2001         | 6          | 条带Buffer异常退出！                 |
| 5    | AC0505 | Strip motor movement timeout;current coordinates:            | 1001       | 2001         | 6          | 条带电机移动超时;当前坐标：          |
| 6    | AC0506 | The strip detects the hole in advance!                       | 1001       | 2001         | 6          | 条带提前探测到孔！                   |
| 7    | AC0507 | Strip hole search overruns!                                  | 1001       | 2001         | 6          | 条带孔搜索超限！                     |
| 8    | AC0508 | Stripe Buffer exit timeout!                                  | 1001       | 2001         | 6          | 条带Buffer退出超时！                 |
| 9    | AC0509 | Send Stripe Buffer exit timeout!                             | 1001       | 2001         | 6          | 送条带Buffer退出超时！               |
| 10   | AC0510 | The strip station is running automatically;please stop it and then operate it! | 1001       | 2001         | 6          | 条带工位自动运行中，请停止后在操作！ |
| 11   | AC0511 | Punch not in safe position                                   | 1001       | 2001         | 6          | 冲切不在安全位                       |
| 12   | AC0512 | Search strip hole timeout                                    | 1001       | 2001         | 6          | 搜索条带孔超时                       |
| 13   | AC0513 | Please stop and then operate!                                | 1001       | 2001         | 6          | 请停止后在操作！                     |
| 14   | AC0514 | Please initialize it and then operate it!                    | 1001       | 2001         | 6          | 请初始化后在操作！                   |
| 15   | AC0515 | Punch not in safe position                                   | 1001       | 2001         | 6          | 冲切不在安全位                       |
| 16   | AC0516 | P&P Z is not in a safe position                              | 1001       | 2001         | 6          | 焊头Z不在安全位                      |



```sh
8501=AC0501,Waste detection full!,Waste detection full!,1001,2001,6,
8502=AC0502,Stripe detection is abnormal!,Stripe detection is abnormal!,1001,2001,6,
8503=AC0503,Strip unwind timeout!,Strip unwind timeout!,1001,2001,6,
8504=AC0504,Stripe Buffer exits abnormally!,Stripe Buffer exits abnormally!,1001,2001,6,
8505=AC0505,Strip motor movement timeout;current coordinates:,Strip motor movement timeout;current coordinates:,1001,2001,6,
8506=AC0506,The strip detects the hole in advance!,The strip detects the hole in advance!,1001,2001,6,
8507=AC0507,Strip hole search overruns!,Strip hole search overruns!,1001,2001,6,
8508=AC0508,Stripe Buffer exit timeout!,Stripe Buffer exit timeout!,1001,2001,6,
8509=AC0509,Send Stripe Buffer exit timeout!,Send Stripe Buffer exit timeout!,1001,2001,6,
8510=AC0510,The strip station is running automatically;please stop it and then operate it!,The strip station is running automatically;please stop it and then operate it!,1001,2001,6,
8511=AC0511,Punch not in safe position,Punch not in safe position,1001,2001,6,
8512=AC0512,Search strip hole timeout,Search strip hole timeout,1001,2001,6,
8513=AC0513,Please stop and then operate!,Please stop and then operate!,1001,2001,6,
8514=AC0514,Please initialize it and then operate it!,Please initialize it and then operate it!,1001,2001,6,
8515=AC0515,Punch not in safe position,Punch not in safe position,1001,2001,6,
8516=AC0516,P&P Z is not in a safe position,P&P Z is not in a safe position,1001,2001,6,

```