<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#sec-1">1. Docker入门</a>
<ul>
<li><a href="#sec-1-1">1.1. 初识Docker</a></li>
<li><a href="#sec-1-2">1.2. Docker核心概念</a></li>
</ul>
</li>
<li><a href="#sec-2">2. Docker Image</a>
<ul>
<li><a href="#sec-2-1">2.1. 获取镜像</a></li>
<li><a href="#sec-2-2">2.2. 查看镜像信息</a></li>
<li><a href="#sec-2-3">2.3. 搜寻镜像</a></li>
<li><a href="#sec-2-4">2.4. 删除镜像</a></li>
<li><a href="#sec-2-5">2.5. 创建镜像</a></li>
<li><a href="#sec-2-6">2.6. 存出和载入镜像</a></li>
<li><a href="#sec-2-7">2.7. 上传镜像</a></li>
</ul>
</li>
<li><a href="#sec-3">3. Docker Container</a>
<ul>
<li><a href="#sec-3-1">3.1. 创建容器</a></li>
<li><a href="#sec-3-2">3.2. 启动终止容器</a></li>
<li><a href="#sec-3-3">3.3. 进入容器</a></li>
<li><a href="#sec-3-4">3.4. 删除容器</a></li>
<li><a href="#sec-3-5">3.5. 导入和导出容器</a></li>
</ul>
</li>
<li><a href="#sec-4">4. Docker use note</a>
<ul>
<li><a href="#sec-4-1">4.1. Docker install</a></li>
<li><a href="#sec-4-2">4.2. Docker command</a></li>
</ul>
</li>
<li><a href="#sec-5">5. common problem</a></li>
</ul>
</div>
</div>


# Docker入门<a id="sec-1" name="sec-1"></a>

杨保华 Docker技术入门与实战

## 初识Docker<a id="sec-1-1" name="sec-1-1"></a>

可以简单的将Docker容器理解为一种沙盒，每个容器内运行一个应用，不同的容器互相隔离，容器之间可以建立通信机制。容器的创建和停止都十分快速，容器自身对资源的需求也十分有限，远远低于虚拟机。

与传统虚拟机比较，Docker容器快，对系统资源需求少，一台主机可以运行数千个Docker容器,docker通过git的操作管理减少学习成本，通过Dockerfile配置文件来灵活自动化创建和部署

传统方式是硬件层面实现虚拟化，需要有额外的虚拟机管理应用和虚拟机操作系统层，Docker容器是操作系统层面上实现的虚拟化，直接复用本地主机的操作系统，因此更加轻量级

