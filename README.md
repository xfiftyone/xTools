# fofahelper
一个fofa搜索辅助小工具
## 配置文件 
修改fofa.exe同目录下fofa.ini配置文件，格式如下：
```
{
    "email": "xxx@mail.com",
    "key": "xxxxxxxxxxxxxxxxxxxxxxxx",
    "page": "1",
    "size": "100"
}
```  
## 效果 
![avatar](https://raw.githubusercontent.com/x51/fofahelper/main/FOFA.png)
## 待完善  
在前期打点阶段，使用fofa来做搜索的大概流程：  
fofa网页内搜索——>查看结果/翻页查看——>发现感兴趣目标——>浏览器打开/漏洞测试——>...  
1、搜索特定目标资产；  
2、搜索特定漏洞应用；  
其中第2点，部分漏洞探测可以用简单的HTTP请求完成，所以可在助手上增加漏洞探测插件，如下：  
