# 带来源样例报告：卡路里与宏量营养追踪

证据检查日期：2026-06-04

## 决策问题

独立开发者是否值得做一个卡路里或 macro tracker app？

## 核心结论

- 结论：避开通用 calorie tracker，验证一个面向不满头部产品的迁移切口。
- 最佳切入点：面向想离开 MyFitnessPal 的重度用户，做一个快速、低摩擦、食物数据更可信、支持导出的食物记录工具。
- 为什么现在：需求和付费意愿已经被验证，但头部产品很大，用户抱怨集中在复杂 UI、订阅、数据库质量和 redesign。
- 最大风险：食物数据库和 barcode 覆盖对独立开发者很难。
- 推荐下一步：用“给 MyFitnessPal switcher 的简单 macro tracker”定位，先做人工/半自动导入，找 50 个 beta 用户测试。

## 开发者假设

- 平台：iOS 优先。
- 时间预算：2 周 MVP 原型，不是完整生产级 tracker。
- 技术栈：SwiftUI、本地数据库、barcode API 或手动搜索、CSV 导入/导出。
- 地区/语言：先做美国/英国英语用户。
- 获客优势：Reddit、SEO、App Store 关键词、alternative to MyFitnessPal 内容。

## 品类快照

- 品类：卡路里计算、macro tracking、饮食记录、营养 dashboard。
- 目标用户：减重用户、运动人群、macro tracker、GLP-1 用户、营养师客户。
- 用户任务：快速记录食物、达成卡路里/macro 目标、扫码、追踪体重、规划饮食、导出历史。
- 变现方式：免费 + 订阅、高级 barcode/语音/拍照记录、年费。

## 证据

