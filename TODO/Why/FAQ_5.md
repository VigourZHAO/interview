常规登陆认证方式：
    1. Cookie + Session 登录
    2. Token 登录
    3. SSO 单点登录
    4. OAuth 第三方登录

jwt: token实现原理
    Ref: https://www.jianshu.com/p/03ad32c1586c
    本质： Headers + salt + algorithm + payload
    Headers： 
    salt： 加盐（提供者持有）
    algorithm： 加密算法
    payload： 主体（info + expired time）
    加密： token = jwt.encode(payload=payload, key=salt, algorithm='HS256', headers=headers).decode('utf-8')
    解密：    
        1. 校验解密： info = jwt.decode(token, salt, True, algorithm='HS256')
        2. 非校验解码： info = jwt.decode(token, '', False, algorithm='HS256')


