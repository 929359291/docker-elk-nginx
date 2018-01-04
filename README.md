### docker-elk-nginx

本项目是收集本机（ubuntu）ssh登录日志  /var/log/auth.log 到es做分析。需要把 /var/log/auth.log 的权限改为 644 。这个坑还没机会填。

收集其他日志，请修改 `./logstash-agent/logstash.conf` 中`input`。并修改`docker-compose.yml`中挂载目录，`patterns`也需要定制。
```
docker-compose up -d
```
web http://ip:81 admin Passw0rd
