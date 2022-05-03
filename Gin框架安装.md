***windows\*环境搭建golang的\*gin框架\*简易教程**

### 第一步：安装golang

下载go****.msi安装程序，按照界面提示安装

### 第二步：配置golang代理库地址（此步可忽略）

```bash
set GOPROXY=https://go.proxy.xxx.net
```

### 第三步： 创建项目

首先使用go env查看GOPATH目录，在该目录下创建bin、pkg、src目录
然后在src目录下创建项目，比如studygin，并在项目下创建go.mod文件

### 第四步： 生成go.mod文件

golang 建立新项目时，要注意在终端上使用以下命令建立go.mod文件。否则 go get，以及引用自己项目包文件时会出错。

```csharp
 go mod init 项目名
```

### 第五步：安裝gin包

直接在项目目录下执行命令安装：

```Go
go get github.com/gin-gonic/gin
```

### 第六步：编写main.go文件

可参考https://gin-gonic.com/zh-cn/

### 第六步：编译

```Go
go build
```