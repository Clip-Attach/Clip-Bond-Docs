# Welcome to MkDocs

## Last modification time: 2024-05-16


## Die Bond

| Camera  name     | Alias            | resolution  um/pix |
| ---------------- | ---------------- | ------------------ |
| dispense  camera | Glue camera      | 13.7               |
| pick camera      | wafer camera     | 20.3               |
| bond camera      | Bond head camera | 8                  |

## Clip Bond

| Camera  name     | Alias            | resolution  um/pix |
| ---------------- | ---------------- | ------------------ |
| dispense  camera | Glue camera      | 13.7               |
| uplook camera    | uplook camera    | 20.3               |
| bond camera      | Bond head camera | 14.3               |


## 任务

```yaml
1、远程控制
S2
F41 42
S7

比如:
工艺程序上传下载功能
远程锁定机器
机台启动

2、map映射
①、晶圆
map S12
waf  E5 S12

②、条带
str E142
str G84   E142


3、工艺信息，变量，事件。软件回调
生产信息

①报警 （host 软件回调）
报错数量，关键，日志
机器报警 回调 到 host 软件 

②常量 （host 软件回调）
常量：机器可以远程修改的 
工艺信息

③变量 （host 软件回调）
变量：机器不能远程修改的
工艺信息

④事件 （host 回调）
远程锁定机器
机台启动


4、了解 E30 
①、添加E30 基础的 机台的工艺状态
②、了解  E142 ，E30 
```

![](https://easyimage1.ghuang.top/i/2024/04/23/004531-1.webp)