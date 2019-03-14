# 用户

### 登录中间件

如果页面需要登录，你可以在路由配置文件上加上下面的参数即可。
```
middleware: user@user.auth
```

### 获取用户信息

通过登录中间件之后用户信息会存在会话里面，可以通过`session`函数获取。

```twig
{{session('user_id')}}
```