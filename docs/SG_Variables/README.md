
![](https://easyimage.ghuang.top/i/2024/06/09/184907-1.webp)



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

