

## 数据类型
- Epj.Types  I1, I2, I4, I8, U1, U2, U4, U8, F4, F8, A, Bo, Bi, L, J, W

| ID   | C#.Type | Cimetrix.Value | Epj.Types | Description          |
| ---- | ------- | -------------- | --------- | -------------------- |
| 1    | string  | AValue         | A         | 单字节字符串         |
| 2    | bool    | BoValue        | Bo        | 布尔值               |
| 3    | byte[]  | BiValue        | Bi        | 二进制数据           |
| 4    | sbyte   | I1Value        | I1        | 1字节有符号整数       |
| 5    | short   | I2Value        | I2        | 2字节有符号整数       |
| 6    | int     | I4Value        | I4        | 4字节有符号整数       |
| 7    | long    | I8Value        | I8        | 8字节有符号整数       |
| 8    | byte    | U1Value        | U1        | 1字节无符号整数       |
| 9    | ushort  | U2Value        | U2        | 2字节无符号整数       |
| 10   | uint    | U4Value        | U4        | 4字节无符号整数       |
| 11   | ulong   | U8Value        | U8        | 8字节无符号整数       |
| 12   | float   | F4Value        | F4        | 4字节浮点数           |
| 13   | double  | F8Value        | F8        | 8字节浮点数           |
| 14   | List    | LValue         | L         | 列表值               |
| 15   | object  | JValue         | J         | JSON对象             |
| 16   | string  | WValue         | W         | 双字节字符串         |



![](https://easyimage.ghuang.top/i/2024/06/18/183029-1.webp)

## GPT 引导

- 帮我转换并翻译表格中的内容：
- 把下面的表格

```sh
| ID   | Name   | Description                | Units | VarType | ValType | EventID | Private | Persistant | Min  | Max  | Default   |
| ---- | ------ | -------------------------- | ----- | ------- | ------- | ------- | ------- | ---------- | ---- | ---- | --------- |
| 1    | AC8301 | Equipment ID               |       | EC      | A       |         | 0       | 0          |      |      | A 32767   |
| 2    | AC8302 | Model Number               |       | EC      | A       |         | 0       | 0          |      |      | A CB004   |
| 3    | AC8303 | Software Version           |       | EC      | A       |         | 0       | 0          |      |      | A V1.0    |
```

- 转换成 

```sh
[id=name, description, units, varType, valType, eventID, private, persistant, min, max, default, ]
8301=AC8301,Equipment ID,,EC,A,,0,0,,,A 32767,
8302=AC8302,Model Number,,EC,A,,0,0,,,A CB004,
8303=AC8303,Software Version,,EC,A,,0,0,,,A V1.0,
```

- 注意事项
- 1、输出内容去除掉  [id=name, description, units, varType, valType, eventID, private, persistant, min, max, default, ]

