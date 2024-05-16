# 01-Avaline_D die bonding alarm code

| ID   | Alarm code | Information  English                                         | Information  Chinese                    |
| ---- | ---------- | ------------------------------------------------------------ | --------------------------------------- |
| 1    | AC0101     | Failed to link ACS drive, program cannot start.....          | 链接ACS驱动器失败，程序无法启动.....    |
| 2    | AC0102     | The motion control card failed to initialize and the program could not be started..... | 运动控制卡初始化失败，程序无法启动..... |
| 3    | AC0103     | The camera initialization failed and the program cannot be started..... | 相机初始化失败，程序无法启动.....       |
| 4    | AC0104     | Door switch detection abnormality!                           | 门开关检测异常！                        |
| 5    | AC0105     | The window is already open, no need to open it again         | 窗口已打开,无需重复打开                 |
| 6    | AC0106     | Startup failed, please reset and start again!                | 启动失败，请复位后再启动！              |
| 7    | AC0107     | The servo motor is being enabled, please wait!               | 伺服电机加使能中，请稍等！              |
| 8    | AC0108     | Enter illegal parameters                                     | 输入非法参数                            |
| 9    | AC0109     | Please stop the equipment before operating!                  | 请停止设备后在操作！                    |
| 10   | AC0110     | Please initialize the header first                           | 请先绑头初始化                          |
| 11   | AC0111     | Please initialize the strip first                            | 请先条带初始化                          |
| 12   | AC0112     | Please stop and then reset!                                  | 请停止后再复位！                        |
| 13   | AC0113     | Reset failed!                                                | 复位失败！                              |
| 14   | AC0114     | Failed to start, clearing track!                             | 启动失败，在清轨道！                    |


## LimitP

- 因为这部分绑定了硬件，所以这样设计
  
| ID   | Alarm code | Information  English              | Information  Chinese |
| ---- | ---------- | --------------------------------- | -------------------- |
| 1    | LimitP1    | Left dispensing X positive limit  | 左点胶X正限位        |
| 2    | LimitP2    | Left dispensing Y positive limit  | 左点胶Y正限位        |
| 3    | LimitP3    | Left dispensing Z positive limit  | 左点胶Z正限位        |
| 4    | LimitP4    | null                              | null                 |
| 5    | LimitP5    | null                              | null                 |
| 6    | LimitP6    | null                              | null                 |
| 7    | LimitP7    | null                              | null                 |
| 8    | LimitP8    | Finger B motor positive limit     | 手指B电机正限位      |
| 9    | LimitP9    | Finger C motor positive limit     | 手指C电机正限位      |
| 10   | LimitP10   | Finger D motor positive limit     | 手指D电机正限位      |
| 11   | LimitP11   | null                              | null                 |
| 12   | LimitP12   | null                              | null                 |
| 13   | LimitP13   | Right dispensing X positive limit | 右点胶X正限位        |
| 14   | LimitP14   | Right dispensing Y positive limit | 右点胶Y正限位        |
| 15   | LimitP15   | Right dispensing Z positive limit | 右点胶Z正限位        |
| 16   | LimitP16   | null                              | null                 |
| 17   | LimitP17   | null                              | null                 |
| 18   | LimitP18   | null                              | null                 |

## LimitN

- 因为这部分绑定了硬件，所以这样设计

| ID   | Alarm code | Information  English              | Information  Chinese |
| ---- | ---------- | --------------------------------- | -------------------- |
| 1    | LimitN1    | Left dispensing X negative limit  | 左点胶X负限位        |
| 2    | LimitN2    | Left dispensing Y negative limit  | 左点胶Y负限位        |
| 3    | LimitN3    | Left dispensing Z negative limit  | 左点胶Z负限位        |
| 4    | LimitN4    | null                              | null                 |
| 5    | LimitN5    | null                              | null                 |
| 6    | LimitN6    | null                              | null                 |
| 7    | LimitN7    | Finger A motor negative limit     | 手指A电机负限位      |
| 8    | LimitN8    | Finger B motor negative limit     | 手指B电机负限位      |
| 9    | LimitN9    | Finger C motor negative limit     | 手指C电机负限位      |
| 10   | LimitN10   | Finger D motor negative limit     | 手指D电机负限位      |
| 11   | LimitN11   | null                              | null                 |
| 12   | LimitN12   | null                              | null                 |
| 13   | LimitN13   | Right dispensing X negative limit | 右点胶X负限位        |
| 14   | LimitN14   | Right dispensing Y negative limit | 右点胶Y负限位        |
| 15   | LimitN15   | Right dispensing Z negative limit | 右点胶Z负限位        |
| 16   | LimitN16   | null                              | null                 |
| 17   | LimitN17   | null                              | null                 |
| 18   | LimitN18   | null                              | null                 |



