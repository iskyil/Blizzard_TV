# 暴雪领取守望先锋
一个简单地定时领取暴雪礼品的python程序（确实十分简单 

:-)

礼品id
```
HS_NEMSY      福利1
HS_PACKET     福利2
WOW_COUPON    福利3
D3_COUPON     福利4
HEROES_COUPON 福利5
OW_CLIENTSE   福利6
OW_UPGRADE    福利7
SC_TERRAN     福利8
SC_PROTOSS    福利9
SC_ZERG       福利10
```
推荐使用``tencent``中函数并部署在腾讯云云函数平台，且不用担心隐私泄露(提取cookie方法同下

腾讯云部署需将配置里的**执行超时时间**改为900秒

![执行超时时间](/img/chufa.jpg)

Github部署方法：(极其不推荐，因为github的定时有延迟
1. 点个star(雾

2. 进入[活动界面](https://tv.blizzard.cn/award)登录暴雪账号，提取cookie

![cookie](/img/cookie.jpg)

3. 接着创建secrets，名为USERS，内容为``cookie#qmsgkey``即可

目前的设定的必须都有，所以即使您没有qmsgkey,您可以在#后随意填取（懒癌发作，不想改了，够用就行

4. 10点5分手动运行函数（定时似乎有延迟，您也可以更改迭代次数，并尽早定时


毕竟我是个新手，程序可读性极差，不过能帮助很多人也满足了