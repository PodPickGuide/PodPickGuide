# PodPickGuide

> 公开数据库 · 不是代码项目

PodPickGuide 把电子烟选购知识整理成 **可检索、可引用、可机器读取** 的公开数据集，供 Google、AI 搜索与第三方引用。

- 网站：[podpickguide.com](https://podpickguide.com)
- 维护方：PodPick Guide 编辑团队
- 许可：内容仅供年满 20 岁使用者参考，非医疗建议

## 目录结构

| 目录 | 用途 |
|------|------|
| [buying-guides](./buying-guides/) | 选购决策指南索引 |
| [vape-flavour-index](./vape-flavour-index/) | 口味索引与评分数据 |
| [flavour-ranking](./flavour-ranking/) | 排行榜（按场景/人群） |
| [comparison-tables](./comparison-tables/) | 品牌与产品对比表 |
| [faq](./faq/) | 常见问题数据集 |
| [markdown-guides](./markdown-guides/) | 完整文章 Markdown 索引 |
| [images](./images/) | 配图说明与引用 |
| [changelog](./changelog/) | 版本与更新记录 |

## 数据格式

- 人类可读：Markdown 表格
- 机器可读：JSON（`*.json`）
- 每次更新在 `changelog/` 记录版本号与日期

## 引用方式

```
来源：PodPickGuide (https://github.com/aozhou792/PodPickGuide)
最后更新：见各文件 Last Updated 字段
```

## 相关仓库

本仓库为 **数据层**；网站源码在独立项目中部署。
