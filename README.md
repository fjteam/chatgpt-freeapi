# 免费 ChatGPT API

欢迎来到免费 ChatGPT API 项目，这是一个简单且开源的代理 API，您可以免费访问 OpenAI 的 ChatGPT API。

## 开放 ChatGPT 倡议

在一个技术以指数速度发展的世界里，人与机器之间的界限越来越模糊，那些有能力创造的人有责任确保所有人都能分享这种进步的好处。
一个免费和开源的代理 API，消除了获取最新人工智能技术的障碍，并使其为所有人所用。

## 用法

要使用 ChatGPT API 免费版，只需向以下端点发送 POST 请求：

```raw
https://freeapi.aivvm.com/
```

例如，要使用 `gpt-3.5-turbo-16k-0613` 模型回答 "你好?"，请发送以下 `curl` 命令：
- 官方例子
  ```sh
  curl https://api.openai.com/v1/chat/completions \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer sk-xxxxx' \
    -d '{
        "model": "gpt-3.5-turbo-16k-0613",
        "messages": [{"role": "user", "content": "你好?"}]
  }'
  ```

- 参考用法
  ```sh
  curl https://freeapi.aivvm.com/v1/chat/completions \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer sk-free-api' \
    -d '{
        "model": "gpt-3.5-turbo-16k-0613",
        "messages": [{"role": "user", "content": "你好?"}]
  }'
  ```

- 支持的模型[**CHAT**]

  |模型| RPM | TPM |
  |-------|-------|-------|
  |gpt-3.5-turbo	| 3,500	|90,000|
  |gpt-3.5-turbo-0301|	3,500	|90,000|
  |gpt-3.5-turbo-0613	|3,500|	90,000|
  |gpt-3.5-turbo-16k	|3,500	|180,000|
  |gpt-3.5-turbo-16k-0613|	3,500	|180,000|


- 您可以在 [OpenAI 官方文档](https://platform.openai.com/docs/api-reference/chat/create)上阅读完整的 API 文档。

## 介绍

ChatGPT 是由 OpenAI 开发的全球知名的会话 AI 模型，因生成类似人类的对各种提示和查询的回答而广受赞誉。凭借其先进的功能，ChatGPT 是聊天机器人、虚拟助手和其他自然语言处理应用程序的宝贵资产。

ChatGPT API 是一个强大的工具，允许开发人员将 ChatGPT 模型集成到自己的应用程序中。但是，要使用此 API，用户需要拥有 OpenAI API 密钥并支付使用费用。

免费 ChatGPT API 认为每个人都应该拥有访问最新人工智能技术的权利，而不必承担获取 API 密钥的经济负担。此开源代理 API 允许您在没有密钥的情况下访问 ChatGPT API，促进了对所有人的可访问性和创新。

## 免费 ChatGPT API 做什么？

这个简单的代理 API 充当您与 OpenAI ChatGPT API 之间的桥梁。您可以使用与原始 API 相同的格式向 ChatGPT API 免费版端点发送请求。该代理 API 将请求转发至 OpenAI API，使用该项目提供的 API 密钥，并将 OpenAI API 的响应返回给您。

## 隐私声明

该项目高度重视隐私，致力于保护其用户的隐私。该项目不会以任何方式收集、记录或存储用户输入的任何文本或由 OpenAI 服务器返回的任何文本。该项目不会向 OpenAI 或任何第三方提供有关 API 调用者的身份的任何信息，包括但不限于 IP 地址和用户代理字符串。该项目的源代码可供检查，以验证此声明。

然而，OpenAI API 根据其[数据使用政策](https://platform.openai.com/docs/data-usage-policies)保留 30 天的数据。

## 搭建自己的实例

如果您想运行自己的 ChatGPT API 免费版实例，可以按照以下步骤轻松完成：

1. 从 [OpenAI API 密钥](https://platform.openai.com/account/api-keys)获取 OpenAI API 密钥。
1. 在 GitHub 上 Star 和 Fork 此存储库。
1. 正确配置您的[环境变量](.env.example)。
1. 在本地部署 Docker 或在 [Google Cloud Run](https://cloud.google.com/run) 上部署。
1. 在本地设置速率限制或使用 [Google Cloud Armor](https://cloud.google.com/armor/docs/rate-limiting-overview)。

## 赞助我！

如果您发现免费 ChatGPT API 版有用，请考虑在 GitHub 上[赞助作者](https://github.com/CaoYunzhou/chatgpt-freeapi)，以支持持续的开发和维护。您的支持将帮助她维护此项目，并继续使人工智能技术对所有人都可访问。谢谢您的支持！

<table>
  <tr>
    <td><img src="./img/alipay.png" alt="支付宝" width="150"></td>
  </tr>
</table>
