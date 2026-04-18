# **Apos接入合利宝配置**

> 文档地址：支付及退款/Apos接入合利宝配置.md


1，接入背景说明

新的微信小程序商城需要通过合利宝走跨境业务，涉及支付+支付申报两块功能，需要先在Apos商家后台新建一个合利宝支付渠道，如截图所示；

![image.png](http://media-hk01.oss-cn-hongkong.aliyuncs.com/images%2Fjackli%40jieztech.com%2F%E5%90%88%E5%88%A9%E5%AE%9D.md%2F32e2aecf-25ad-466d-90a6-e8288837dacd_image.png?Expires=1816661755&OSSAccessKeyId=LTAIXyAB35iFpHM0&Signature=AYPiGrNKcv2zMGJqOLmWIL%2Fxbqg%3D&x-oss-process=image%2Fformat%2Cpng)

勾选后，会弹出所需要配置参数项，也是你接下来需要获取的目标数据

![image.png](http://media-hk01.oss-cn-hongkong.aliyuncs.com/images%2Fjackli%40jieztech.com%2F%E5%90%88%E5%88%A9%E5%AE%9D.md%2Ff2d1a0b6-2499-4d9e-bd22-23c7d36fec87_image.png?Expires=1816661775&OSSAccessKeyId=LTAIXyAB35iFpHM0&Signature=o4VhGqnfV4POc%2Fy3WSPrQRNmFtY%3D&x-oss-process=image%2Fformat%2Cpng)

2，合利宝-支付渠道侧获取数据

A，使⽤邮箱账号登陆“商户后台”https://cbp.helipay.com/cbmerchant/login

![image.png](http://media-hk01.oss-cn-hongkong.aliyuncs.com/images%2Fjackli%40jieztech.com%2F%E5%90%88%E5%88%A9%E5%AE%9D.md%2Fd0b60936-7866-483b-a970-c3191cf13da6_image.png?Expires=1816661797&OSSAccessKeyId=LTAIXyAB35iFpHM0&Signature=3NbS0hFjPJWfKoFI5DJQBUDQ0Sw%3D&x-oss-process=image%2Fformat%2Cpng)

B,交易费率---产品列表---找到对应的产品“微信小程序”，

![image.png](http://media-hk01.oss-cn-hongkong.aliyuncs.com/images%2Fjackli%40jieztech.com%2F%E5%90%88%E5%88%A9%E5%AE%9D.md%2F871479c4-fa86-4db3-89a9-0ee8918ab9c0_image.png?Expires=1816661832&OSSAccessKeyId=LTAIXyAB35iFpHM0&Signature=HaV9NGnbKPubiZVgia%2FRY3ngQwQ%3D&x-oss-process=image%2Fformat%2Cpng)

C,点击右侧“详情”链接---点击“发送密钥到邮箱

![image.png](http://media-hk01.oss-cn-hongkong.aliyuncs.com/images%2Fjackli%40jieztech.com%2F%E5%90%88%E5%88%A9%E5%AE%9D.md%2F12c635bc-c928-453d-a8a9-abb622f3a11e_image.png?Expires=1816661851&OSSAccessKeyId=LTAIXyAB35iFpHM0&Signature=hVNWG0lzFmHN2Qd4olbcvhP54O8%3D&x-oss-process=image%2Fformat%2Cpng)

D，商家手机上会收到合利宝平台下发的短信，例如这种

你好：深圳芥舟科技有限公司

 商户编号[Me1004xxxx] 您的微信小程序产品的签名AES密钥为：[xxxxx/xxxx+xx+xxxx==]，SHA256密钥为：[xxxxxxxxxxx]，用于系统的API对接使用，请确保此密钥的安全，不能转交他人。
商户编号[Me1004xxxx] 您的报关产品的签名AES密钥为：[xxxxxJxxxxxxxxxxxxA==]，SHA256密钥为：[xxxxxxxx]，用于系统的API对接使用，请确保此密钥的安全，不能转交他人。

E,将收到的短信密钥+签名填入Apos商户后台。门店设置，支付设置的合利宝渠道中，配置完成

![image.png](http://media-hk01.oss-cn-hongkong.aliyuncs.com/images%2Fjackli%40jieztech.com%2F%E5%90%88%E5%88%A9%E5%AE%9D.md%2Ff45b7150-bbf8-4314-afba-d2803a3fdaf0_image.png?Expires=1816661870&OSSAccessKeyId=LTAIXyAB35iFpHM0&Signature=8E8Uwjel%2FNH8t2B2cbkAfh8KFVk%3D&x-oss-process=image%2Fformat%2Cpng)
