# Go语言环境安装

Go 语言支持以下系统：

* Linux
* FreeBSD
* Mac OS X（也称为 Darwin）
* Windows

安装包下载地址为：[https://golang.org/dl/](https://golang.org/dl/)。

如果打不开可以使用这个地址：[https://golang.google.cn/dl/](https://golang.google.cn/dl/)。

各个系统对应的包名：

| 操作系统 | 包名 |
| :--- | :--- |
| Windows | go1.4.windows-amd64.msi |
| Linux | go1.4.linux-amd64.tar.gz |
| Mac | go1.4.darwin-amd64-osx10.8.pkg |
| FreeBSD | go1.4.freebsd-amd64.tar.gz |

## ![img](/static/image/golist.jpg)Windows 系统下安装

Windows 下可以使用 .msi 后缀\(在下载列表中可以找到该文件，如go1.4.2.windows-amd64.msi\)的安装包来安装。

默认情况下**.msi**文件会安装在**c:\Go**目录下。你可以将**c:\Go\bin**目录添加到**Path**环境变量中。添加后你需要重启命令窗口才能生效。

到这里go的基本配置就ok了，另外需要注意的是，你的go项目文件，都是放在工作目录里面的src下面的，一个项目一个文件。  
![img](/static/image/微信截图_20190928154122.png)

### Go



