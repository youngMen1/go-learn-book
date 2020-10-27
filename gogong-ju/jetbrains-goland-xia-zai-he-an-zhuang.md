# 1.GoLand 工具下载安装和开发环境的下载与安装

## 1.1.JetBrains GoLand工具下载安装

Goland 是由 JetBrains 公司开发的一个新的商业 IDE，旨在为 Go 开发者提供的一个符合人体工程学的新的商业 IDE。Goland 整合了 IntelliJ 平台（一个用于 java 语言开发的集成环境，也可用于其他开发语言），提供了针对Go语言的编码辅助和工具集成。

大家可以从 Goland 的官网下载对应版本的 Goland 的安装包：（教程中使用的版本是 2019.2.3）

**官网下载地址：**[https://www.jetbrains.com/go/download/other.html；](https://www.jetbrains.com/go/download/other.html；)

![](/static/image/4-1910241H54A13.gif)

## 1.2.Golang开发环境的下载与安装

**Golang 官网国内镜像站点：**[https://golang.google.cn/dl/](https://golang.google.cn/dl/)

下图中的版本号可能并不是最新的，但总体来说安装教程是类似的。Go语言更新迭代比较快，推荐使用较新版本，体验最新特性：

![](/static/image/20200917185938391.png)

Windows平台和Mac平台推荐下载可执行文件版，Linux平台下载压缩文件版。

2020091719002888.png  
2020091719004298.png  
20200917190057710.png

**注意：**安装目录选择自己容易找到的目录即可。

**打开电脑CMD输入go version 查看是否安装成功：**  
20200917190115666.png

### 1.2.1. 配置GOPATH

`GOROOT`和`GOPATH`都是环境变量，其中`GOROOT`是我们安装go开发包的路径，而从Go 1.8版本开始，Go开发包在安装完成后会为`GOPATH`设置一个默认目录，参见下表。

**GOPATH在不同操作系统平台上的默认值**

| 平台 | GOPATH默认值 | 举例 |
| :--- | :--- | :--- |
| Windows | %USERPROFILE%/go | C:\Users\用户名\go |
| Unix | $HOME/go | /home/用户名/go |

这里我选择在电脑D盘下新建GOPATH：D:\GoLang\GoLang-workspace
20200917190203206.png


# 2.参考

[https://blog.csdn.net/weixin\_43591980/article/details/108650466](https://blog.csdn.net/weixin_43591980/article/details/108650466)  
Goland 2019下载和安装：[http://c.biancheng.net/view/6124.html](http://c.biancheng.net/view/6124.html)

