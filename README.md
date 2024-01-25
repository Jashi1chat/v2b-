V2b-Theme-Sleek
前后端分离主题 可搭建多个前端应用
提交的需求尽量满足 不定期维护更新
请注意同源策略

TG反馈群: https://t.me/+IUSXjq0U8kU3NDk8
安装教程
后端：修改v2b后端支付回调文件

前后端分离重要步骤

进入目录 app/Services/PaymentService.php

文件第50行 'return_url' => config('v2board.app_url') . '/#/order/' . $order['trade_no'],

修改成： 'return_url' => $_SERVER['HTTP_ORIGIN'] . "/#/dashboard",


前端：正常解析一个网址到解析目录 下载前端文件放置解析根目录

前端配置部分都在config.js 文件里

修改config.js的hosturl 填写后端网址 https://xxxx.xx/ 格式
在线客服请到index.html里插入代码
网页标题和svg都在index.html 自行更改 有能力的可自行混淆config.js 文件
注意事项
v2b后台的邀请限制不要为0 不然会报错
用https 不然某些功能用不了
注意cors策略!!
产品演示(部分)
![image](https://github.com/Jashi1chat/v2b-/assets/145463840/7ac1cb04-f303-4178-97b3-ddbd56521b58)
![image](https://github.com/Jashi1chat/v2b-/assets/145463840/e32f7eba-5934-47f0-9410-d6fba4dd3879)
![image](https://github.com/Jashi1chat/v2b-/assets/145463840/6503eb0f-d028-47eb-acaf-db71f5464836)
![image](https://github.com/Jashi1chat/v2b-/assets/145463840/462cc68a-e8e2-4b5e-bca2-1ba820c0fd95)
![image](https://github.com/Jashi1chat/v2b-/assets/145463840/95422bc0-0d2e-48a3-a4f4-164f0640e0c3)
![image](https://github.com/Jashi1chat/v2b-/assets/145463840/04bbba31-cda0-4bc4-a2a7-5f9eef35c470)





