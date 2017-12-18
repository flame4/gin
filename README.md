# 如何下载到本地并运行起 gin 来进行调试？

1. 安装到本地路径
```bash
mkdir -p ~/YOU_PATH/src/github.com/gin-gonic
cd  ~/gin/src/github.com/gin-gonic
git clone github.com/gin-gonic/gin
```

2. 设置GOPATH
export GOPATH=/~/YOU_PATH

使用goland可以设置GOPATH，并且只指定gin目录为git目录，这样既可以本地编译测试，又可以方便提交和管理。

3. glide进行版本管理
```bash
go get github.com/Masterminds/glide
cp ~/gin/src/github.com/gin-gonic/gin/vendor/glide.yaml ~/gin/src
glide install
```
