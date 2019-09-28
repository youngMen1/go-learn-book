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

&lt;!--  
 /\* Font Definitions \*/  
 @font-face  
	{font-family:宋体;  
	panose-1:2 1 6 0 3 1 1 1 1 1;  
	mso-font-alt:SimSun;  
	mso-font-charset:134;  
	mso-generic-font-family:auto;  
	mso-font-pitch:variable;  
	mso-font-signature:3 680460288 22 0 262145 0;}  
@font-face  
	{font-family:"Cambria Math";  
	panose-1:2 4 5 3 5 4 6 3 2 4;  
	mso-font-charset:1;  
	mso-generic-font-family:roman;  
	mso-font-format:other;  
	mso-font-pitch:variable;  
	mso-font-signature:0 0 0 0 0 0;}  
@font-face  
	{font-family:Calibri;  
	panose-1:2 15 5 2 2 2 4 3 2 4;  
	mso-font-charset:0;  
	mso-generic-font-family:swiss;  
	mso-font-pitch:variable;  
	mso-font-signature:-520092929 1073786111 9 0 415 0;}  
@font-face  
	{font-family:"\@宋体";  
	panose-1:2 1 6 0 3 1 1 1 1 1;  
	mso-font-charset:134;  
	mso-generic-font-family:auto;  
	mso-font-pitch:variable;  
	mso-font-signature:3 680460288 22 0 262145 0;}  
 /\* Style Definitions \*/  
 p.MsoNormal, li.MsoNormal, div.MsoNormal  
	{mso-style-unhide:no;  
	mso-style-qformat:yes;  
	mso-style-parent:"";  
	margin:0cm;  
	margin-bottom:.0001pt;  
	text-align:justify;  
	text-justify:inter-ideograph;  
	mso-pagination:none;  
	font-size:10.5pt;  
	mso-bidi-font-size:11.0pt;  
	font-family:"Calibri","sans-serif";  
	mso-ascii-font-family:Calibri;  
	mso-ascii-theme-font:minor-latin;  
	mso-fareast-font-family:宋体;  
	mso-fareast-theme-font:minor-fareast;  
	mso-hansi-font-family:Calibri;  
	mso-hansi-theme-font:minor-latin;  
	mso-bidi-font-family:"Times New Roman";  
	mso-bidi-theme-font:minor-bidi;  
	mso-font-kerning:1.0pt;}  
.MsoChpDefault  
	{mso-style-type:export-only;  
	mso-default-props:yes;  
	mso-bidi-font-family:"Times New Roman";  
	mso-bidi-theme-font:minor-bidi;}  
 /\* Page Definitions \*/  
 @page  
	{mso-page-border-surround-header:no;  
	mso-page-border-surround-footer:no;}  
@page Section1  
	{size:612.0pt 792.0pt;  
	margin:72.0pt 90.0pt 72.0pt 90.0pt;  
	mso-header-margin:36.0pt;  
	mso-footer-margin:36.0pt;  
	mso-paper-source:0;}  
div.Section1  
	{page:Section1;}  
--&gt;  


go

基本命令



