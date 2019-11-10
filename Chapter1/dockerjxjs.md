# Docker镜像加速


鉴于国内网络问题，后续拉取 Docker 镜像十分缓慢，我们可以需要配置加速器来解决，

新版的 Docker 使用 /etc/docker/daemon.json（Linux） 或者 %programdata%\docker\config\daemon.json（Windows） 来配置 Daemon 请在该配置文件中加入（没有该文件的话，请先建一个）：

```
官方中国代理
{
  "registry-mirrors": ["https://registry.docker-cn.com"]
}
```

```
阿里云
{
  "registry-mirrors": ["https://qbbiq8ik.mirror.aliyuncs.com"]
}
```

# 重启Docker Deamon
```
执行命令：
systemctl restart docker
```