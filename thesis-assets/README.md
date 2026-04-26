# thesis-assets 论文材料目录

本目录用于存放毕业论文正文草稿、证据材料、文献材料、测试记录和答辩准备文件。

## 当前主文件

| 类型 | 文件 | 说明 |
| --- | --- | --- |
| 论文主稿 | `毕业论文正式草稿版.docx` | 当前主要维护的论文草稿；已完成文献增强；封面、诚信责任书和任务书仍为占位 |
| 历史快照 | `毕业论文资料整合版.docx` | 早期资料整合版，仅作历史快照，不作为正式提交依据 |
| 总控 | `thesis-control.md` | 当前状态唯一总控；状态冲突时优先参考本文件和 `final-evidence-lock.md` |
| 证据锁版 | `final-evidence-lock.md` | 记录截图、图表、测试、代码、文献和答辩证据是否同步 |
| 补料状态 | `final-supplement-checklist.md` | 记录终稿前已完成、预留待测和可选补充内容 |

## 文献材料

| 文件 | 说明 |
| --- | --- |
| `references-draft.bib` | 参考文献工作库；只写入可核验字段，不强行补造 |
| `literature-quality-review.md` | 文献质量评估表，记录采用/不采用依据 |
| `literature-evidence-map.md` | 文献证据映射表，记录文献与章节落位关系 |
| `citation-placement-plan.md` | 早期引用落位方案，作为阶段记录 |
| `official-source-register.md` | 官方来源登记 |
| `official-network-references-draft.md` | 官方网络资源参考文献草案 |

## 章节草稿

| 文件 | 说明 |
| --- | --- |
| `chapter-01-introduction-draft.md` | 第一章绪论草稿 |
| `chapter-02-related-tech-draft.md` | 第二章相关技术综述草稿 |
| `chapter-03-analysis-design-draft.md` | 第三章系统分析与设计草稿 |
| `chapter-04-implementation-draft.md` | 第四章系统实现草稿 |
| `chapter-05-testing-draft.md` | 第五章系统测试草稿 |
| `chapter-06-conclusion-abstract-draft.md` | 第六章总结与展望草稿 |
| `abstract-keywords.md` | 中英文摘要与关键词 |

## 图表、测试和实现证据

| 目录/文件 | 说明 |
| --- | --- |
| `diagrams/` | 第三章 Mermaid 源文件和 PNG 图表 |
| `figure-table-register.md` | 图表编号登记表 |
| `test-data/` | 第五章测试环境、业务测试和性能采集记录 |
| `code-snippets/` | 第四章核心实现证据 |
| `bug-evidence/` | 真实 Bug 证据 |
| `bug-package-2026-04-24.md` | Bug 复盘材料 |

## 答辩材料

| 文件 | 说明 |
| --- | --- |
| `defense-package-2026-04-25.md` | 答辩材料包 |
| `defense-slide-map.md` | PPT 页级映射表 |
| `defense-script-5-8min.md` | 5-8 分钟答辩讲稿 |

## 放置规则

- `毕业论文正式草稿版.docx` 是当前主稿；后续修订应覆盖该文件。
- `毕业论文资料整合版.docx` 只保留为历史快照，原则上不再维护。
- 新增文献材料优先放入 `references-draft.bib`、`literature-quality-review.md` 和 `literature-evidence-map.md`。
- 新增截图、图表、测试或代码证据后，应同步更新 `final-evidence-lock.md`。
- 不提交 Office 临时锁文件、一次性 ZIP 包和本地备份文件。

## 仍需人工确认

- 学校/学院正式封面模板。
- 诚信责任书正式模板。
- 毕业论文（设计）任务书正式模板。
- 是否需要真实公网 LLM 性能测试。
- 是否需要按导师要求调整答辩 PPT 页数和结构。
