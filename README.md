# mysql

## 父镜像地址
```shell script
https://github.com/docker-library/mysql/blob/6b1dc54320b03b83a89068f49cc796fea0ff6bb4/5.7/Dockerfile
```
## 镜像信息
```shell script

https://cr.console.aliyun.com/repository/cn-beijing/meowbite/mysql/build

registry.cn-beijing.aliyuncs.com/meowbite/mysql:5.7

```

## 使用方法
```shell script
docker pull registry.cn-beijing.aliyuncs.com/meowbite/mysql:5.7

docker run --name some-mysql -p 3306:3306 -v /my/own/datadir:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=my-secret-pw -d registry.cn-beijing.aliyuncs.com/meowbite/mysql:5.7
```



## 验证

```shell script
mysql -h 127.0.0.1 -u root -p 
Enter password:
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MySQL connection id is 2
Server version: 5.7.27 MySQL Community Server (GPL)

Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

```