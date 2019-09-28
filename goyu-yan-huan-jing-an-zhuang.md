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

go语言自带一套完整的命令操作系统，你可以在终端中执行go命令来进行查看！接下来介绍一些常用的go命令操作

go version  
查看go当前的版本

go env  
查看当前go的环境变量

go list  
查看当前安装的全部package

go run  
编译并运行go程序

go build  
这个命令主要用于编译代码。在包的编译过程中，若有必要，会同时编译与之相关联的包。go build命令有如下几点值得注意的地方：

如果是普通包，当你执行go build命令之后，它不会产生任何文件。如果你需要在$GOPATH/pkg下生成相应的文件，那就得执行go install命令  
如果是main包，当你执行go build命令之后，它就会在当前目录下生成一个可执行文件。如果你需要在$GOPATH/bin下生成相应的文件，那么你需要执行go install命令，或者使用go build -o 路径/xx  
如果项目文件夹中有多个文件，但是此时你只想编译其中某一个文件，就可以在go build之后加上文件名，例如：go build demo\_1.go。默认情况下，build命令会编译当前目录下所有go文件  
你也可以指定编译输出的文件名。我们可以使用go build -o xxx，来指定编译输出的文件名，默认情况下是你的项目名  
go build会自动忽略以\_或者.开头的go文件  
如果你的源代码针对不同操作系统需要不同的处理，那么你可以根据不同操作系统后缀来命名文件。例如有一个读取数组的程序，它对于不同的操作系统可能有如下几个源文件：

```
array_linux.go 
array_windows.go 
array_darwin.go
```

### go build

会选择性的编译以系统名结尾的文件，例如，在Linux系统下编译只会选择array\_linux.go文件，其他系统命名后缀文件全部忽略！

常用参数介绍：

* -o：指定输出的文件名，可以带上路径，例如：go build -o app/a.exe

* -i：安装相应的包，相当于build+install

* -a：更新全部已经是最新的包的

* -n：把需要执行的编译命令打印出来，但是不执行它们

* -p n：指定可以并行运行的编译数目，默认是CPU数量

* -race：开启编译的时候自动检测数据竞争的情况，目前只支持64位的机器

* -v：打印出来正在编译的包名

* -work：打印出来编译时间的临时文件夹名称，并且如果已经存在的话就不要删除

* -x：打印出来执行的命令，与-n类似，只不过这个会执行

### go clean

这个命令是用来移除当前源码包和关联源码包里面编译生成的文件，这些文件包括：

* \_obj/：旧的object目录，由Makefiles遗留

* \_test/：旧的test目录，由Makefiles遗留

* \_testmain.go：旧的gotest文件，由Makefiles遗留

* test.out：旧的test记录，由Makefiles遗留

* build.out：旧的test记录，由Makefiles遗留

* \*.\[568ao\]：object文件，由Makefiles遗留

* DIR\(.exe\)：由go build产生

* DIR.test\(.exe\)：由go test -c产生

* MAINFILE\(.exe\)：由go build MAINFILE.go产生

* \*.so：由SWIG产生

参数介绍：

* -i：清楚关联的安装包和可运行文件，也就是通过go install安装的文件

* -n：把需要执行的清除命令打印出来，但是不执行

* -f：循环的清除在import引入的包

* -x：打印出来执行的详细命令，与-n类似，只不过这个会执行

### 等等。。。。。。。。。

## Go语言开发

注意package需要为main

![img](/static/image/微信截图_20190928163056.png)  
![img](/static/image/微信截图_20190928163249.png)

## 参考

[https://blog.csdn.net/y472360651/article/details/82914263](https://blog.csdn.net/y472360651/article/details/82914263)

