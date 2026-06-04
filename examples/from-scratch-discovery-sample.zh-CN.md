# 样例报告：从零开始发现 App Idea

证据风格：示意样例。真实构建决策前，请替换为最新来源证据。

## 决策问题

如果一个独立开发者完全不知道做什么 app，下一步最值得研究什么？

## 开发者假设

- 平台：iOS 或 Web。
- 时间预算：1-2 周 MVP。
- 技术栈：SwiftUI 或 Next.js。
- 地区/语言：英语用户。
- 获客优势：Reddit、X、SEO、App Store 搜索。

## 信号扫描摘要

| 信号桶 | 检查来源 | 有用信号 | 置信度 |
|---|---|---|---|
| App store 排名/搜索 | App Store 和 Google Play 品类搜索 | 高频工作流的付费消费工具仍然可行 | 中 |
| 评论痛点 | 热门效率、营养、笔记、植物、文档 app | 价格、导出、复杂度和隐私抱怨反复出现 | 中 |
| 新产品发布 | AI 笔记、个人效率、浏览器工具 | 许多新产品围绕捕捉、摘要和自动化发布 | 中 |
| 社区痛点 | Reddit/HN productivity、iOS、freelancer、PKM 讨论 | 用户反复寻找更简单替代品和迁移路径 | 中 |
| 定价/变现 | 竞品定价页和 IAP 列表 | 订阅常见，但一次性买断也可作为差异化 | 中 |

## 原始候选池

| 候选 idea | 用户群体 | 问题触发 | 变现信号 | 获客切口 | 保留？ |
|---|---|---|---|---|---|
| 私密语音记忆 app | 创始人/写作者/ADHD 用户 | 语音笔记难搜索、难导出 | 订阅或本地版买断 | PKM 和效率社区 | 是 |
| MyFitnessPal switcher | Macro tracking 用户 | Redesign、复杂、迁移痛点 | 低价年订阅 | "Alternative to MyFitnessPal" SEO | 是 |
| 宠物安全植物清单 | 有宠物的室内植物用户 | 不确定哪些植物有毒 | 年订阅或一次性审核 | toxic plants TikTok/SEO | 是 |
| 自由职业者收据扫描 | 自由职业者 | 每月报销/税务整理麻烦 | 年订阅 | freelancer tax 内容 | 是 |
| AI habit tracker | 自我提升用户 | 通用 habit tracker 不够适配 | 订阅 | TikTok demo | 可能 |
| 销售会议机器人 | B2B 销售团队 | CRM 笔记录入 | 团队订阅 | LinkedIn outbound | 否 |
| AI recipe generator | 家庭做饭用户 | meal planning 疲劳 | 订阅 | SEO | 否 |
| Travel itinerary AI app | 旅行用户 | 规划复杂 | Freemium | 旅行 TikTok | 否 |

## 被拒绝的 idea

| Idea | 拒绝原因 |
|---|---|
| 销售会议机器人 | B2B 会议工具拥挤，销售集成扩大范围，支持成本高 |
| AI recipe generator | 太泛，留存弱，免费替代品多 |
| Travel itinerary AI app | 季节性强，竞品多，如果没有 booking 很难变现 |

## 排名候选

| 排名 | Idea | 用户切口 | 分数 | 证据强度 | 主要风险 |
|---:|---|---|---:|---|---|
| 1 | 私密语音记忆 app | 用语音思考、需要检索笔记的人 | 81 | 中 | 转写成本和赛道拥挤 |
| 2 | MyFitnessPal switcher | 不满头部产品的 macro tracking 重度用户 | 77 | 中 | 食物数据库覆盖 |
| 3 | 宠物安全植物清单 | 有室内植物的宠物主人和父母 | 74 | 中 | 安全/信任风险 |
| 4 | 自由职业者收据扫描 | 每月做 admin 的 solo freelancer | 72 | 弱-中 | OCR/导出准确性 |

## 最高推荐

- Idea：私密语音记忆 app。
- 一句话概念：快速录音，并把想法转成可搜索、可导出的 Markdown 笔记。
- 为什么是它：使用频率高，工作流窄，隐私/导出差异化明确，MVP 可控。
- 为什么现在：用户已经接受 AI notes，但很多工具是会议优先或团队优先。
- 为什么适合独立开发者：第一版只需要专注 capture、transcript、summary、search、export。
- 主要风险：重度用户会带来较高转写成本。

## MVP 范围

- 必备：一键录音、转写、摘要、搜索、Markdown 导出。
- 可选：Obsidian/Notion 导出、短笔记本地转写。
- 排除：会议机器人、团队协作、视频会议集成。
- 定价假设：每月免费 10 条笔记，$4.99/month 或 $39/year。
- 首个获客渠道：PKM/效率社区和 X demo。

## 7 天验证计划

| 天数 | 动作 | 成功信号 |
|---:|---|---|
| 1 | 发布带 3 张 mock screenshot 的 landing page | 30 个 waitlist signup |
| 2 | 在效率和 PKM 社区发布 prototype flow | 10 条具体痛点评论 |
| 3 | 提供人工转写 + Markdown 导出 | 5 个用户提交真实音频 |
| 4 | 访谈隐私和导出需求 | 3 个用户要求 Obsidian/Notion |
| 5 | 测试 pricing page | 3 个用户选择付费层 |
| 6 | 做 clickable prototype | 8/10 完成录音到导出 |
| 7 | 决定 build/no-build | 只有用户要求重复使用时继续 |

## 下一步需要深入分析

- 最新竞品评论挖掘。
- 真实 App Store 关键词搜索。
- 转写成本模型。
- Landing page 转化测试。

## 交给 Analyst 的提示词

```text
使用 app-opportunity-analyst 深度验证这个 idea：

Idea：私密语音记忆 app，把快速录音转成可搜索、可导出的 Markdown 笔记。
目标用户：创始人、写作者、ADHD 用户，以及习惯用语音思考的 PKM 用户。
平台：iOS 优先，Mac 可选。
关键证据：AI notes 需求可见，会议优先产品留下了个人记忆缺口，隐私和导出是重复痛点。
主要风险：转写成本、品类拥挤、本地模型性能。
开发者限制：独立开发者，SwiftUI，1-2 周 MVP，低预算。
```
