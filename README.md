# DingTalk Robot Action

![](https://github.com/fifsky/dingtalk-action/workflows/dingtalk/badge.svg)

## 钉钉自定义机器人消息

##  示例

```yml
  type: markdown
  content: |
    # Hello
```

请在项目设置中设置 DINGTALK_WEBHOOK 的 Secret ，设置为获取的 Webhook

## 选项

| 选项    | 类型   | 要求   | default | 描述                                    |
| ------- | ------ | ------ | ------- | --------------------------------------- |
| url     | string | 必选   | none    | Webhook 地址                            |
| type    | string | 非必选 | text    | 消息类型，支持 Markdown、纯文本、custom |
| content | string | 必选   | none    | 消息文本，支持 Markdown、纯文本和 Json  |
| at      | string | 非必选 | none    | @用户                                   |

## 自定义类型 Json格式

[链接](https://ding-doc.dingtalk.com/doc#/serverapi2/qf2nxq)
