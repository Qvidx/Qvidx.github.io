---
hide:
  - title
  #- navigation # 显示右
  #- toc #显示左
  - footer
  - feedback
comments: false
---

<style>
  .md-typeset h1 {
    display: none;
  }
</style>

##Docker常用命令

###帮助命令
```shell
ducker version         #查看版本
docker info            #查看信息，包括镜像和容器的数量
docker 命令 --help     #万能命令（详细可以去看官网）
```

###镜像命令
```shell
docker images          #查看所有本地的主机上的镜像（返回镜像的仓库源、标签、id、创建时间、大小）
    #可选项
      -a,--all         #列出所有镜像
      -q,--quiet       #只显示镜像的id

docker search          #搜索镜像
    #可选项，通过收藏来过滤
      --filter=STARS=3000  #搜索出来的镜像就是stars大于3000的

docker pull            #下载镜像 docker pull 镜像名 [:tag]
docker rmi -f          #删除指定镜像（-f指id，可跟多个id）
docker rmi $(docker images -aq) #递归删除全部的镜像
```
###容器命令
```shell
docker run [可选参数] image
# 参数说明
--name="Name"          #容器名字 tomcat01 tomcat02,用来区分容器
-d                     #后台方式运行
-it                    #使用交互方式运行，进入容器查看内容
-p                     #指定容器端口 -p 8080:8080
      -p  ip:主机端口:容器端口
      -p  主机端口:容器端口（常用）
      -p  容器端口
      容器端口
exit                   #停止退出容器
Ctrl + P + Q           #容器不停止退出  
docker ps              #列出正在运行的容器
         -a            #列出历史运行的容器
         -n=?          #显示最近创建的容器
docker rm 容器id       #删除指定的容器，不能删除正在运行的容器  
docker rm -f $(docker ps -aq) #删除全部的容器
docker ps -a -q|xargs docker rm #删除全部的容器
```

###启动和停止容器的操作
```shell
docker start 容器id         #启动容器
dockers restart 容器id      #重启容器
docker stop 容器id          #停止容器
docker kill 容器id          #强制停止容器
```

##其他常用命令

###后台启动容器
```shell
docker run -d 镜像名      #在用docker ps . 发现镜像是停止的，
                         #这是因为容器使用后台运行，就必须要一个前台进程，就会自动停止
```

###查看日志
```shell
docker logs
            -tf          #显示日志时间戳
            --tail number     #要显示日志条数
```

###查看容器中进程信息ps
```shell
docker top 容器id
```

###查看镜像的元数据
```shell
docker inspect --
```

###进入当前正在运行的容器
```shell
#我们通常容器都是使用后台方式运行的，需要进入容器，修改配置
docker exec -it 容器id bashshell           #相当于打开一个新建的终端
docker attach  容器id                      #正在执行当前的终端
```

###从容器内拷贝文件到主机上
```shell
docker cp 容器id:容器内路径 目的的主机路径
```