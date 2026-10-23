---
name: growth-playbook
description: 覆盖 52 个营销子技能的全链路增长作战手册。面向营销计划与 GTM、定位与竞品、文案与内容、SEO 与 AI 搜索、付费广告与创意、CRO 与 A/B 测试、注册/引导/付费墙、邮件与短信、推荐与联盟、B2B 外呼与销售赋能、分析与归因。适用于制定营销方案、诊断转化漏斗、优化落地页与广告、规划内容与搜索增长、设计生命周期与留存策略。需要营销策略或任一营销子领域时加载；纯工程开发、财务审计等与营销无关的任务不触发。
license: MIT
metadata:
  display_name: 增长作战手册
  sub_skills: "52"
  clis: "66"
  integrations: "101"
---

# 增长作战手册（Growth Playbook）

面向 AI 智能体的营销方法论库，内含 **52 个可按需加载的子技能**，覆盖从市场策略到渠道执行、从获客到留存的完整链路，另附带 **66 个零依赖 CLI 脚本**与 **101 份平台接入指南**。

本入口文件只负责识别任务与路由；具体方法论、模板、检查清单和脚本都在对应子技能中。

## 工作方式（必读）

1. 先判断请求属于哪个营销环节，再从下方路由表选出 **1–3 个**最相关的子技能。
2. 打开并**完整阅读**所选子技能的 `SKILL.md`，再按它的指引读取其 `references/`、`assets/` 或 `scripts/`。**不要只凭入口摘要执行**。
3. 多个子技能协同时，按「先策略 → 后执行 → 最后测量」的顺序阅读，避免不同子技能的建议互相冲突。
4. 子技能内的相对路径以该子技能目录为基准；**本技能根目录是 `SKILL.md` 所在目录**（即 `skills/growth-playbook/`）。
5. 需要真实平台数据或写入外部系统时，先确认凭据与授权；**没有数据就明确标注假设，不要编造指标**。

## 子技能路由

### 战略、定位与规划

- **marketing-plan** — 12 个月 AARRR 营销计划、GTM 路线图、市场测算、fCMO 方案。读 [SKILL.md](references/skills/marketing-plan/SKILL.md)
- **product-marketing** — 产品营销上下文：定位、ICP、品牌语调。读 [SKILL.md](references/skills/product-marketing/SKILL.md)
- **customer-research** — 客户访谈、ICP 研究、访谈与问卷结果综合。读 [SKILL.md](references/skills/customer-research/SKILL.md)
- **competitor-profiling** — 基于网址的竞品画像与竞争格局分析。读 [SKILL.md](references/skills/competitor-profiling/SKILL.md)
- **marketing-ideas** — 139 个营销点子与增长战术库。读 [SKILL.md](references/skills/marketing-ideas/SKILL.md)
- **marketing-council** — 由传奇营销大师组成的顾问团，多视角评审营销问题。读 [SKILL.md](references/skills/marketing-council/SKILL.md)
- **marketing-psychology** — 营销心理学、心智模型与行为科学。读 [SKILL.md](references/skills/marketing-psychology/SKILL.md)
- **offers** — Offer 设计：价值方程、赠品堆叠、保证、稀缺与紧迫感。读 [SKILL.md](references/skills/offers/SKILL.md)
- **pricing** — 定价、套餐结构、免费增值、试用与变现策略。读 [SKILL.md](references/skills/pricing/SKILL.md)
- **marketing-loops** — 可循环、可自动运行的营销工作流设计。读 [SKILL.md](references/skills/marketing-loops/SKILL.md)

### 内容、品牌与传播

