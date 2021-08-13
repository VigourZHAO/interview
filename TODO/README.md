问题记录：
```
elementary OS 6 下安装 Docker
报错信息:
    1. echo \
"deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
$(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
    2. echo $(lsb_release -cs) 为 odin，在 Docker维护的信息上无此版本相关。
```
