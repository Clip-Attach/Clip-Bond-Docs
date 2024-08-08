# 02-CCD die bonding alarm code(OK)

| ID   | Name   | description                                                  | setEventID | clearEventID | alarm code | Text                                 |
| ---- | ------ | ------------------------------------------------------------ | ---------- | ------------ | ---------- | ------------------------------------ |
| 1    | AC0201 | Place camera calibration reading Mark failed!                | 1001       | 2001         | 6          | Place相机标定读取Mark失败！          |
| 2    | AC0202 | Place camera calibration failed!                             | 1001       | 2001         | 6          | Place相机标定失败！                  |
| 3    | AC0203 | The search area of the column is unreasonable and must be higher than the width | 1001       | 2001         | 6          | 列的搜索区域不合理；必须高度大于宽度 |
| 4    | AC0204 | The search area of the row is unreasonable and must be wider than the height | 1001       | 2001         | 6          | 行的搜索区域不合理；必须宽度大于高度 |
| 5    | AC0205 | Ink dot search area exceeds the limit area!                  | 1001       | 2001         | 6          | 墨点搜索区域超出限制区域！           |
| 6    | AC0206 | Failed to read the glue volume detection parameter!          | 1001       | 2001         | 6          | 读取胶量检测参数失败！               |
| 7    | AC0207 | Failed to save glue volume detection parameters!             | 1001       | 2001         | 6          | 保存胶量检测参数失败！               |
| 8    | AC0208 | Failed to create a template!                                 | 1001       | 2001         | 6          | 创建模板失败！                       |
| 9    | AC0209 | Failed to read detection parameters!                         | 1001       | 2001         | 6          | 读取检测参数失败!                    |
| 10   | AC0210 | Failed to save detection parameters!                         | 1001       | 2001         | 6          | 保存检测参数失败!                    |
| 11   | AC0211 | The match value cannot be less than 30!                      | 1001       | 2001         | 6          | 匹配值不能小于30！                   |
| 12   | AC0212 | Enter an illegal parameter!                                  | 1001       | 2001         | 6          | 输入非法参数！                       |
| 13   | AC0213 | Parameter read failed!                                       | 1001       | 2001         | 6          | 参数读取失败！                       |
| 14   | AC0214 | Parameter save failed!                                       | 1001       | 2001         | 6          | 参数保存失败！                       |
| 15   | AC0215 | Failed to read detection parameters!                         | 1001       | 2001         | 6          | 读取检测参数失败！                   |



```sh
8201=AC0201,Place camera calibration reading Mark failed!,Place camera calibration reading Mark failed!,1001,2001,6,
8202=AC0202,Place camera calibration failed!,Place camera calibration failed!,1001,2001,6,
8203=AC0203,The search area of the column is unreasonable and must be higher than the width,The search area of the column is unreasonable and must be higher than the width,1001,2001,6,
8204=AC0204,The search area of the row is unreasonable and must be wider than the height,The search area of the row is unreasonable and must be wider than the height,1001,2001,6,
8205=AC0205,Ink dot search area exceeds the limit area!,Ink dot search area exceeds the limit area!,1001,2001,6,
8206=AC0206,Failed to read the glue volume detection parameter!,Failed to read the glue volume detection parameter!,1001,2001,6,
8207=AC0207,Failed to save glue volume detection parameters!,Failed to save glue volume detection parameters!,1001,2001,6,
8208=AC0208,Failed to create a template!,Failed to create a template!,1001,2001,6,
8209=AC0209,Failed to read detection parameters!,Failed to read detection parameters!,1001,2001,6,
8210=AC0210,Failed to save detection parameters!,Failed to save detection parameters!,1001,2001,6,
8211=AC0211,The match value cannot be less than 30!,The match value cannot be less than 30!,1001,2001,6,
8212=AC0212,Enter an illegal parameter!,Enter an illegal parameter!,1001,2001,6,
8213=AC0213,Parameter read failed!,Parameter read failed!,1001,2001,6,
8214=AC0214,Parameter save failed!,Parameter save failed!,1001,2001,6,
8215=AC0215,Failed to read detection parameters!,Failed to read detection parameters!,1001,2001,6,

```