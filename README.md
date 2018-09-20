@[TOC](注册登录的完整实例（使用vue）)

# 项目实例介绍
本项目实例主要采用两种方式实现登录、注册、注销的功能，涉及前端的cookies、session和token三个内容。前端使用vue和vue-router，后台服务采用node.js和express结合express-session

# 项目实例结构
**说明：** src---对应---server，src-token--对应server-token
```
vue-login
├─build                  
├─config
├─server              
├─server-token        
├─src
├─src-token
│  ├─assets
│  ├─router
│  ├─store
│  ├─util
│  └─views
└─static
```
## session方式
服务端将登陆后的sessionId返回给客户端，客户端保存
## token方式
客户端登陆后由服务端生成token返回给客户端