## Alm

- 因为这部分绑定了硬件，所以这样设计

| ID   | Alarm code | Information  English       | Information  Chinese |
| ---- | ---------- | -------------------------- | -------------------- |
| 1    | Alm1       | Left dispensing X failure  | 左点胶X故障          |
| 2    | Alm2       | Left dispensing Y failure  | 左点胶Y故障          |
| 3    | Alm3       | Left dispensing Z failure  | 左点胶Z故障          |
| 4    | Alm4       | null                       | null                 |
| 5    | Alm5       | null                       | null                 |
| 6    | Alm6       | null                       | null                 |
| 7    | Alm7       | Finger A motor failure     | 手指A电机故障        |
| 8    | Alm8       | Finger B motor failure     | 手指B电机故障        |
| 9    | Alm9       | Finger C motor failure     | 手指C电机故障        |
| 10   | Alm10      | Finger D motor failure     | 手指D电机故障        |
| 11   | Alm11      | null                       | null                 |
| 12   | Alm12      | null                       | null                 |
| 13   | Alm13      | Right dispensing X failure | 右点胶X故障          |
| 14   | Alm14      | Right dispensing Y failure | 右点胶Y故障          |
| 15   | Alm15      | Right dispensing Z fault   | 右点胶Z故障          |
| 16   | Alm16      | null                       | null                 |
| 17   | Alm17      | null                       | null                 |
| 18   | Alm18      | null                       | null                 |



## ALimitP

- 因为这部分绑定了硬件，所以这样设计

| ID   | Alarm code | Information  English                | Information  Chinese |
| ---- | ---------- | ----------------------------------- | -------------------- |
| 1    | ALimitP1   | Binding head Z motor positive limit | 绑头Z电机正限位      |
| 2    | ALimitP2   | Binding head Y motor positive limit | 绑头Y电机正限位      |
| 3    | ALimitP3   | null                                | null                 |
| 4    | ALimitP4   | null                                | null                 |
| 5    | ALimitP5   | Welding head A motor positive limit | 焊头A电机正限位      |
| 6    | ALimitP6   | Binding head X motor positive limit | 绑头X电机正限位      |
| 7    | ALimitP7   | Camera Y motor positive limit       | 相机Y电机正限位      |
| 8    | ALimitP8   | Cutter motor positive limit         | 切刀电机正限位       |
| 9    | ALimitP9   | null                                | null                 |
| 10   | ALimitP10  | null                                | null                 |



## ALimitN

- 因为这部分绑定了硬件，所以这样设计

| ID   | Alarm code | Information  English                | Information  Chinese |
| ---- | ---------- | ----------------------------------- | -------------------- |
| 1    | ALimitN1   | Binding head Z motor negative limit | 绑头Z电机负限位      |
| 2    | ALimitN2   | Binding head Y motor negative limit | 绑头Y电机负限位      |
| 3    | ALimitN3   | null                                | null                 |
| 4    | ALimitN4   | null                                | null                 |
| 5    | ALimitN5   | Welding head A motor negative limit | 焊头A电机负限位      |
| 6    | ALimitN6   | Binding head X motor negative limit | 绑头X电机负限位      |
| 7    | ALimitN7   | Camera Y motor negative limit       | 相机Y电机负限位      |
| 8    | ALimitN8   | Cutter motor negative limit         | 切刀电机负限位       |
| 9    | ALimitN9   | null                                | null                 |
| 10   | ALimitN10  | null                                | null                 |



## AAlm

- 因为这部分绑定了硬件，所以这样设计

| ID   | Alarm code | Information  English            | Information  Chinese |
| ---- | ---------- | ------------------------------- | -------------------- |
| 1    | AAlm1      | Head binding Z motor failure    | 绑头Z电机故障        |
| 2    | AAlm2      | Y motor failure of binding head | 绑头Y电机故障        |
| 3    | AAlm3      | null                            | null                 |
| 4    | AAlm4      | null                            | null                 |
| 5    | AAlm5      | Welding head A motor failure    | 焊头A电机故障        |
| 6    | AAlm6      | Head binding X motor failure    | 绑头X电机故障        |
| 7    | AAlm7      | Camera Y motor failure          | 相机Y电机故障        |
| 8    | AAlm8      | Cutter motor failure            | 切刀电机故障         |
| 9    | AAlm9      | Belt feeding motor failure      | 送条带电机故障       |
| 10   | AAlm10     | null                            | null                 |

