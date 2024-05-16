# 06-FlipBondUl die bonding alarm code


| ID   | Name    | Description                                                 | setEventID | clearEventID | alarm code | Text                                    |
| ---- | ------- | ------------------------------------------------------------ | ---------- | ------------ | ---------- | --------------------------------------- |
| 1    | AC0601  | Prompt& input illegal parameter!                             | 1001       | 2001         | 6          | 提示&输入非法参数！                       |
| 2    | AC0602  | Please initialize before proceeding!                         | 1001       | 2001         | 6          | 请初始化后在操作！                         |
| 3    | AC0603  | Please stop before proceeding!                               | 1001       | 2001         | 6          | 请停止后在操作！                           |
| 4    | AC0604  | Prompt& welding head Z is not in the safe position           | 1001       | 2001         | 6          | 提示&焊头Z不在安全位                      |
| 5    | AC0605  | Obtaining welding image Mark point cross center abnormality& calibration failed! | 1001       | 2001         | 6          | 获取焊接图像Mark点十字中心异常&标定失败！ |
| 6    | AC0606  | Prompt& please pause before proceeding!                      | 1001       | 2001         | 6          | 提示&请暂停后在操作！                     |



```sh
8601=AC0601,Prompt& input illegal parameter!,Prompt& input illegal parameter!,1001,2001,6,
8602=AC0602,Please initialize before proceeding!,Please initialize before proceeding!,1001,2001,6,
8603=AC0603,Please stop before proceeding!,Please stop before proceeding!,1001,2001,6,
8604=AC0604,Prompt& welding head Z is not in the safe position,Prompt& welding head Z is not in the safe position,1001,2001,6,
8605=AC0605,Obtaining welding image Mark point cross center abnormality& calibration failed!,Obtaining welding image Mark point cross center abnormality& calibration failed!,1001,2001,6,
8606=AC0606,Prompt& please pause before proceeding!,Prompt& please pause before proceeding!,1001,2001,6,
```