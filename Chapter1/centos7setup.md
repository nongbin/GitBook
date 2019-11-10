# Centos7安装Docker

# 设置仓库

```
yum install -y yum-utils device-mapper-persistent-data lvm2
yum-config-manager --add-repo http://mirrors.aliyun.com/docker-ce/linux/centos/docker-ce.repo
yum makecache fast
```

# 安装docker CE
```
yum -y install docker-ce
```
# 启动Docker
```
systemctl start docker
```