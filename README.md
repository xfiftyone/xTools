<h1 align="center">
xTools
</h1>
<h4 align="center">减少重复劳动，利用空间搜索引擎打点时的一个辅助性工具🚀</h4>
<p align="center">
<a href="https://github.com/xfiftyone/xTools/issues"><img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat"></a>
<a href="https://github.com/xfiftyone/xTools/releases"><img src="https://img.shields.io/github/release/xfiftyone/xTools"></a>
</p>

#  🎉开始使用

首次使用，需要在程序配置界面配置好各平台认证信息，点击确定后会在程序目录生成`xTools.exe.config`，此文件保存程序所有配置信息。

![image](https://user-images.githubusercontent.com/45651912/147092506-87e4b46e-4286-4226-9337-f6a5f0f8bb9d.png)
  
## 🔍数据提取

目前用到的是 `FOFA` & `Hunter`，详细语法请参考官方页面：  

[FOFA](https://fofa.so/)  
[Hunter](https://hunter.qianxin.com/)

example：

```
domain=github.com&&port=80
```
![image](https://user-images.githubusercontent.com/45651912/147092665-7f6dfc8f-1325-4740-a364-382a6d039ca6.png)
 
 Hunter查询会将消耗积分的信息输出在状态栏：
 
 ![image](https://user-images.githubusercontent.com/45651912/147092824-d529925f-5611-45de-ae8e-a205bd6f75cd.png)

## 访问Web

双击即可在浏览器直接打开（默认以http协议），或者右键访问web

## 二次探测

右键可以对单个IP进行查询，或者该IP所在C段信息查询：

![image](https://user-images.githubusercontent.com/45651912/147093207-c34b40a8-39cd-4b33-9b9f-dc75c26815c2.png)  

## ✨Nmap端口扫描

如果需要调用Nmap，需要首先从[Nmap主页](https://nmap.org/download.html)下载非安装版`Latest stable command-line zipfile`到程序`extra`目录下对应文件夹。  

可在`程序配置`界面——`Nmap配置`处，填入自定义`Nmap`命令，代码处理逻辑如下：  

```
nmap.exe {args} {ip} -vv
``` 
如果默认不设置，则使用初始扫描参数`nmap.exe -sS -n -T3 {ip} -vv`，**建议配置自定义参数**。

![image](https://user-images.githubusercontent.com/45651912/147377162-346c1512-6b73-4e06-83d1-3c442fe4bcbe.png)

调用`Nmap`扫描效果：  

![image](https://user-images.githubusercontent.com/45651912/147377174-375f244f-8eba-46d4-a374-464ff378b69f.png)


## ✨Nuclei探测
如果需要调用Nuclei，需要首先从[Nuclei官方仓库](https://github.com/projectdiscovery/nuclei)下载`nuclei.exe`到程序`extra`目录下对应文件夹。  

得益于Nuclei的高度可定制化，我们可以将自定义的POC放置到到程序templates目录下，**程序会自动识别分类名并添加至右键菜单，并读取各分类目录下的所有POC信息**，可以很方便的右键调起扫描（请忽略POC命名信息，此处仅做演示截图）

![image](https://user-images.githubusercontent.com/45651912/147093914-23feed79-fd89-4315-9f42-351d897ce832.png)

选择并点击需要探测的POC名称即可调起nuclei程序进行扫描，**点击分类菜单会对该目录下所有POC进行探测**：

![image](https://user-images.githubusercontent.com/45651912/147099691-fbeda6d1-ffe5-4ebd-8b6b-fce398bf72c0.png)

## 结果导出

右键导出结果为csv格式，导出结果保存在程序主目录。

![image](https://user-images.githubusercontent.com/45651912/147102388-b633dfe1-a2ac-44e0-a126-7662ac4e2e63.png)


## POC编写

请移步https://nuclei.projectdiscovery.io/templating-guide/#template-details

## ⚗️TODO 

增加漏洞利用模块；  
增加其他空间搜索引擎；