- **copywriting** — 首页、落地页、定价页、功能页与产品页文案。读 [SKILL.md](references/skills/copywriting/SKILL.md)
- **copy-editing** — 文案审校、改写与旧内容翻新。读 [SKILL.md](references/skills/copy-editing/SKILL.md)
- **content-strategy** — 内容策略、选题规划与分发。读 [SKILL.md](references/skills/content-strategy/SKILL.md)
- **launch** — 产品发布、功能公告、Product Hunt 与发布节奏。读 [SKILL.md](references/skills/launch/SKILL.md)
- **lead-magnets** — 线索磁铁、内容升级包与邮件捕获。读 [SKILL.md](references/skills/lead-magnets/SKILL.md)
- **free-tools** — 免费工具营销，用工具获取线索与自然流量。读 [SKILL.md](references/skills/free-tools/SKILL.md)
- **events** — 活动、网络研讨会、会议赞助、演讲与活动 ROI。读 [SKILL.md](references/skills/events/SKILL.md)
- **social** — 社媒内容、排期、平台策略与社交聆听。读 [SKILL.md](references/skills/social/SKILL.md)
- **video** — AI 视频、程序化视频与短视频制作。读 [SKILL.md](references/skills/video/SKILL.md)
- **image** — 营销图像生成、编辑与优化。读 [SKILL.md](references/skills/image/SKILL.md)
- **public-relations** — 公关、媒体关系、记者外联与危机沟通。读 [SKILL.md](references/skills/public-relations/SKILL.md)
- **influencer-marketing** — 达人、创作者与品牌大使合作。读 [SKILL.md](references/skills/influencer-marketing/SKILL.md)
- **co-marketing** — 联合营销、伙伴筛选与联合活动。读 [SKILL.md](references/skills/co-marketing/SKILL.md)
- **community-marketing** — 社区策略、Discord/Slack 运营与社区增长。读 [SKILL.md](references/skills/community-marketing/SKILL.md)
- **directory-submissions** — 创业、SaaS、AI、MCP 等目录提交与外链曝光。读 [SKILL.md](references/skills/directory-submissions/SKILL.md)

### SEO 与搜索增长

- **seo-audit** — SEO 审计、技术 SEO、排名诊断与本地 SEO。读 [SKILL.md](references/skills/seo-audit/SKILL.md)
- **ai-seo** — AI 搜索优化、AEO/GEO，让内容被大模型引用。读 [SKILL.md](references/skills/ai-seo/SKILL.md)
- **programmatic-seo** — 用模板与数据规模化生成 SEO 页面。读 [SKILL.md](references/skills/programmatic-seo/SKILL.md)
- **schema** — Schema 标记、结构化数据与富媒体结果。读 [SKILL.md](references/skills/schema/SKILL.md)
- **site-architecture** — 站点层级、导航、URL 结构与内链。读 [SKILL.md](references/skills/site-architecture/SKILL.md)
- **link-building** — 外链建设、第三方提及与风险控制。读 [SKILL.md](references/skills/link-building/SKILL.md)
- **competitors** — 竞品对比页、替代页与买家决策内容。读 [SKILL.md](references/skills/competitors/SKILL.md)

### 付费广告与应用商店

- **ads** — Google、Meta、LinkedIn、TikTok 等付费广告投放与审计。读 [SKILL.md](references/skills/ads/SKILL.md)
- **ad-creative** — 广告标题、正文、素材与批量创意变体。读 [SKILL.md](references/skills/ad-creative/SKILL.md)
- **aso** — App Store 与 Google Play 商店优化。读 [SKILL.md](references/skills/aso/SKILL.md)

### 转化率与增长实验

- **cro** — 页面、表单与漏斗转化率优化。读 [SKILL.md](references/skills/cro/SKILL.md)
- **ab-testing** — A/B 测试设计、样本量与实验体系。读 [SKILL.md](references/skills/ab-testing/SKILL.md)
- **signup** — 注册、开户与试用激活流程。读 [SKILL.md](references/skills/signup/SKILL.md)
- **onboarding** — 新用户引导、激活率与首次价值体验。读 [SKILL.md](references/skills/onboarding/SKILL.md)
- **paywalls** — 应用内付费墙、升级页与功能门控。读 [SKILL.md](references/skills/paywalls/SKILL.md)
- **popups** — 弹窗、浮层、滑入与退出意图。读 [SKILL.md](references/skills/popups/SKILL.md)
- **churn-prevention** — 流失预防、取消挽留与失败付款回收。读 [SKILL.md](references/skills/churn-prevention/SKILL.md)
- **referrals** — 推荐计划、联盟计划与口碑机制。读 [SKILL.md](references/skills/referrals/SKILL.md)

