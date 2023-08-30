---
title: 国内ChatGPT API Key申请使用及虚拟信用卡充值教程
date: 2023-03-03 21:32:29
categories: ChatGPT
tags: 
- ChatGPT API
- ChatGPT
---

## 一、ChatGPT API介绍

今天，OpenAI 又开启了一个收费计划，开放 ChatGPT 和 Whisper API，前者允许任何企业在其应用程序、网站、产品和服务中使用 ChatGPT 功能，后者可以实现语音转文本。

![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-1.png)


ChatGPT API有什么用？简单地说，它允许任何企业或个人在他们自己的应用程序、网站、产品和服务中使用 ChatGPT 功能，并且是最新的训练模型，$0.002/1K tokens的价格看起来也似乎非常诱人！

ChatGPT API 的开放, 类似乔布斯当时建立了Apple应用商店，让全世界的企业和个人开发者都可以在应用程序中预留人工智能的接口, 与类ChatGPT平台联结起来。

![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-2.png)


## 二、ChatGPT账号申请及充值

本文默认你已经申请好了OpenAI官网账号，如果你还没有，请先参考这篇[《Chat GPT官方推荐新手教程》](https://chatgpt-plus.github.io/chatgpt-plus/) 参考文中的第1步先申请一个账号，需要借助接码平台和Depay虚拟信用卡，成本不到1$，支持支付宝。
关于充值，参考新手教程中的第2、3步做即可。

有了卡之后，登录到OpenAI网站，点击右上角账号信息-->Billing ,设置付款方式，在这里绑定你刚刚申请的卡号信息即可对ChatGPT API充值。

![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-3.png)


## 三、开始使用ChatGPT API

OpenAI账号注册完成后，登录界面如下所示。点击右上角View API keys—> Create new secret key，可以生成属于你自己的API，有了这个API，就可以用于开发基于ChatGPT API的应用程序。

需要注意的是，出于安全原因，这个API只展示一次，请务必在关闭对话框之前，将其复制到你其他的地方保管。

![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-4.png)



![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-5.png)



另外，点击左侧栏的Usage ,可以方便清晰看到token的使用量情况，数据5分钟更新一次。OpenAI官方针对每一个新注册的账户，提供$18免费token使用额度。这样一想，前面花费不到$1就能默认有$18 token使用额度，不亏。不过需要注意的是，免费额度有时间限制，过期了额度就作废。

![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-6.png)



ChatGPT API的使用方法也十分简单，首先可以用简单的curl命令测试下。把$OPENAI_API_KEY替换成你自己的API KEY就好。

![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-7.png)



另外，官方也提供了基于各种编程语言的简单实现代码。比如Python，你只需import openai包，带上刚申请的API，模型选择这次开放的最新模型——gpt-3.5-turbo就可以。

![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-8.png)



更多的例子，请自行参考[官方例子](https://openai.com/blog/introducing-chatgpt-and-whisper-apis)以及[官方API文档](https://platform.openai.com/docs/api-reference/introduction)。

不过，作为开发人员，我们也可以灵活地选择特定构建版本，以享受最新的特性。例如今天发布的 gpt-3.5-turbo-0301，这种临时版本至少会支持3个月。

## 四、ChatGPT API使用的几个问题

### 1、GPT-3.5-turbo模型

这么说吧，GPT-3.5 是 OpenAI公司目前为止通API方式所提供的最强大的文本生成模型，其中，代号“turbo”指的是 GPT-3.5 的优化版本、响应速度更快。OpenAI 也将GPT其称之为是“许多非聊天用例的最佳模型”。按照计划，GPT-4今年会发布。gpt-3.5-turb模型号称成本只有达芬奇text-davinci-003 的十分之一，而且会一直保持更新，比如gpt-3.5-turbo-0301这样，

### 2、ChatGPT API速度如何

个人感觉这个 token 用得还是挺快的！比官方的ChatGPT要快，响应也不需要一个字一个字蹦出来了。会不会突然有点不适应了？哈哈！

### 3、如何给ChatGPT API充值

文章开头说了，国内无法通过任何银行卡充值，必须使用Depay虚拟信用卡来绑定充值，参考文章第二章的官方指导文档操作即可。当然，如果你已经有国外卡，那会方便很多，直接充。

### 4、ChatGPT API Token收费标准

官方这次的收费标准是 $0.002/1K tokens，大概 750 词。虽然1k个token看起来很多。但其实，发送一段供API响应的文本可能就会花费不少token。

据我观察，基本问1个问题就要耗费100多个token，算起来其实不少的，尤其在连续会话中，为了保持对话的连续性，必须每次都要回传历史消息，并且输入都要算 token 数算钱的，满打满算，按量付费其实也不便宜。
按照一般的经验来看，在英语中“一个 token 通常对应大约 4 个字符”，而1个汉字大致是2~2.5个token。
举一个官方的说明例子可能更直观一些：根据 OpenAI 官方文档，“ChatGPT is great!”这组单词就需要六个 token —— 它的 API 将其分解为 “Chat”、“G”、“PT”、“is”、“great”和“!”。
如果你想查询一串指定的文本到底需要耗费多少个token(钱💰)，官方也有提供一个[免费查询计算器](https://platform.openai.com/tokenizer)：
![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-9.png)


### 5、ChatGPT API的连续会话能力

我们知道，官方的ChatGPT以及ChatGPT Plus最强的地方就在于它拥有上下文联系，也就是能跟你连续会话的能力，正因为如此，让你拥有了跟一个现实伴侣、导师或者朋友交谈的感觉。另外，这次的API自带连续对话能力，你只需在接口入参的地方将历史对话内容一并赋值给Message参数，回传给模型就可以。不过这势必会增加token的费用，这点有点坑啊。官方似乎也意识到了这点，所以，单次传的token上限为4096，超过4096会返回报错。

### 6、ChatGPT API使用的地区限制

ChatGPT API使用有地区限制吗？有群友反馈说今天开始国内访问API已经不稳定了，目前我这边还是可以的。但后面不好说，可能得走国际IP也说不定。

### 7、关于套壳APP&网站

随着官方ChatAPT API的发布，过段时间，国内势必会不断涌出套壳APP或者网站，声称用的最新的ChatAPT API。文章前面说了，token是需要付费的，而且如果达到跟官方chatgpt甚至 chatgpt plus一样优秀的连续会话水平，是需要回传历史会话信息的。试想一下，把你跟ChatAPT API聊天的答案之类的都传过去，这一下得花多少token。请大家千万要多留一个心眼，毕竟天下没有免费的午餐。

比如，你可以试试问一下那些套壳AI网站“今天是哪一天？”，看看它怎么回答。

![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-10.png)



### 8、Whisper API

除了 ChatGPT API，这次，OpenAI 还宣布了 Whisper API 。Whisper 是OpenAI在去年9月份开源的语音转文字模型，开元之后就受到了全球开发者社区的盛赞。Whisper API 基于开源 的whisper-large-v2 模型，方便开发者们按需使用，价格为每分钟 0.006 美元。

根据官方文档的介绍，Whisper API 可被用来转录（以源语言转录）或翻译（转录为英语），并转为各种格式（M4A、MP3、MP4、MPEG、MPGA、WAV、WEBM）

官方也有提供Whisper的使用[例子](https://openai.com/blog/introducing-chatgpt-and-whisper-apis)：

![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-11.png)



![](https://cdn.jsdelivr.net/gh/btcltceth/blogassets@latest/c/img/chatgpt-api-12.png)



## 五、ChatGPT Plus还有必要续费吗？

最后一个问题，ChatGPT API发布之后，有些人会想，是不是ChatGPT Plus可以不用续费了。其实并不然。正如上面所介绍，ChatGPT API使用偏向于程序员以及应用开发者，对普通用户有较大的使用门槛。还有，上面也说了，Token看似便宜，实际上需要回传历史消息才能延续上下文连续回话能力，何况当前还有4096个token的限制，真正使用下来，一个月也比Plus的$20定价也便宜不了多少。

API速度上会比Plus快，但是，二者关于回答的质量上，目前肯定是官方Plus占优。毕竟除了模型，模型的参数才是决定性的，一句话，你永远可以相信官方。

## 六、如何升级到ChatGPT Plus?

如果有条件，还是建议按照这篇[国内开通Chat GPT Plus保姆级教程【典藏】](https://chatgpt-plus.github.io)，升级到ChatGPT Plus，一劳永逸!