# API监控 (apiwatch)

面向国内开发者的 API 接口运行状态监控工具，飞书 / 企业微信实时告警。

---

## 功能亮点

- ✅ **HTTP 接口定时检测** — 每分钟自动 ping 一次
- ✅ **飞书 / 企业微信告警** — 连续 3 次失败立即通知，恢复时也通知
- ✅ **延迟 + 状态码监控** — 自定义超时阈值
- ✅ **内网接口支持** — 服务器有外网即可监控
- ✅ **5 个接口永久免费** — Pro 50 个 ¥9.9/月
- ✅ **零运维** — 基于腾讯云 CloudBase，无需服务器

## 在线使用

👉 [https://apiwatch.devany.top](https://apiwatch.devany.top)

## 技术栈

- **前端**：原生 HTML/CSS/JS（零框架依赖）
- **后端**：腾讯云 CloudBase 云函数（Node.js）
- **数据库**：CloudBase 文档型数据库
- **告警**：飞书 Webhook + 企业微信 Webhook
- **支付**：爱发电（afdian.net）Webhook 自动开通

## 项目结构

```
web/
├── landing.html    # 产品落地页
├── login.html      # 邮箱登录/注册
└── index.html      # 主界面（监控管理）

cloudfunctions/
├── monitorApi/     # API 云函数（CRUD + 套餐管理）
├── pingWorker/     # 定时检测 Worker
└── paymentWebhook/ # 爱发电支付回调
```

## 许可证

MIT License
