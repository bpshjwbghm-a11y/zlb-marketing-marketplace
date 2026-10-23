# 增长操盘官 Growth Operator

依托 52 个营销子技能，诊断增长漏斗、制定可执行方案、优化转化与投放、搭建可验证的测量体系。

## 类型

Agent 型（单个 AI 专家） · 行业分类：营销增长（05-MarketingGrowth）

## 功能

本专家挂载《增长作战手册》（`growth-playbook`），内含：

| 资源 | 数量 | 说明 |
|---|---|---|
| 营销子技能 | 52 | 覆盖战略定位、内容传播、SEO 与 AI 搜索、付费广告、CRO 与 A/B 测试、生命周期消息、B2B 销售、分析归因八大板块 |
| 平台 CLI | 66 | GA4、Google Ads、Meta Ads、Ahrefs、Semrush、Klaviyo、HubSpot 等，Node 18+ 零依赖 |
| 平台接入指南 | 101 | 各平台凭据配置、权限边界与常见操作 |

**核心机制**：渐进式披露。专家先判断问题属于哪个营销环节，再从手册路由到 1–3 个子技能并完整读取其方法论，避免上下文一次性塞满，也避免凭先验知识空谈。

**已剔除内容**：上游付费合作方（Converly / Ploy / AIsa / Omnia）的推荐表与专属集成文档已全部移除，避免向 Agent 注入商业倾向；中性的多工具横向对比均已保留。

## 使用示例

- 帮我诊断当前的增长漏斗，找出最该优先修复的环节，并给出可执行的改进方案。
- 为我的产品制定一份未来 12 个月的营销计划与 GTM 路线图。
- 审计这个落地页的转化率问题，并按优先级给出改写建议。

## 使用真实数据

CLI 脚本需要 Node 18+（零依赖）。凭据存放请遵循 `references/tools/SETUP.md`：使用本地环境变量或密钥管理，**切勿在对话中粘贴 token**。只读诊断优先，写操作须经明确授权。

## 头像

头像已自动生成在 `avatars/` 目录下。如需替换，要求：PNG/JPG、512×512 px、单张不超过 500KB。

## 目录结构

```
zlb-growth-operator/
├── .codebuddy-plugin/plugin.json    # 专家定义与展示字段
├── agents/growth-operator.md        # 专家人设与工作流程
├── skills/growth-playbook/          # 增长作战手册
│   ├── SKILL.md                     # 52 子技能路由层
│   └── references/
│       ├── skills/<52 个子技能>/
│       └── tools/{clis,integrations}/
├── avatars/expert.png
├── LICENSE.txt                      # 上游 MIT 许可证
└── README.md
```

## 打包分享

```bash
python3 scripts/package_expert.py <expert-dir>
```

## 溯源

方法论源自 coreyhaines31/marketingskills（MIT License），入口路由层为中文改写，子技能正文保留英文原文以保证模板完整性。
