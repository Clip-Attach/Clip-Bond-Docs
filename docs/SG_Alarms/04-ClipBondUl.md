# 04-ClipBondUl die bonding alarm code

| ID   | Name    | Description                                                 | setEventID | clearEventID | alarm code | Text                                    |
| ---- | ------- | ------------------------------------------------------------ | ---------- | ------------ | ---------- | --------------------------------------- |
| 1    | AC0401  | Prompt& input illegal parameter!                             | 1001       | 2001         | 6          | 提示&输入非法参数！                   |
| 2    | AC0402  | Prompt& the overall modification has set illegal parameters! | 1001       | 2001         | 6          | 提示&整体修改设定了非法参数！         |
| 3    | AC0403  | Please initialize before proceeding!                         | 1001       | 2001         | 6          | 请初始化后在操作！                     |
| 4    | AC0404  | Please stop before proceeding!                               | 1001       | 2001         | 6          | 请停止后在操作！                       |
| 5    | AC0405  | Please select a coordinate point!                            | 1001       | 2001         | 6          | 请选择坐标点！                         |
| 6    | AC0406  | Camera Y motor movement timeout!                             | 1001       | 2001         | 6          | 相机Y电机运动超时！                   |
| 7    | AC0407  | Prompt& welding head Z is not in the safe position           | 1001       | 2001         | 6          | 提示&焊头Z不在安全位                |
| 8    | AC0408  | Obtaining welding image Mark point cross center abnormality& calibration failed! | 1001       | 2001         | 6          | 获取焊接图像Mark点十字中心异常&标定失败！ |
| 9    | AC0409  | The welding head is not in the force measuring position!     | 1001       | 2001         | 6          | 焊头未在测力位置！                   |
| 10   | AC0410  | Welding head Z return to origin failed!                      | 1001       | 2001         | 6          | 焊头Z回原点失败！                     |
| 11   | AC0411  | Please pause before proceeding!                              | 1001       | 2001         | 6          | 请暂停后在操作！                     |
| 12   | AC0412  | Prompt& please pause before proceeding!                      | 1001       | 2001         | 6          | 提示&请暂停后在操作！               |
| 13   | AC0413  | The angle between the welding head and the camera Y exceeds the specified range (87 ° -93 °): Binding the welding head to the welding camera failed! | 1001       | 2001         | 6          | 焊头与相机Y夹角超出了规定范围(87°-93°)：绑定焊头与焊接相机失败！ |
| 14   | AC0414  | The first point of the welding head is larger than 65mm!     | 1001       | 2001         | 6          | 焊头第一点位置大于了65mm！           |



```sh
8401=AC0401,Prompt& input illegal parameter!,Prompt& input illegal parameter!,1001,2001,6,
8402=AC0402,Prompt& the overall modification has set illegal parameters!,Prompt& the overall modification has set illegal parameters!,1001,2001,6,
8403=AC0403,Please initialize before proceeding!,Please initialize before proceeding!,1001,2001,6,
8404=AC0404,Please stop before proceeding!,Please stop before proceeding!,1001,2001,6,
8405=AC0405,Please select a coordinate point!,Please select a coordinate point!,1001,2001,6,
8406=AC0406,Camera Y motor movement timeout!,Camera Y motor movement timeout!,1001,2001,6,
8407=AC0407,Prompt& welding head Z is not in the safe position,Prompt& welding head Z is not in the safe position,1001,2001,6,
8408=AC0408,Obtaining welding image Mark point cross center abnormality& calibration failed!,Obtaining welding image Mark point cross center abnormality& calibration failed!,1001,2001,6,
8409=AC0409,The welding head is not in the force measuring position!,The welding head is not in the force measuring position!,1001,2001,6,
8410=AC0410,Welding head Z return to origin failed!,Welding head Z return to origin failed!,1001,2001,6,
8411=AC0411,Please pause before proceeding!,Please pause before proceeding!,1001,2001,6,
8412=AC0412,Prompt& please pause before proceeding!,Prompt& please pause before proceeding!,1001,2001,6,
8413=AC0413,The angle between the welding head and the camera Y exceeds the specified range (87 ° -93 °): Binding the welding head to the welding camera failed!,The angle between the welding head and the camera Y exceeds the specified range (87 ° -93 °): Binding the welding head to the welding camera failed!,1001,2001,6,
8414=AC0414,The first point of the welding head is larger than 65mm!,The first point of the welding head is larger than 65mm!,1001,2001,6,
```