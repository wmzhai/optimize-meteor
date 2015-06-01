# Kadira 入门

Kadira可以告诉我们下述问题

- 最近一分钟有多少method被调用
- 这个method需要多少时间处理
- 最常用的是哪些publication
- 我的程序的瓶颈在哪里

![](https://cldup.com/ywUoARDLNI.png) 

## Clone程序

首先向Meteor应用添加Kadira支持，我们使用下述程序

	git clone https://github.com/bulletproof-meteor/bullet-kadira.git

然后登录[Kadira](https://kadira.io/)，并创建一个账号。

## 创建Kadira App

我们在Kadira上创建一个app，并用我们的Todo程序连接它。

- 首先，在https://ui.kadira.io创建一个app
- 然后，你会获得AppId和AppSecret
- 在Meteor代码目录下，执行指令添加kadira: `meteor add meteorhacks:kadira`
- 最后在代码`server/kadira.js`中加入如下指令

		Kadira.connect("<appId>", "<appSecret>")

然后运行程序，添加几个todo

![](https://cldup.com/uebxVoxI0o.png) 


## 使用Kadira UI


程序启动以后可以看到kadira的运行效果，进一步的使用方法可以看[Kadira Academy](https://kadira.io/academy/)的文章。

