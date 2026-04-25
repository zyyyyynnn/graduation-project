# 终稿前补料状态表

## 说明

本表用于锁定论文终稿前资料状态。当前已从“补料清单”切换为“已完成 / 预留待测 / 可选补充”口径，避免与证据锁版记录和第五章测试数据互相矛盾。

## A. 已完成项

| 类别 | 内容 | 证据位置 | 状态 |
| --- | --- | --- | --- |
| 第三章图表 | 系统整体架构图、系统核心用例图、数据库 E-R 图 | `thesis-assets/diagrams/`、`thesis-assets/figure-table-register.md` | 已完成 |
| 第五章测试环境 | Windows、PowerShell、JDK、Maven、Node.js、npm、MySQL、浏览器和网络环境 | `thesis-assets/test-data/test-evidence-2026-04-24.md` | 已完成 |
| Demo 业务测试 | `TC-01` 到 `TC-09` 功能测试结果 | `thesis-assets/test-data/demo-business-test-2026-04-25.md` | 已完成 |
| Demo 性能采集 | SSE TTFB、SSE 总耗时、PDF 上传/解析接口耗时 | `thesis-assets/test-data/demo-business-test-2026-04-25.md` | 已完成 |
| 构建验证 | 后端 `mvn -q test`、前端 `npm run build` | `thesis-assets/test-data/test-evidence-2026-04-24.md` | 已完成 |
| 实现证据 | SSE 推送、PDF 解析、上下文截断核心代码片段 | `thesis-assets/code-snippets/implementation-evidence-2026-04-24.md` | 已完成 |
| Bug 复盘 | Demo 代理错连、MySQL 启动前置校验 | `thesis-assets/bug-package-2026-04-24.md`、`thesis-assets/bug-evidence/` | 已完成 |
| 答辩基础材料 | 演示路线、亮点、难点、追问问答、风险预案 | `thesis-assets/defense-package-2026-04-25.md` | 已完成 |

## B. 本轮新增整合项

| 类别 | 内容 | 目标文件 | 状态 |
| --- | --- | --- | --- |
| 答辩页映射 | PPT 页码、页面主题、证据材料、对应论文章节和讲解要点 | `thesis-assets/defense-slide-map.md` | 本轮补齐 |
| 正式讲稿 | 5-8 分钟答辩讲稿 | `thesis-assets/defense-script-5-8min.md` | 本轮补齐 |
| 论文资料整合版 | 六章正文、图表、截图、测试、代码、Bug、答辩材料、参考文献整合为 DOCX | `thesis-assets/毕业论文资料整合版.docx` | 本轮补齐 |

## C. 预留待测项

| 类别 | 当前口径 | 是否阻塞终稿 |
| --- | --- | --- |
| 真实公网 LLM 性能 | 当前第五章仅采用 Demo Twin 本机闭环测试数据；公网模型响应性能受网络、模型服务负载和上下文长度影响，后续如需要性能对比再单独采集。 | 不阻塞当前整合版 |

## D. 可选补充项

| 类别 | 建议 | 使用场景 |
| --- | --- | --- |
| DevTools Network 截图 | 如导师要求更强测试证据，可补接口耗时截图。 | 第五章或答辩追问 |
| 数据库截图 | 可补 `interview_message`、`interview_session` 表截图。 | 第四章实现或数据持久化说明 |
| PPT 初稿 | 根据 `defense-slide-map.md` 生成正式 PPT。 | 答辩前 |
| 学校模板 | 如拿到学院封面、诚信书、任务书模板，再迁移为正式提交版 Word。 | 终稿排版 |
