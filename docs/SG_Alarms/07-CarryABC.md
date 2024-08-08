# 07-CarryABC alarm code

| ID   | Name   | Description                                                  | setEventID | clearEventID | alarm code | Text                                 |
| ---- | ------ | ------------------------------------------------------------ | ---------- | ------------ | ---------- | ------------------------------------ |
| 1    | AC0701 | Please initialize the over-chip station before starting it!  | 1001       | 2001         | 6          | 过片工位请初始化后再启动！           |
| 2    | AC0702 | Operation failed;please pause and then operate!              | 1001       | 2001         | 6          | 操作失败，请暂停后在操作！           |
| 3    | AC0703 | Please initialize it before operation!                       | 1001       | 2001         | 6          | 请初始化后再操作！                   |
| 4    | AC0704 | No frames were detected at the track entrance!               | 1001       | 2001         | 6          | 轨道入口未检测到框架！               |
| 5    | AC0705 | Failed to capture frame edge!                                | 1001       | 2001         | 6          | 捕获框架边缘失败！                   |
| 6    | AC0706 | Failure of the vacuum furnace to take the frame!             | 1001       | 2001         | 6          | 真空炉取框架失败！                   |
| 7    | AC0707 | Please pause before operating                                | 1001       | 2001         | 6          | 请暂停后再操作                       |
| 8    | AC0708 | Please reset and clear the track again                       | 1001       | 2001         | 6          | 请复位后再清空轨道                   |
| 9    | AC0709 | Failed to return to the origin over slice A!                 | 1001       | 2001         | 6          | 过片A回原点失败！                    |
| 10   | AC0710 | Failed to return to the origin over slice B!                 | 1001       | 2001         | 6          | 过片B回原点失败！                    |
| 11   | AC0711 | Failed to return to the origin over slice C!                 | 1001       | 2001         | 6          | 过片C回原点失败！                    |
| 12   | AC0712 | Failed to return to the origin over slice D!                 | 1001       | 2001         | 6          | 过片D回原点失败！                    |
| 13   | AC0713 | Automatic operation of the cross-piece station;Please stop before operating! | 1001       | 2001         | 6          | 过片工位自动运行中，请停止后在操作！ |
| 14   | AC0714 | Please initialize it and then operate it!                    | 1001       | 2001         | 6          | 请初始化后在操作！                   |
| 15   | AC0715 | Please reset before operation                                | 1001       | 2001         | 6          | 请复位后再操作                       |
| 16   | AC0716 | Teach frame edge failure;no signal captured!                 | 1001       | 2001         | 6          | 教导框架边缘失败，未捕获到信号！     |



```sh
8701=AC0701,Please initialize the over-chip station before starting it!,Please initialize the over-chip station before starting it!,1001,2001,6,
8702=AC0702,Operation failed;please pause and then operate!,Operation failed;please pause and then operate!,1001,2001,6,
8703=AC0703,Please initialize it before operation!,Please initialize it before operation!,1001,2001,6,
8704=AC0704,No frames were detected at the track entrance!,No frames were detected at the track entrance!,1001,2001,6,
8705=AC0705,Failed to capture frame edge!,Failed to capture frame edge!,1001,2001,6,
8706=AC0706,Failure of the vacuum furnace to take the frame!,Failure of the vacuum furnace to take the frame!,1001,2001,6,
8707=AC0707,Please pause before operating,Please pause before operating,1001,2001,6,
8708=AC0708,Please reset and clear the track again,Please reset and clear the track again,1001,2001,6,
8709=AC0709,Failed to return to the origin over slice A!,Failed to return to the origin over slice A!,1001,2001,6,
8710=AC0710,Failed to return to the origin over slice B!,Failed to return to the origin over slice B!,1001,2001,6,
8711=AC0711,Failed to return to the origin over slice C!,Failed to return to the origin over slice C!,1001,2001,6,
8712=AC0712,Failed to return to the origin over slice D!,Failed to return to the origin over slice D!,1001,2001,6,
8713=AC0713,Automatic operation of the cross-piece station;Please stop before operating!,Automatic operation of the cross-piece station;Please stop before operating!,1001,2001,6,
8714=AC0714,Please initialize it and then operate it!,Please initialize it and then operate it!,1001,2001,6,
8715=AC0715,Please reset before operation,Please reset before operation,1001,2001,6,
8716=AC0716,Teach frame edge failure;no signal captured!,Teach frame edge failure;no signal captured!,1001,2001,6,

```