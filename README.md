# CSDNAccess
Run this program to add your CSDN view number

使用这个项目可以给CSDN刷阅读量，使用了http代理，和模仿浏览器，实测是可以刷成功的

# 参数配置

代码都在 /app/Main.py 中，可配置的参数在代码开头，参数介绍：
1. threadN : 使用几个线程来运行，建议和自己电脑的CPU核心数相同
2. url_list : 需要刷访问量的url

# 使用方法
## 一，你有docker的情况下（推荐）
直接下载contrain：`docker pull davidhwj/csdn-access`
然后运行：`docker run -d -t davidhwj/csdn-access`

或者下载代码自己构建镜像：
1. 下载本项目 
`git clone git@github.com:David-hwj/CSDNAccess.git`
2. 进入项目文件夹
`cd CSDNAccess`
3. 构建镜像(注意命令后有个点)
`docker build -t csdn-access .`
4. 运行镜像
`docker run -d -t csdn-access`

## 二，直接运行代码
直接运行代码需要本地有几个python的模块，需要的模块见`requirements.txt`文件