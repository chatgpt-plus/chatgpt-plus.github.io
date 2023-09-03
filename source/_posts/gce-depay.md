---
title: Depay(Dupay)虚拟卡如何白嫖谷歌云服务器$300美金大羊毛
date: 2023-08-10 13:57:59
update_at: 2023-08-10 14:06:22
categories: ChatGPT
tags: 
- Depay 
- 谷歌云
- VPS
- 薅羊毛
---

在前面文章中，我们说过，Depay(现在改名为Dupay了)卡平常可以用于微信，支付宝，美团消费，直接用USDT做日常小额消费，还免收手续费，小额的话，这点还是很舒服的。  

但其实，Depay卡的用途远不止此，平常可以多挖掘挖掘。今天教大家如何用Depay卡白嫖谷歌云服务器。申请成功后随即可获得300美元的试用金，有效期限是三个月。获得试用金后，就可以创建云服务器VM实例了。

##### 需要您提前准备好——
1. 一个[Depay卡](https://depay.depay.one/web-app/register-h5?invitCode=920750&lang=zh-cn)账号。
3. 至少2美金验证金，用于验证卡的所属权，验证完毕会归还。
4. 科学上网，[魔法上网](https://v.600ml.top/#/register?code=TOcQBatp)

##### 一、注册Depay卡
申请一个Depay卡(虚拟的，不需要现场办理，线上申请并kyc即可)，参考前文[《国内开通Chat GPT Plus保姆级教程【典藏】》](https://chatgpt-plus.github.io/chatgpt-plus/)中的“实操步骤”里的第2和3两步，充值2美刀也是参考这里即可。

##### 二、填写资料
使用您的谷歌账号登录Google Cloud官网并进行账户注册：[https://cloud.google.com/](https://cloud.google.com/) 
我们在**官网首页-->点击免费试用进行注册--> 填写国家和地区资料**，我们在右侧栏可以看到90天有效期的300刀赠额说明。国家地区选择真实所在地，这里我选择美国(填中国也可以)，勾选同意条款，点击同意并继续——

![image.png](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/gce-depay-1.png)


##### 三、绑定 Depay卡
在“付款方式”这里绑定您在上述第1步中申请的Depay卡，填卡的信息跟您申请卡的时候填写的保持一致即可。

![image.png](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/gce-depay-2.png)

谷歌云(GCP)在认证时会产生一笔$0.00~2.00 的交易，仅用于验证您是否是卡主，验证通过之后会原路退回，要是没法正常划扣的话是没办法过验证的。所以，要求咱们的Depay卡里至少得充值2美元，不充钱是没法用的。转账到Depay卡里时注意要转美元。谷歌云的验证方法其实是让您填写这笔订单的后6位数字(如图所示)。

![image.png](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/gce-depay-3.png)

Depay卡绑定成功之后，再填写3个小调查问卷题目就可以了，这里随便填。

![image.png](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/gce-depay-4.png)

到这里，白嫖成功，$300的大羊毛，90天。

![image.png](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/gce-depay-5.png)

##### 四、谷歌云初体验——创建VM虚拟机
这里，谷歌给你默认创建了个名为"My First Project"的项目，左侧栏找到 VM Instances-->点击 New VM Instance，创建一台虚拟机，这里，我选了2vCPU+4GB，10GB磁盘的Ubuntu 22.04系统机器，大概一个月费用是$28。

![image.png](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/gce-depay-6.png)

创建好后，就可以通过SSH远程登录管理您的VM服务器了。这里，我创建的VM服务器名字叫做"instance-1", 可以看到它有1 个外网IP可以远程连过去。
![image.png](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/gce-depay-7.png)

最后，本地连上SSH，完美。
![image.png](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/gce-depay-8.png)
