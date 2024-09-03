

![](https://easyimage.ghuang.top/i/2024/09/03/145527-1.webp)

### 一、Install CIMConnect

![](https://easyimage.ghuang.top/i/2024/09/03/145627-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/145648-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/145701-1.webp)

- 选择 License

![](https://easyimage.ghuang.top/i/2024/09/03/145745-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/145801-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/145819-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/145834-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/145900-1.webp)


### 二、Install EquipmentTest

![](https://easyimage.ghuang.top/i/2024/09/03/145935-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/145958-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/150016-1.webp)

- 选择 License

![](https://easyimage.ghuang.top/i/2024/09/03/150059-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/150114-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/150127-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/150139-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/150215-1.webp)

### 三、Install ALPS

#### 1、先安装环境
- 安裝ALPS之前請先在Windows將.net Framework 3.5 / IIS / MSMQ這三個功能給enable.

![](https://easyimage.ghuang.top/i/2024/09/03/151155-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/151231-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/151358-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/151458-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/151722-1.webp)

#### 2、安装软件

- 解压

![](https://easyimage.ghuang.top/i/2024/09/03/150309-1.webp)

- 执行 `setup`, 记得关闭杀毒软件

![](https://easyimage.ghuang.top/i/2024/09/03/150554-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/150659-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/150724-1.webp)

- 一定要选择 `ALPS Server`

![](https://easyimage.ghuang.top/i/2024/09/03/150741-1.webp)


- 出现这个说明。 `1、先安装环境` 没安装好

![](https://easyimage.ghuang.top/i/2024/09/03/150842-1.webp)

- 继续安装

![](https://easyimage.ghuang.top/i/2024/09/03/151817-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/151839-1.webp)

- 点击下一步，安装数据库需要一会

![](https://easyimage.ghuang.top/i/2024/09/03/151858-1.webp)

- 点击下一步，自动重启电脑

![](https://easyimage.ghuang.top/i/2024/09/03/152350-1.webp)


#### 3、导入License

- 打开文件夹 `C:\Program Files (x86)\PDF Solutions\ALPS NET\RLM`

![](https://easyimage.ghuang.top/i/2024/09/03/153350-1.webp)


- 导入License

![](https://easyimage.ghuang.top/i/2024/09/03/153443-1.webp)


### 四、Test Demo

- E142EquipmentSimulation_Strip

- 1、将 `E142EquipmentSimulation.epj` 文件放到指定文件夹

```yaml
C:\E142EquipmentSimulation_Strip\E142EquipmentSimulation.epj
↓
C:\CIMConnectProjects\Equipment1\Projects\E142EquipmentSimulation.epj
```
![](https://easyimage.ghuang.top/i/2024/09/03/155200-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/154144-1.webp)


- 2、运行程序

![](https://easyimage.ghuang.top/i/2024/09/03/154231-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/154425-1.webp)

- 3、打开 `CimetrixEquipmentTest`

![](https://easyimage.ghuang.top/i/2024/09/03/154329-1.webp)

- 4、选择 `CIM142.xml`

![](https://easyimage.ghuang.top/i/2024/09/03/154459-1.webp)

- 5、连接
  
![](https://easyimage.ghuang.top/i/2024/09/03/154548-1.webp)

- 6、将 Substrate ID:的内容 从 `ToSiPStrip_ALPS` 修改为 `ToSiPStrip`

![](https://easyimage.ghuang.top/i/2024/09/03/154731-1.webp)

- 7、下载 `Map`

![](https://easyimage.ghuang.top/i/2024/09/03/154800-1.webp)

- 8、发送 `Map`

![](https://easyimage.ghuang.top/i/2024/09/03/154838-1.webp)

![](https://easyimage.ghuang.top/i/2024/09/03/154947-1.webp)

- 9、UI 显示最终结果

![](https://easyimage.ghuang.top/i/2024/09/03/155047-1.webp)