| 信号 | 来源 | 说明 | 质量 |
|---|---|---|---|
| MyFitnessPal 在 Google Play 显示 100M+ 下载、2.87M 评论、4.4 分、IAP，并且是 Health & Fitness #2 top grossing。 | [MyFitnessPal Google Play](https://play.google.com/store/apps/details?hl=en&id=com.myfitnesspal.android) | 需求和变现极强，但竞争也极强。 | 强 |
| MyFitnessPal Premium+ 包含 meal planning、grocery lists、voice logging、meal scan、barcode scanner 和 GLP-1 medication reminders。 | [MyFitnessPal Premium+ help](https://support.myfitnesspal.com/hc/en-us/articles/34347930588557-Premium), [MyFitnessPal App Store](https://apps.apple.com/us/app/myfitnesspal-calorie-counter/id341232718) | 头部产品正在从记录扩展到规划和 AI 辅助输入。 | 强 |
| Lose It 在 App Store 有 753K 评分、4.8 分，Premium 提供 photo meal logging、AI voice、barcode scanning、advanced tracking、fasting 和 meal planning。 | [Lose It App Store](https://apps.apple.com/us/app/lose-it-calorie-counter/id297368629) | 当工作流足够简单时，用户愿意为营养工具付费。 | 强 |
| Cronometer Gold 定价为 $10.99/month 或 $59.99/year，并强调 verified/lab-analyzed foods、图表、barcode scanning、voice log、recipe importer 和 custom targets。 | [Cronometer Gold](https://cronometer.com/gold/index.html) | 存在愿意为准确性付费的高端用户。 | 强 |
| MacroFactor Nutrition 定价为 $11.99/month、$47.99/half-year 或 $71.99/year。 | [MacroFactor subscription docs](https://help.macrofactorapp.com/en/articles/393-how-macrofactor-subscriptions-and-bundles-work) | 严肃 macro 用户愿意为 coaching 和算法追踪付费。 | 强 |
| 2026 年 Reddit 讨论显示，用户对 MyFitnessPal redesign 有明显负面反馈，并讨论迁移到 Cronometer 或替代品。 | [r/Myfitnesspal update thread](https://www.reddit.com/r/Myfitnesspal/comments/1steb4o/hate_the_new_app_wont_be_renewing/), [r/Myfitnesspal design feedback](https://www.reddit.com/r/Myfitnesspal/comments/1te5ix7/finally_updated_today_and_yikes_submitted_this/) | redesign 时存在切换意图。 | 中 |

## 竞品矩阵

| 产品 | 平台 | 定位 | 变现 | 优势 | 弱点 / 抱怨 | 机会缺口 |
|---|---|---|---|---|---|---|
| MyFitnessPal | iOS/Android/Web | 大型营养和健身追踪器 | 免费 + Premium/Premium+ | 巨大食物数据库、品牌、集成、top-grossing 信号 | redesign、复杂、premium gating 抱怨 | 简单的 MFP switcher UX |
| Lose It | iOS/Android | 减重 calorie tracker | 免费 + Premium | 友好 UX、拍照/语音/barcode 功能 | 用户提交食物带来准确性问题 | 可信食物和重度用户工作流 |
| Cronometer | iOS/Android/Web | 准确性和微量营养素 | 免费 + Gold | verified food database 和深度营养 | 对轻量用户可能太技术化 | 简单的可信记录 |
| MacroFactor | iOS/Android | Macro tracker 和 diet coach | 付费订阅 | 严肃 coaching algorithm 和付费用户群 | 没有免费轻量层 | 更轻、更便宜的 tracker |

## 痛点模式

1. 用户更想要快速记录，而不是复杂 dashboard。
2. Redesign 和肌肉记忆变化会触发迁移。
3. 用户提交的食物数据带来准确性问题。
4. Barcode、拍照、语音、meal planning 正成为高级功能战场。
5. 完整食物数据库是独立开发者最大的门槛。

## 机会想法

| 想法 | 用户切口 | 分数 | 为什么可能成立 | 主要风险 |
|---|---|---:|---|---|
| 简单的 MFP switcher macro tracker | 不满头部产品的重度用户 | 77 | 切换触发清晰，品类付费强，SEO 角度明确 | 食物数据库覆盖 |
| GLP-1 饮食耐受记录 | GLP-1 用户 | 74 | 新兴工作流明确，直接竞争较少 | 医疗表述和隐私 |
| Verified-foods 极简 tracker | 注重准确性的用户 | 70 | Cronometer 证明准确性有价值 | 数据库成本和覆盖 |

## 推荐 MVP

- 一句话概念：给想离开 MyFitnessPal 的用户做一个快速 macro tracker，强调简单记录、可信食物和干净导出。
- 必备功能：手动食物记录、保存常用餐、从 MyFitnessPal CSV 导入、macro 目标、体重趋势、常见食品 barcode 查询、导出。
- 暂不做：社交 feed、运动记录、meal delivery、AI recipe planner、巨大社区数据库。
- 定价假设：早鸟 $19/year，包含终身导入/导出。
- 获客切口：“给怀念旧版 MyFitnessPal 的人，一个安静的 macro tracker。”

## 7 天验证计划

| 天数 | 动作 | 成功信号 |
|---:|---|---|
| 1 | 发布面向 MFP switcher 的 landing page | 100 个 waitlist signup |
| 2 | 在 MFP/Cronometer/Lose It 社区发对比 mockup | 20 条评论提到具体迁移需求 |
| 3 | 做 CSV 导入 PoC | 正确导入 3 份样例食物日志 |
| 4 | 访谈 10 个不满用户 | 5 个表示愿意为干净迁移付费 |
| 5 | 测试 $19/year preorder | 5 个付费预订或强购买意向 |
| 6 | 原型化每日记录流程 | 8/10 用户 30 秒内记录早餐 |
| 7 | 决定构建范围 | 只有 import/export 是明确 hook 时继续 |

## 风险和未知

- Barcode 数据库和餐厅食品数据可能昂贵或不完整。
- 减重和 GLP-1 定位需要谨慎健康免责声明。
- MyFitnessPal 和 Lose It 可以快速改善 UI。
- 如果没有 SEO/社区牵引，App Store 获客可能很贵。

## 最终建议

不要做通用 calorie tracker。先验证一个小的、迁移优先的 tracker，服务对 MyFitnessPal 不满的用户；只有当导入/导出和快速记录被证明有粘性时再扩展。
