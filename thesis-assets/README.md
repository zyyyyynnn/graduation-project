# thesis-assets 论文材料目录

本目录用于存放毕业论文正文草稿、证据材料、文献材料、测试记录和答辩准备文件。

## 当前主文件

| 类型 | 文件 | 说明 |
| --- | --- | --- |
| 论文主稿 | `毕业论文正式版（草稿）.docx` | 当前主要维护的论文草稿；已完成文献增强；封面和诚信责任书仍为占位 |
| 历史快照 | `毕业论文资料整合.docx` | 早期资料整合版，仅作历史快照，不作为正式提交依据 |
| 总控 | `thesis-control.md` | 当前状态唯一总控；状态冲突时优先参考本文件和 `final-evidence-lock.md` |
| 证据锁版 | `final-evidence-lock.md` | 记录截图、图表、测试、代码、文献和答辩证据是否同步 |
| 补料状态 | `final-supplement-checklist.md` | 记录终稿前已完成、预留待测和可选补充内容 |
| 资料清单 | `material-checklist.md` | 五类资料包状态：学校要求、文献、素材、Bug、答辩 |

## 文献材料

| 文件 | 说明 |
| --- | --- |
| `references-draft.bib` | 参考文献工作库；已按正文首次引用顺序前置排序；只写入可核验字段，不强行补造 |
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
| `chapter-04-implementation-draft.md` | 第四章系统实现草稿；已补入简历解析输入长度保护表述 |
| `chapter-05-testing-draft.md` | 第五章系统测试草稿；已补入 LLM 配置连通性测试表述 |
| `chapter-06-conclusion-abstract-draft.md` | 第六章总结与展望草稿；已补入单用户本机验证、模型降级和报告结构化输出展望 |
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

## 阶段记录与历史文件

以下文件用于保留论文推进过程，不作为当前状态判断依据；当前状态以 `thesis-control.md`、`final-evidence-lock.md` 和本 README 为准。

| 文件类型 | 示例 | 处理规则 |
| --- | --- | --- |
| dated 阶段记录 | `thesis-next-step-2026-04-24.md`、`defense-package-2026-04-25.md` | 保留为阶段记录；如状态冲突，以当前总控为准 |
| breakpoint 报告 | `*-breakpoint-report.md` | 保留为开发审查记录；不作为当前任务清单 |
| cleanup 报告 | `*-cleanup-*.md`、`conditional-cleanup-strategy.md` | 保留为清稿过程记录；不作为终稿质量结论 |
| 早期引用方案 | `citation-placement-plan.md`、`official-network-references-draft.md` | 保留为阶段记录；正式文献状态以 `references-draft.bib` 和 `literature-quality-review.md` 为准 |
| 旧 DOCX | `毕业论文资料整合.docx` | 历史快照，不再维护，不覆盖当前主稿 |

## 放置规则

- `毕业论文正式版（草稿）.docx` 是当前主稿；后续修订应覆盖该文件。
- `毕业论文资料整合.docx` 只保留为历史快照，原则上不再维护。
- 新增文献材料优先放入 `references-draft.bib`、`literature-quality-review.md` 和 `literature-evidence-map.md`。
- 新增截图、图表、测试或代码证据后，应同步更新 `final-evidence-lock.md`。
- 新增阶段报告应优先使用日期命名，并在完成后视为阶段记录，不要替代总控文件。
- 不提交 Office 临时锁文件、一次性 ZIP 包和本地备份文件。

## 不建议现在移动的内容

- 不建议移动 dated 阶段记录，避免破坏已存在的交叉引用。
- 不建议再次重命名 `毕业论文正式版（草稿）.docx`，避免后续提交和答辩材料路径混乱。
- 不建议删除旧清稿报告，除非论文终稿和答辩材料均已完成。

## 仍需人工确认

- 学校/学院正式封面模板。
- 诚信责任书正式模板。
- 是否需要真实公网 LLM 性能测试。
- 是否需要按导师要求调整答辩 PPT 页数和结构。

## 当前任务书口径

- 已读取的论文设计管理办法当前未将任务书列入论文主稿装订顺序。
- 任务书不再作为当前终稿阻塞项或主稿占位项维护。
- 若学院、导师或系统提交页面另行要求任务书，再作为单独归档附件处理，不并入当前论文主稿口径。
