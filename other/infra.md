## lsblk指令
 lsblk命令的英文是“list block”,即用于列出所有可用块设备的信息,而且还能显示他们之间的依赖关系,但是它不会列出RAM盘的信息。块设备有硬盘,闪存盘,CD-ROM等等。

# telnet命令
telnet是应用层协议。是互联网远程登陆服务的标准协议和主要方式，用于服务器的远程控制。

### 测试远程主机端口通不通
`ssh -v -p 7890 admina@192.168.56.1`

`ssh 192.168.56.1 -p 7890`

`wget 192.168.56.1:7890`

### sar命令

https://linuxtools-rst.readthedocs.io/zh-cn/latest/tool/sar.html

top命令

free命令

# compose简介
定义和运行多容器的工具。

## 使用compose分三步
1. 使用Dockerfile定义应用程序环境
2. 使用docker-compose.yml定义构成应用程序的服务，以便在隔离环境下一起运行
3. 执行docker-compose up启动

## docker 安装命令

```
sudo yum remove docker \
                  docker-client \
                  docker-client-latest \
                  docker-common \
                  docker-latest \
                  docker-latest-logrotate \
                  docker-logrotate \
                  docker-engine

sudo yum install -y yum-utils
sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo

sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

sudo systemctl start docker

sudo docker run hello-world

yum update

yum install -y docker-compose-plugin
```


sudo yum groupinstall -y "Development Tools"
sudo yum install -y zlib-devel bzip2-devel openssl-devel ncurses-devel sqlite-devel readline-devel tk-devel gdbm-devel db4-devel libpcap-devel xz-devel libffi-devel





 