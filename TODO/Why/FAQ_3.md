1. 输入地址：
    先从本地缓存找(历史记录等)，如果没有，Enter。
2. 浏览器查找域名的 IP 地址：
    1. 请求发起后，域名解析：本地 hosts
    2. 本地 hosts 查找不到，发送 DNS 请求到本地服务器，再查询本地服务器的缓存，递归直到查找到。
3. 先发送 HTTP 请求（请求与80端口建立链接）：
    三次握手四次挥手: seq、ack、syn、FIN、TIME_WAIT
    Request URL + Request Method + Status Code + Request Address:port + Policy
4. 服务重定向(TCP 拆包)：
    重定向至要搜索的服务。
5. 服务端返回：
    Response
6. WEB解析渲染：
    展示
