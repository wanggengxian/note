## 命令
|command|comments|
|-|-|
|docker run -it --rm ubuntu:16.04 bash|-i 交互式操作，-t启动终端， --rm 退出时删除容器|
|docker system df|查看镜像、容器占用的空间|
|docker image ls --format "{{.ID}}: {{.Repository}}"|只包含镜像ID和仓库名字|
|docker image ls --digests|查看镜像摘要|