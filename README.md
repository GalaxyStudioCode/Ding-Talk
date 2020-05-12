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

发送的内容和选项在[这里](https://github.com/Galaxy-Studio-Team/DingTalk-Robot-Action/blob/master/.github/workflows/dingtalk.yml)修改

## 选项

| 选项    | 类型   | 要求   | default | 描述                                    |
| ------- | ------ | ------ | ------- | --------------------------------------- |
| url     | string | 必选   | none    | Webhook 地址                            |
| type    | string | 非必选 | text    | 消息类型，支持 Markdown、纯文本、custom |
| content | string | 必选   | none    | 消息文本，支持 Markdown、纯文本和 Json  |
| at      | string | 非必选 | none    | @用户                                   |

## Markdown 格式

[教程](https://lab.github.com/githubtraining/communicating-using-markdown)

## 自定义类型 Json格式

[链接](https://ding-doc.dingtalk.com/doc#/serverapi2/qf2nxq)

## 运行 Github Action 发送消息

为了防止误提交等意外发生，项目设置为 Star 时发送，Star 按钮在右上角。如果找不到，他是长这样的

![star](https://raw.githubusercontent.com/Galaxy-Studio-Team/DingTalk-Robot-Action/master/star.jpg?token=APIY2YRQSL56XHYLBLMPZKC6XIIEG)

Star 后再次发送只要 Unstar 再 Star 就行了
