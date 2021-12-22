## ❤️ 说明
```
减少重复劳动，利用空间搜索引擎打点时的一个辅助性工具。
```
# xTools
A tool to quickly collect some information.
###  使用方法

首次使用，需要在程序配置界面配置好各平台认证信息：

![image](https://user-images.githubusercontent.com/45651912/147092506-87e4b46e-4286-4226-9337-f6a5f0f8bb9d.png)
  
###  数据提取（✔️）

目前用到的是FOFA&Hunter，详细语法请参考官方页面：

```
domain=github.com&&port=80
```
![image](https://user-images.githubusercontent.com/45651912/147092665-7f6dfc8f-1325-4740-a364-382a6d039ca6.png)
 
 Hunter查询会将消耗积分的信息输出在状态栏：
 
 ![image](https://user-images.githubusercontent.com/45651912/147092824-d529925f-5611-45de-ae8e-a205bd6f75cd.png)

### 访问Web（✔️）

双击即可在浏览器直接打开（默认以http协议），或者右键访问web

#### 二次探测

右键可以对单个IP进行查询，或者该IP所在C段信息查询：

![image](https://user-images.githubusercontent.com/45651912/147093207-c34b40a8-39cd-4b33-9b9f-dc75c26815c2.png)
### Nuclei探测

得益于Nuclei的高度可定制化，我们可以将自定义的POC放置到到程序templates目录下，程序会自动识别分类名并添加至右键菜单，并读取各分类目录下
的所有POC信息，可以很方便的右键调起扫描（请忽略POC命名信息，此处仅做演示截图）

![image](https://user-images.githubusercontent.com/45651912/147093914-23feed79-fd89-4315-9f42-351d897ce832.png)

选择并点击需要探测的POC名称即可调起nuclei程序进行扫描，点击分类菜单会对该目录下所有POC进行探测：

![image](https://user-images.githubusercontent.com/45651912/147099691-fbeda6d1-ffe5-4ebd-8b6b-fce398bf72c0.png)

### 结果导出（✔️）

右键导出结果为cvs格式，导出结果保存在程序主目录。

![image](https://user-images.githubusercontent.com/45651912/147097903-47eb3fa2-3d9d-4754-afef-2db8097c30d8.png)

### POC编写

请移步https://nuclei.projectdiscovery.io/templating-guide/#template-details

### TODO

增加常用exploit如XX OA等；
增加其他空间搜索引擎；
