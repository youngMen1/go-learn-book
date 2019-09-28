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

### Go基本命令

go语言自带一套完整的命令操作系统，你可以在终端中执行go命令来进行查看！接下来介绍一些常用的go命令操作go version查看go当前的版本go env查看当前go的环境变量go list查看当前安装的全部packagego run编译并运行go程序go build这个命令主要用于编译代码。在包的编译过程中，若有必要，会同时编译与之相关联的包。go build命令有如下几点值得注意的地方：如果是普通包，当你执行go build命令之后，它不会产生任何文件。如果你需要在$GOPATH/pkg下生成相应的文件，那就得执行go install命令如果是main包，当你执行go build命令之后，它就会在当前目录下生成一个可执行文件。如果你需要在$GOPATH/bin下生成相应的文件，那么你需要执行go install命令，或者使用go build -o 路径/xx如果项目文件夹中有多个文件，但是此时你只想编译其中某一个文件，就可以在go build之后加上文件名，例如：go build demo\_1.go。默认情况下，build命令会编译当前目录下所有go文件你也可以指定编译输出的文件名。我们可以使用go build -o xxx，来指定编译输出的文件名，默认情况下是你的项目名go build会自动忽略以\_或者.开头的go文件如果你的源代码针对不同操作系统需要不同的处理，那么你可以根据不同操作系统后缀来命名文件。例如有一个读取数组的程序，它对于不同的操作系统可能有如下几个源文件：

打算地方

