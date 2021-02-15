# xiao-you

> 可以公开的情报

小游，小云（基于 [el-bot](https://github.com/ElpsyCN/el-bot) 的机器人，尚未开源）的妹妹，用来存储一些示例配置。

你可以为 [rss.yml](./rss.yml) 提交 PR，以在群 389401003 内订阅博客。

例如：

```yml
rss:
  - name: 云游君的小站
    url: https://www.yunyoujun.cn/atom.xml
    customFields:
      item:
        - updated
        - summary
    content:
      - 标题：${item.title}
      - 链接：${item.link}
      - 时间：${item.updated}
      - "---------------"
      - ${item.summary}
    target:
      group:
        - 389401003
```
