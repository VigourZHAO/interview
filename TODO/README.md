问题记录：
1. 安装 Docker 报错问题
```
elementary OS 6 下安装 Docker
报错信息:
    1. echo \
"deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
$(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
    2. echo $(lsb_release -cs) 为 odin，在 Docker维护的信息上无此版本相关。
问题排错： elementary os 6基于ubuntu 20.04，修改源文件 odin 为 focal.
    
```
2. Neutron 知识点回顾：ing
3. 英文自我介绍（Done）
4. Django生命周期分析？
5. Linux 端口复用技术实现？
