## Docker 简介

### 基本定义

Docker 是一个开源的应用容器引擎，让开发者可以打包他们的应用以及依赖包到一个可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。

### 优势

1. 性能方面：不依赖于任何语言、框架或包括系统。几乎没有性能开销,可以很容易地在机器和数据中心中运行，大多数docker容器只需不到1秒即可启动。

2. 环境方面：让开发和生产环境一致，不会在出现“开发时一切都正常，肯定是运维的问题”现象。

3. 产品方面：提高测试和部署效率，给精益创业满意的开发周期。

### Docker使用的典型场景

1. Automating the packaging and deployment of applications

2. Creation of lightweight, private PAAS environments

3. Automated testing and continuous integration/deployment

4. Deploying and scaling web apps, databases and backend services

### Docker 组件

#### Docker 客户端与服务器

Docker 是一个客户-服务器（C/S）架构的程序。Docker客户端只需向Docker服务器或守护进程发出请求，守护进程或服务器将完成所有工作并返回结果。

#### 镜像

镜像是Docker生命周期中的“构建”阶段。

#### Registry

Registry用来保存用户构建的镜像，是Docker生命周期的“仓储和运输”阶段。

#### 容器

容器是Docker的启动或执行阶段。可以这样说，容器是：

- 另一种镜像格式
- 一系列标准的操作
- 一个执行环境

### 其他

和集装箱一样，Docker 在执行操作时，并不关心容器中到底塞进了什么，他不管里面是web服务器，还是数据库，或是应用程序服务器什么的。所有容器都按照相同的方式将内容装载进去。

## Docker 安装

- [mac安装](https://docs.docker.com/installation/mac/)

- [Ubuntu安装](https://docs.docker.com/installation/ubuntulinux/)

## Docker 基本操作

### container的创建、启动、停止与删除
- 查看info: `docker info`
- 查看正在运行的container: `docker ps`
- 交互式启动一个cotainer: `docker run -i -t ImageName`
- 交互式启动一个自定义命名的cotainer: `docker run --name ContianerName -i -t ImageName`
- 守护式启动一个cotainer: `docker run -d ImageName`
- 守护式启动一个自定义命名的cotainer: `docker run --name ContianerName -d ImageName`
- 重新启动一个已有的cotainer: `docker start ContianerName/ContainerId`
- 停止一个已运行的cotainer: `docker stop ContianerName/ContainerId`
- 删除一个cotainer: `docker rm ContianerName/ContainerId` 
- 删除Docker中全部cotainer: docker rm `docker ps -a -q` 

### 通过docker进行container内部操作
- 深入查看container的info: `docker info`
- 查看容器中的log: `docker logs ContianerName/ContainerId`
- 查看容器中的log(follow模式): `docker logs -f ContianerName/ContainerID`
- 查看容器中的进程情况: `docker top ContianerName/ContainerId`
- 守护式操作容器: `docker exec -d ContianerName/ContainerId CommandText`
- 交互式操作容器: `docker exec -i -t ContianerName/ContainerId CommandText`

### 通过docker进行image的操作
- 在客户端登陆Docker Hub: `docker login`
- 查看image列表: `docker images`
- 拉取image列表: `docker pull ImageName`
- 拉取特定的image: `docker pull ImageName:TagName`
- 搜索image: `docker search ImageName`
- commit image: `docker commit -m"llllllll" --author="XXXXX" ContainerID Username/ImageName`(官方不推荐) 
- build image: `docker build -t TagName ContextPath`
- 查看image历史: `docker build history ImageID`

## 欢迎大家继续贡献和分享笔记

Docker是一项很酷的技术。大家来贡献和分享笔记和好资料哦~






















