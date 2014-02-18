QQ Connect SDK for Ruby Api


================

### 通知:

本 gem 是在 [QQConnect SDK](https://github.com/046569/qq)基础上做了修改，使用的前提条件：已经通过Authorization Code获取了Access Token, 具体 [参考](http://wiki.connect.qq.com/%E4%BD%BF%E7%94%A8authorization_code%E8%8E%B7%E5%8F%96access_token
), 再通过获取openid 就可以调用 qq 互联的api

### 安装:

在你的Gemfile里新增一行

`gem 'qq_connect'`

然后

`bundle install`

### 使用:

必须传入的两个参数：

```Ruby
appid // 你注册的 app的 appid
access_token //获取到的用户的accessToken
```
获取用户信息：

```Ruby
user=Qq.new(appid,access_token])
res = user.get_user_info('https://graph.qq.com/user/get_user_info')
p res
```

相关参数请查阅[QQ互联开放平台](http://connect.qq.com/intro/login/)


### 授权:

MIT
