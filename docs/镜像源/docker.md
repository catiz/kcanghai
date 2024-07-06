# Docker
## 加速地址
```
https://docker.isikun.eu.org
```

## 使用方法
找到 Docker 的配置文件。这个文件通常位于 /etc/docker/daemon.json。如果该文件不存在，您可以创建它。
编辑 daemon.json 文件，添加或修改 registry-mirrors 键值
```json
{
  "registry-mirrors": ["https://docker.isikun.eu.org"]
}
```

保存 daemon.json 文件并重启 Docker 服务以应用更改