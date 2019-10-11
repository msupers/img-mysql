# nexus

## 父镜像地址
```shell script
https://github.com/docker-library/mysql/blob/6b1dc54320b03b83a89068f49cc796fea0ff6bb4/5.7/Dockerfile
```
## 镜像信息
```shell script

https://cr.console.aliyun.com/repository/cn-beijing/meowbite/nexus/build

registry.cn-beijing.aliyuncs.com/meowbite/nexus:20191001

```

## 使用方法
```shell script
docker pull registry.cn-beijing.aliyuncs.com/meowbite/nexus:20191001

docker run -d -p 8081:8081 --name nexus registry.cn-beijing.aliyuncs.com/meowbite/nexus:20191001
```

## docker-compose管理
```shell script
mkdir /opt/nexus -p
cp docker-compose.yml /opt/mexus/
docker-compose up -d 
```

## 验证
```shell script
iptables -A INPUT -p tcp --dport 8081 -j ACCEPT

curl 127.0.0.1:8081
```