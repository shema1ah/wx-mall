# 微信小程序商城

微信小程序商城，微信小程序微店。


## 扫码体验

<p>
<img src="https://cdn.it120.cc/apifactory/2017/09/15/487409738ebb80c44eda01c46d59b20c.jpg" width="200px">
</p>

## 接口 & 后台声明

本项目为小程序商城纯前端项目，由于人力和精力所限，本项目并未有开发配套的后台系统，而是直接使用了 [api 工厂](https://www.it120.cc/) 提供的免费接口和后台，可以完全满足本项目的所有功能需求。

- [接口 SDK](https://github.com/gooking/wxapi)

- [WeUI](https://github.com/Tencent/weui-wxss/)


## 使用说明

1、申请后台账号/获取专属域名

2、开通商城模块

<img src="https://cdn.it120.cc/apifactory/2018/11/14/b61fe6ffb2460f7e4554758b394814f5.png">

3、修改根目录下 config.js 文件

```javascript
module.exports = {
  version: "5.0",
  note: "优化接口调用流程",
  subDomain: "tz", // 如果域名是： https://api.it120.cc/abcd 那么这里只要填写 abcd
  appid: "wxa46b09d413fbcaff", // 您的小程序的appid，购物单功能需要使用
  shareProfile: "百款精品商品，总有一款适合您" // 首页转发的时候话术
};

```

4、[设置小程序合法服务器域名](https://www.it120.cc/info/faq/10469)

5、重启您的小程序开发工具，完成

6、如何在后台管理小程序启动图和首页头部的轮播 banner 图片

```javascript
这两个功能都是使用后台 “系统设置” --> “banner” 管理功能来实现的；
后台发布banner的时候，自定义类型请分别填写  app  和  index；
小程序会自动读取类型为 app 的banner图片作为启动展示图片；
小程序会自动读取类型为 index 的banner图片作为首页头部的轮播图；
```


