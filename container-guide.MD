# docker
docker ps
docker ps -a

备份容器image
docker commit -p [CONTAINER ID] 自定义名

docker images

docker restart [CONTAINER ID]

### docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
docker run
* -d: 后台运行容器，并返回容器ID；
* -P: 随机端口映射，容器内部端口随机映射到主机的高端口
* -p: 指定端口映射，格式为：主机(宿主)端口:容器端口
* --name="nginx-lb": 为容器指定一个名称；


###  docker exec [OPTIONS] CONTAINER COMMAND [ARG...]
-d :分离模式: 在后台运行
-i :即使没有附加也保持STDIN 打开
-t :分配一个伪终端

通过 exec 命令对指定的容器执行 bas
docker exec -it [CONTAINER ID] /bin/bash
