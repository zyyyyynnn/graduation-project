# 同步决策报告

## 同步范围

- 输入 Word：`thesis-assets/毕业论文正式版（草稿）.docx`
- 输入报告：`thesis-assets/process/sync/md-word-sync-report.md`
- 输入 Markdown：`abstract-keywords.md`、`chapter-01` 至 `chapter-06`
- 输出目录：`thesis-assets/process/sync/`

## 采用决策

| 文件 | 采用来源 | 决策 |
| --- | --- | --- |
| `abstract-keywords.sync.md` | Word | 保留 Word 的 `摘要`、英文题名、`Abstract`、关键词结构；未写入 Markdown 中间标题 `摘要与关键词`、`中文摘要`、`English Abstract`。 |
| `chapter-01.sync.md` | Word | 第一章以 Word 主稿为准，纳入 Word 独有段落和当前引用编号。 |
| `chapter-02.sync.md` | Word | 第二章以 Word 主稿为准，纳入 Word 独有段落和当前引用编号。 |
| `chapter-03.sync.md` | Word | 第三章以 Word 主稿为准，纳入 Word 独有边界说明、图 3.1 至图 3.3 图题及当前引用编号。 |
| `chapter-04.sync.md` | 人工合并 | 以 Word 为骨架，保留 Word 独有内容；补入已核实的用户级模型配置管理、模型配置连通性测试、简历解析输入长度保护说明，并同步更新本章小结中的实现证据描述。 |
| `chapter-05.sync.md` | 人工合并 | 以 Word 为骨架，Node.js 保持 Word 的 `v24.15.0`；已核实存在 `/api/user/llm-config/test`，因此补入 LLM 配置连通性测试说明和测试结论口径。 |
| `chapter-06.sync.md` | Markdown | 以 Markdown 为主，保留其工程稳定性、测试边界和展望段落；按 Word 当前参考文献顺序调整第六章引用编号。 |

## 已核实实现项

- 用户级 LLM 配置管理：代码和文档中存在 Provider、模型、用户 API Key 保存逻辑，后端路径包含 `GET/PUT /api/user/llm-config`。
- LLM 配置连通性测试接口：后端存在 `POST /api/user/llm-config/test`，前端 `testUserLlmConfig()` 调用该接口；真实模式发起轻量模型调用，Demo 模式返回固定可用状态。
- 简历解析输入长度保护：`ResumeServiceImpl` 中存在 `MAX_LLM_PARSE_TEXT_LENGTH = 12000`，保存完整 `rawText`，提交模型解析前通过 `limitText` 截断并追加截断提示。

## 需人工确认

- 本轮未发现必须强行排除正文的未核实系统功能。
- 仍需人工在 Word 侧最终整合时确认目录域、页码、图题表题格式、参考文献格式是否符合学校模板要求。

## 未执行事项

- 未修改原始 Word。
- 未修改原始 Markdown。
- 未自动润色正文。
- 未新增事实、数据、文献或系统功能。
