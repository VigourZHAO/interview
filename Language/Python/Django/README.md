WSGI(Web Server Gateway Interface): 服务网关

Django 常规请求流程：RESTful请求到达 Web 服务端口，请求到达 Server Gateway，进行请求解析，走中间件进行认证授权等相关，通过后再分发给 handler ，由此传给服务段进行服务处理，服务端将请求处理后，反馈结果。
