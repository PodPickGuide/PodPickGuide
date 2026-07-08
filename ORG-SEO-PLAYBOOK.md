# GitHub Organization SEO Playbook — PodPick Guide

## 核心思路

GitHub 不是放代码的地方，而是 **公开数据库 + 搜索引擎入口**。

Google 现在非常喜欢结构化、可引用的公开数据源。Organization 比个人账号更有 **品牌实体感**。

## 架构：一主题一仓库

```
PodPickGuide (Organization)
│
├── .github                    ← Org Profile README（首页）
├── PodPickGuide               ← 枢纽索引
├── podpick-flavour-index      ← 口味索引（关键词：disposable vape flavours）
├── vape-comparison-data       ← 品牌对比（关键词：Alibarbar vs HQD）
├── pod-flavour-ranking        ← 排行榜（关键词：best pod flavours 2026）
├── pod-faq-database           ← FAQ 数据集
└── pod-buying-guides-data     ← 选购指南索引
```

**千万不要建空仓库。** 每个仓库至少包含：
- SEO 优化的 README（含 Version / Last Updated / Sources 表）
- `/data/*.json` 机器可读数据
- 互链到其他仓库 + podpickguide.com

## 每个 README 的 SEO 模板

```markdown
# [目标关键词] — [副标题]

## Meta
| Version | 1.0.0 |
| Last Updated | 2026-07-08 |
| Sources | podpickguide.com/... |

## [数据表格 — Google 最爱 Markdown Table]

## Machine-Readable Data
- data/xxx.json

## Related Repositories
[互链表]
```

## GitHub Topics（每个仓库设置）

```
vape, pod-system, flavour-guide, disposable-vape,
sp2s, alibarbar, buying-guide, public-dataset
```

## Organization 创建步骤

1. 前往 https://github.com/organizations/plan 创建 **PodPickGuide** Organization（Free）
2. 将以下仓库从 `aozhou792` **Transfer** 到 Organization：
   - podpick-flavour-index
   - vape-comparison-data
   - pod-flavour-ranking
   - pod-faq-database
   - pod-buying-guides-data
   - PodPickGuide
3. 在 Org 下创建 `.github` 仓库，放入 `profile/README.md`
4. 更新所有 README 中的链接：`aozhou792` → `PodPickGuide`

## 与网站互链

在 podpickguide.com 页脚添加：

```html
<a href="https://github.com/PodPickGuide">Data on GitHub</a>
```

在网站 JSON-LD Organization 中添加：

```json
"sameAs": ["https://github.com/PodPickGuide"]
```

## 更新节奏

| 频率 | 动作 |
|------|------|
| 每次实测更新 | 改 JSON → 改 version → 写 CHANGELOG → push |
| 每月 | 检查 Google Search Console 中 github.com 来源流量 |
| 每季度 | 新增仓库（如 `pod-troubleshooting-data`）扩展关键词覆盖 |

## 为什么比单仓库好？

| 单仓库（上次做的） | Organization 多仓库 |
|-------------------|---------------------|
| 1 个 URL 承载所有关键词 | 每个仓库独立排名不同关键词 |
| Google 视为 1 个页面 | 6+ 个独立入口 |
| 无品牌实体感 | Organization = 品牌实体 |
| 无 Org Profile 首页 | `.github/profile/README.md` = 组织首页 |

## 当前状态

- ✅ GitHub Organization `PodPickGuide` 已创建
- ✅ 6 个主题仓库已迁移至 Organization
- ✅ Org Profile README 已部署（`.github` 仓库）
- ⏳ 需在 podpickguide.com 添加互链
