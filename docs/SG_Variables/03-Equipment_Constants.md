# 03-Equipment Constants

| ID   | Name   | Description                | Units | VarType | ValType | EventID | Private | Persistant | Min  | Max  | Default   |
| ---- | ------ | -------------------------- | ----- | ------- | ------- | ------- | ------- | ---------- | ---- | ---- | --------- |
| 1    | AC8301 | Equipment ID               |       | EC      | A       |         | 0       | 0          |      |      | A 32767   |
| 2    | AC8302 | Model Number               |       | EC      | A       |         | 0       | 0          |      |      | A CB004   |
| 3    | AC8303 | Software Version           |       | EC      | A       |         | 0       | 0          |      |      | A V1.0    |
| 4    | AC8304 | Process Recipes            |       | EC      | A       |         | 0       | 0          |      |      | A TO220   |
| 5    | AC8305 | Communication Parameters   |       | EC      | A       |         | 0       | 0          |      |      | A 0.0.0.0 |
| 6    | AC8306 | Part No                    |       | EC      | A       |         | 0       | 0          |      |      | A         |
| 7    | AC8307 | Camera resolution:dispense |       | EC      | A       |         | 0       | 0          |      |      | A 13.7    |
| 8    | AC8308 | Camera resolution: uplook  |       | EC      | A       |         | 0       | 0          |      |      | A 20.3    |
| 9    | AC8309 | Camera resolution: bond    |       | EC      | A       |         | 0       | 0          |      |      | A 14.3    |
| 10   | AC8310 | Production Statistics      |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 11   | AC8311 | Total cutter count         |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 12   | AC8312 | Scrap Knife Count          |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 13   | AC8313 | Nozzle Count               |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 14   | AC8314 | Upper cutter count         |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 15   | AC8315 | Lower cutter count         |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 16   | AC8316 | Head binding UPH           |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 17   | AC8317 | Left Dispensing UPH        |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 18   | AC8318 | Right Dispensing UPH       |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 19   | AC8319 | UPH                        |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 20   | AC8320 | Head binding CT (ms)       |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 21   | AC8321 | Left glue CT(ms)           |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |
| 22   | AC8322 | Right dispensing CT(ms)    |       | EC      | I8      |         | 0       | 0          |      |      | I8 0      |


```sh
8301=AC8301,Equipment ID,,EC,A,,0,0,,,A 32767,
8302=AC8302,Model Number,,EC,A,,0,0,,,A CB004,
8303=AC8303,Software Version,,EC,A,,0,0,,,A V1.0,
8304=AC8304,Process Recipes,,EC,A,,0,0,,,A TO220,
8305=AC8305,Communication Parameters,,EC,A,,0,0,,,A 0.0.0.0,
8306=AC8306,Part No,,EC,A,,0,0,,,A,
8307=AC8307,Camera resolution:dispense,,EC,A,,0,0,,,A 13.7,
8308=AC8308,Camera resolution: uplook,,EC,A,,0,0,,,A 20.3,
8309=AC8309,Camera resolution: bond,,EC,A,,0,0,,,A 14.3,
8310=AC8310,Production Statistics,,EC,I8,,0,0,,,I8 0,
8311=AC8311,Total cutter count,,EC,I8,,0,0,,,I8 0,
8312=AC8312,Scrap Knife Count,,EC,I8,,0,0,,,I8 0,
8313=AC8313,Nozzle Count,,EC,I8,,0,0,,,I8 0,
8314=AC8314,Upper cutter count,,EC,I8,,0,0,,,I8 0,
8315=AC8315,Lower cutter count,,EC,I8,,0,0,,,I8 0,
8316=AC8316,Head binding UPH,,EC,I8,,0,0,,,I8 0,
8317=AC8317,Left Dispensing UPH,,EC,I8,,0,0,,,I8 0,
8318=AC8318,Right Dispensing UPH,,EC,I8,,0,0,,,I8 0,
8319=AC8319,UPH,,EC,I8,,0,0,,,I8 0,
8320=AC8320,Head binding CT (ms),,EC,I8,,0,0,,,I8 0,
8321=AC8321,Left glue CT(ms),,EC,I8,,0,0,,,I8 0,
8322=AC8322,Right dispensing CT(ms),,EC,I8,,0,0,,,I8 0,
```


# 3.Variables

在SECS/GEM（SEMI Equipment Communications Standard/Generic Equipment Model）协议中，设备常量（Equipment Constants, EC）是设备特定的参数和设置，它们通常不经常更改，并且在设备操作期间保持相对恒定。这些常量对设备的配置和操作非常重要，通常在设备初始化和设置时定义。以下是一些常见的设备常量：

1. **设备ID（Equipment ID）**：
   - 用于唯一标识设备的ID号。

2. **设备型号（Model Number）**：
   - 设备的型号信息。

3. **软件版本（Software Version）**：
   - 设备运行的软件版本号。

4. **硬件配置（Hardware Configuration）**：
   - 设备的硬件配置细节，比如安装的模块或组件信息。

5. **校准参数（Calibration Parameters）**：
   - 用于校准设备的参数，比如传感器的校准数据。

6. **工艺配方（Process Recipes）**：
   - 设备运行的工艺配方信息，包括工艺步骤和参数。

7. **通信参数（Communication Parameters）**：
   - 设备通信设置，比如网络配置、端口号等。

8. **安全设置（Safety Settings）**：
   - 设备的安全设置，包括紧急停止参数、安全联锁等。

9. **维护周期（Maintenance Intervals）**：
   - 设备的维护和保养周期信息。

10. **生产统计（Production Statistics）**：
    - 设备的生产统计数据，比如运行时间、产量等。

这些设备常量在SECS/GEM通信中通常通过S2（设备管理）消息来获取和设置，例如S2F13（Equipment Constant Request）和S2F15（Equipment Constant Update）。这些常量对设备的正常运行和管理至关重要。

