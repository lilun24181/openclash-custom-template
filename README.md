# OpenClash Huayu Template

个人 OpenClash 订阅转换模板。它只保存策略组和分流规则，不包含机场订阅地址、节点、密码、内网地址或控制面板密钥。

## 模板地址

```text
https://raw.githubusercontent.com/lilun24181/openclash-custom-template/main/OpenClash-Huayu.ini
```

[查看模板文件](https://github.com/lilun24181/openclash-custom-template/blob/main/OpenClash-Huayu.ini)

## 使用

1. 在 OpenClash 的“配置订阅”页面编辑机场订阅。
2. 启用“订阅转换”。
3. 将“自定义模板地址”设置为本仓库 `OpenClash-Huayu.ini` 的 GitHub Raw 地址。
4. 保存后更新配置，并检查配置文件是否包含 `AI专用-自动`。

## 默认策略

- ChatGPT、Claude、Gemini、Copilot、HeyGen：`AI专用-自动`
- Meta AI、Perplexity：`AI专用-自动`
- `AI专用-自动` 只筛选美国和新加坡节点，保留 ChatGPT 连通性检测及 120 秒检测间隔。
- GitHub、Telegram、流媒体和国外网站：自动节点
- TikTok、Apple、Microsoft、Steam 下载、NVIDIA 下载和中国大陆流量：直连
- NVIDIA 登录、机场面板：国外代理

## 注意

- 机场节点名需要带有常见的国家或地区名称，地区自动组才能正确筛选。
- OpenClash 本地 DNS 覆写、Fake-IP 过滤和 NVIDIA 防火墙绕过不属于订阅转换模板，仍由路由器本地配置负责。
- 仓库必须为公开仓库，否则 OpenClash 的订阅转换服务无法读取 GitHub Raw 地址。
