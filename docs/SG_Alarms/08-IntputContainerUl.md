# 08-IntputContainerUl die bonding alarm code

| ID   | Name   | description                             | setEventID | clearEventID | alarm code | Text                                                         |
| ---- | ------ | --------------------------------------- | ---------- | ------------ | ---------- | ------------------------------------------------------------ |
| 1    | AC0801 | 复位出料盒工位后&在操作！             | 1001       | 2001         | 6          | After resetting the discharge box station& start the operation! |
| 2    | AC0802 | 进料盒出口检测异常                     | 1001       | 2001         | 6          | Abnormal detection at the outlet of input box                |
| 3    | AC0803 | 输入非法参数！                         | 1001       | 2001         | 6          | Illegal parameter entered!                                   |
| 4    | AC0804 | 请初始化后在操作！                     | 1001       | 2001         | 6          | Please operate after initialization!                         |
| 5    | AC0805 | 请停止后在操作！                       | 1001       | 2001         | 6          | Please stop before proceeding!                               |
| 6    | AC0806 | 入料X轴不在原点                        | 1001       | 2001         | 6          | Input x-axis is not at the origin                            |
| 7    | AC0807 | 入料Z轴不在原点                        | 1001       | 2001         | 6          | Input Z-axis is not at the origin                            |
| 8    | AC0808 | 提示&请暂停后在操作！                 | 1001       | 2001         | 6          | Prompt& please pause before proceeding!                      |



```sh
8801=AC0801,Reset the discharge box station before operating!,After resetting the discharge box station& start the operation!,1001,2001,6,
8802=AC0802,Abnormal detection at the outlet of input box,Abnormal detection at the outlet of input box,1001,2001,6,
8803=AC0803,Illegal parameter entered!,Illegal parameter entered!,1001,2001,6,
8804=AC0804,Please operate after initialization!,Please operate after initialization!,1001,2001,6,
8805=AC0805,Please stop before proceeding!,Please stop before proceeding!,1001,2001,6,
8806=AC0806,Input x-axis is not at the origin,Input x-axis is not at the origin,1001,2001,6,
8807=AC0807,Input Z-axis is not at the origin,Input Z-axis is not at the origin,1001,2001,6,
8808=AC0808,Prompt& please pause before proceeding!,Prompt& please pause before proceeding!,1001,2001,6,
```