### 生命周期消息

- **emails** — 邮件序列、滴灌活动与生命周期邮件。读 [SKILL.md](references/skills/emails/SKILL.md)
- **sms** — 短信、MMS 与 WhatsApp 营销。读 [SKILL.md](references/skills/sms/SKILL.md)

### B2B 与销售

- **cold-email** — B2B 冷邮件、跟进、多渠道触达与回复处理。读 [SKILL.md](references/skills/cold-email/SKILL.md)
- **prospecting** — 线索挖掘、资格筛选与目标名单构建。读 [SKILL.md](references/skills/prospecting/SKILL.md)
- **sales-enablement** — 销售物料、Pitch Deck、一页纸与异议处理。读 [SKILL.md](references/skills/sales-enablement/SKILL.md)
- **revops** — 收入运营、线索生命周期与市场到销售的交接。读 [SKILL.md](references/skills/revops/SKILL.md)

### 数据、追踪与归因

- **analytics** — GA4、事件追踪与分析体系建设。读 [SKILL.md](references/skills/analytics/SKILL.md)
- **conversion-tracking** — 转化追踪、GTM 配方、浏览器端与服务端追踪。读 [SKILL.md](references/skills/conversion-tracking/SKILL.md)
- **attribution** — 归因模型选择、跨工具数据对账与增量判断。读 [SKILL.md](references/skills/attribution/SKILL.md)

## 常用组合

- **从零制定营销方案**：product-marketing → customer-research → competitor-profiling → marketing-plan，再按计划调度渠道子技能。
- **落地页或注册不转化**：cro → copywriting → signup/onboarding → ab-testing → conversion-tracking。
- **付费投放起量与降本**：ads → ad-creative → conversion-tracking → attribution。
- **搜索与 AI 搜索增长**：seo-audit → content-strategy → ai-seo 或 programmatic-seo → schema → link-building。
- **SaaS 留存与增购**：onboarding → emails → paywalls → churn-prevention → referrals。
- **B2B 获客管线**：prospecting → cold-email → sales-enablement → revops → analytics。
- **新品发布**：launch → public-relations → social → directory-submissions → events。

## 执行约定

- **先读后做**：选定子技能后完整读取它的 `SKILL.md`；其中标为「read/reference」的文件只在当前步骤需要时再读，避免一次性塞满上下文。
- **路径映射**：子技能文档里的 `node tools/clis/xxx.js` 指本技能目录下的 `references/tools/clis/xxx.js`。执行时使用该文件的**绝对路径**。
- **平台连接**：`references/tools/integrations/` 下有 101 个平台的接入说明，`references/tools/clis/` 下是 66 个可直接运行的 CLI（Node 18+，零依赖）。调用外部平台前确认环境变量、账号权限与写操作范围；**只读诊断优先**。
- **数据诚实**：缺少预算、CAC、转化率等关键数据时，明确标注为假设或待确认项，**不用虚构数字补全方案**。
- **交付风格**：默认中文输出，保留必要的英文专业术语。营销方案、审计报告等交付物按子技能规定的结构产出，不擅自缩减关键章节。

## 目录

- `references/skills/<子技能>/SKILL.md` — 52 个子技能入口及各自的 references、assets、scripts。
- `references/tools/clis/` — 66 个营销平台命令行工具（GA4、Google Ads、Meta Ads、Ahrefs、Klaviyo 等）。
- `references/tools/integrations/` — 101 份平台接入与鉴权说明。
- `references/tools/REGISTRY.md` — 工具总表；`SETUP.md` — 凭据配置向导与安全边界说明。
- `references/tools/clis/README.md` — CLI 通用用法与环境变量约定。
