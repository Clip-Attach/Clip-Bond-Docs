# 19-WaferTableUl die bonding alarm code

| ID   | Name   | description                             | setEventID | clearEventID | alarm code | Text                                                         |
| ---- | ------ | --------------------------------------- | ---------- | ------------ | ---------- | ------------------------------------------------------------ |
| 1    | AC1901 | 参数设定非合法字符！                   | 1001       | 2001         | 6          | Illegal character in parameter setting!                      |
| 2    | AC1902 | 顶针不在原点                           | 1001       | 2001         | 6          | Needle is not at the origin                                  |
| 3    | AC1903 | 请停止后在操作！                       | 1001       | 2001         | 6          | Please stop before proceeding!                               |
| 4    | AC1904 | 提示&请暂停后在操作！                 | 1001       | 2001         | 6          | Prompt&please pause before proceeding!                      |
| 5    | AC1905 | 底座气缸不在高位！                   | 1001       | 2001         | 6          | The base cylinder is not in high position!                   |
| 6    | AC1906 | 推顶气缸不在低位！                   | 1001       | 2001         | 6          | The pushing cylinder is not in the low position!             |
| 7    | AC1907 | 扩片不在低位！                       | 1001       | 2001         | 6          | Expansion not in low position!                               |
| 8    | AC1908 | 请初始化后在操作！                   | 1001       | 2001         | 6          | Please initialize before proceeding!                         |
| 9    | AC1909 | 获取晶圆片图像Mark点十字中心异常&标定失败！ | 1001       | 2001         | 6          | Abnormal Mark point cross center in obtaining wafer image&calibration failed! |
| 10   | AC1910 | 获取左点胶图像Mark点十字中心异常&标定失败！ | 1001       | 2001         | 6          | The center of the Mark dot cross in obtaining the left glue image is abnormal&calibration failed! |
| 11   | AC1911 | 获取焊头图像Mark点十字中心异常&标定失败！   | 1001       | 2001         | 6          | Obtaining welding head image Mark point cross center abnormality&calibration failed! |
| 12   | AC1912 | 晶圆盘回原点失败！                   | 1001       | 2001         | 6          | Failed to return the WaferTable to the original point!       |
| 13   | AC1913 | 晶圆环中心教导失败！                 | 1001       | 2001         | 6          | The calibration of the WaferTable center is completed!       |
| 14   | AC1914 | 夹角超出±10°&标定失败！             | 1001       | 2001         | 6          | The included angle exceeds ± 10 °&calibration failed!       |



```sh
9901=AC1901,Illegal character in parameter setting!,Illegal character in parameter setting!,1001,2001,6,
9902=AC1902,Needle is not at the origin,Needle is not at the origin,1001,2001,6,
9903=AC1903,Please stop before proceeding!,Please stop before proceeding!,1001,2001,6,
9904=AC1904,Prompt&please pause before proceeding!,Prompt&please pause before proceeding!,1001,2001,6,
9905=AC1905,The base cylinder is not in high position!,The base cylinder is not in high position!,1001,2001,6,
9906=AC1906,The pushing cylinder is not in the low position!,The pushing cylinder is not in the low position!,1001,2001,6,
9907=AC1907,Expansion not in low position!,Expansion not in low position!,1001,2001,6,
9908=AC1908,Please initialize before proceeding!,Please initialize before proceeding!,1001,2001,6,
9909=AC1909,Abnormal Mark point cross center in obtaining wafer image&calibration failed!,Abnormal Mark point cross center in obtaining wafer image&calibration failed!,1001,2001,6,
9910=AC1910,The center of the Mark dot cross in obtaining the left glue image is abnormal&calibration failed!,The center of the Mark dot cross in obtaining the left glue image is abnormal&calibration failed!,1001,2001,6,
9911=AC1911,Obtaining welding head image Mark point cross center abnormality&calibration failed!,Obtaining welding head image Mark point cross center abnormality&calibration failed!,1001,2001,6,
9912=AC1912,Failed to return the WaferTable to the original point!,Failed to return the WaferTable to the original point!,1001,2001,6,
9913=AC1913,The calibration of the WaferTable center is completed!,The calibration of the WaferTable center is completed!,1001,2001,6,
9914=AC1914,The included angle exceeds ± 10 °&calibration failed!,The included angle exceeds ± 10 °&calibration failed!,1001,2001,6,
```