![img](//7xpyfe.com1.z0.glb.clouddn.com/blog/20171018/113219426.png)

## Docker核心概念<a id="sec-1-2" name="sec-1-2"></a>

1.  Image
2.  Container
    
    镜像自身是只读的，容器从镜像启动的时候，Docker会在镜像的最上层创建一个可写层，镜像本身将保持不变
3.  Repository
    
    Docker集中存放镜像文件的场所
    
    目前最大的公开仓库是Docker Hub 国内 Docker Pool
    
    Registry 注册服务器包含众多Repository

# Docker Image<a id="sec-2" name="sec-2"></a>

## 获取镜像<a id="sec-2-1" name="sec-2-1"></a>

docker pull NAME[: TAG] 

    docker pull ubuntu  
    不指定TAG默认选择latest标签,最新版本的镜像
    docker pull registry.hub.docker.com/ubuntu :latest

## 查看镜像信息<a id="sec-2-2" name="sec-2-2"></a>

-   docker images  #查看本地所有镜像

-   docker inspect 747cb2d60bbe #查看镜像信息

## 搜寻镜像<a id="sec-2-3" name="sec-2-3"></a>

-   docker search mysql #搜索远端仓库中共享的镜像
    
        docker search k8s --no-trunc=false --filter=stars=1 --filter=is-automated=true
        
        --filter=is-automated=true #只显示自动创建的镜像
        --no-trunc=false  #输出信息不截断显示
        --filter=stars=0 #指定星级以上的镜像

## 删除镜像<a id="sec-2-4" name="sec-2-4"></a>

docker rmi IMAGE[IMAGE..] #IMAGE可以是标签或者是ID

    docker rmi ff4 -f
    image 创建的容器存在的时候，是无法删除删除的 -f 强制删除

## 创建镜像<a id="sec-2-5" name="sec-2-5"></a>

1.  基于已有image的容器创建
    
    docker commit [OPTIONS] CONTAINER [REPOSITORY[: TAG]]
    
        docker commit -m "add a test" -a 'manue1' -p 836 centos_test:v1.0 
        
        -a 作者 -m  提交信息 -p 提交时暂停容器运行
2.  基于本地模版导入
    
    下载系统镜像模板
    
    <https://openvz.org/Download/template/precreated>
    
    cat xx.tar.gz | docker import - ubuntu:16.04
3.  基于Dockerfile创建

## 存出和载入镜像<a id="sec-2-6" name="sec-2-6"></a>

docker save -o ubuntu-16.04.tar ubuntu:latest

docker load &#x2013;input ubuntu-16.04.tar

## 上传镜像<a id="sec-2-7" name="sec-2-7"></a>

docker tag SOURCE\_IMAGE[:TAG] TARGET\_IMAGE[:TAG]

docker push TARGET\_IMAGE[: TAG]

    需要先修改本地仓库name为远程仓库名，必须先创建远程仓库manue1sec/test
    - docker tag 3a4 manue1sec/test:u_test
    - docker push manue1sec/test

# Docker Container<a id="sec-3" name="sec-3"></a>

## 创建容器<a id="sec-3-1" name="sec-3-1"></a>

docker create -it ubuntu

docker run -it ubuntu /bin/bash  #创建并启动容器，-t启动一个虚拟终端，-i保持终端 -d 在后台守护运行

## 启动终止容器<a id="sec-3-2" name="sec-3-2"></a>

docker start d3e

docker kill ce5 

docker ps -a #显示所有容器

## 进入容器<a id="sec-3-3" name="sec-3-3"></a>

docker attach 18a

docker exec -ti 24c /bin/bash  (推荐)

## 删除容器<a id="sec-3-4" name="sec-3-4"></a>

docker rm 18a

## 导入和导出容器<a id="sec-3-5" name="sec-3-5"></a>

docker export 18a > ubuntu\_container.tar  作为镜像

docker import a.tar

# Docker use note<a id="sec-4" name="sec-4"></a>

## Docker install<a id="sec-4-1" name="sec-4-1"></a>

1.  图解Docker
    
    ![img](//7xpyfe.com1.z0.glb.clouddn.com/blog/20170607/115341763.png)
2.  [官网文档](https://docs.docker.com/engine/installation/) 有详细说明
    
    国内网速很慢，采用了阿里云的[镜像源](https://yq.aliyun.com/articles/7695)
    
        curl -sSL http://acs-public-mirror.oss-cn-hangzhou.aliyuncs.com/docker-engine/intranet | sh -
    
    ![img](//7xpyfe.com1.z0.glb.clouddn.com/blog/20170607/131800763.png)

## Docker command<a id="sec-4-2" name="sec-4-2"></a>

-   service docker start/stop
-   docker rmi ventz/cif
-   docker images 命令查看本地的镜像列表
-   docker inspect cif 查看指定镜像的详细信息
-   docker ps -l 查看我们正在运行的容器 -l 最后状态
-   docker exec -it 9121af6cabed /bin/bash
-   docker stop cif 停止容器
-   docker rm -f cif  运行冲突 remove it using
-   docker run &#x2013;name cif -d -p 5000:5000 csirtgadgets/cif

# common problem<a id="sec-5" name="sec-5"></a>

1.  ImportError: No module named apt\_pkg
    
    安装docker 执行 sudo add-apt-repository 的时候报错
    
    Solve it by this:
    
    /usr/lib/python3/dist-packages# cp apt\_pkg.cpython-34m-x86\_64-linux-gnu.so apt\_pkg.so