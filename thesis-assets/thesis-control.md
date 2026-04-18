# thesis-control

## 使用方式

- 这是你的唯一总控视图。
- 你只需要维护“当前阶段、当前卡点、下一步缺什么”这几个最小信息。
- 其余章节写作、文献整理、测试组织、答辩材料生成默认由 Codex 推进。
- 若当前阶段所需资料已齐，我会直接继续，不需要你重复下指令。
- 当前工程搭建阶段已临时切换为“一次性连续实施”：完成项目搭建、UI 设计、测试与审查后统一交付，不再中途形成断点。
- 在每个阶段内，若有助于提升质量与效率，我会适当、合理地调用本地 skills 与 MCP 工具完成检索、抽取、核验、格式化与交叉比对；但不会用工具替代真实证据，也不会脱离你已确认的项目边界自行补造事实。

## 当前阶段

- 当前主任务：完整 MVP 收尾实施
- 当前卡点：无阻塞；正在按一次性交付要求完成后端流式对话、报告生成、前端 UI、构建测试与最终审查
- 下一步需要我提供的材料：暂无；真实模型成功链路和论文实测数据可在项目可运行后再补
- 当前阶段审查状态：待完整 MVP 统一交付后审查

## 资料状态

- 学校要求包：已提供
- 文献包：已提供（待你审查）
- 素材包：未提供 / 补充中 / 已提供
- Bug 包：未提供 / 补充中 / 已提供
- 答辩包：未提供 / 补充中 / 已提供

## 当前产出

- 已完成：
  - 项目根目录 `.gitignore`
  - 项目根目录 `README.md`
  - 后端 Maven 工程骨架
  - 前端 Vite + Vue 3 工程骨架
  - 后端配置文件、建表脚本与初始化数据
  - 前端路由、状态管理、基础页面与流式组合式函数骨架
  - 后端统一返回体、业务异常、全局异常处理
  - 后端 JWT 工具、认证拦截器、用户上下文、跨域配置与 SSE 线程池
  - 后端注册 / 登录接口
  - 前端 Axios 拦截器、Pinia 登录态、路由守卫与登录注册页联调代码
  - 后端简历上传、PDFBox 文本提取、DeepSeek 同步解析封装与简历列表接口
  - 前端简历上传页、解析结果展示与简历列表
  - 后端岗位列表、面试会话创建、system 消息初始化与历史会话查询接口
  - 前端岗位选择弹窗、发起面试入口与面试页会话信息展示
  - 后端流式对话接口、上下文截断、`[DONE]` 收口与 AI 回复落库
  - 后端评估报告生成接口与会话状态流转
  - 前端 `fetch + ReadableStream` 流式状态机
  - 前端面试页、报告页和答辩专业感 UI 重构
  - 完整 MVP 测试记录
  - 完整 MVP 审查报告
  - 学校级论文管理办法与撰写规范提取
  - 学校要求包首版整理
  - 第一批中文文献证据映射表初版
  - 第一批英文文献初筛与合并
  - 第一批 BibTeX 草稿
  - 第一章绪论草稿
  - 第二章相关技术综述草稿
  - 第三章系统分析与设计草稿
  - 第四章系统实现草稿
  - 第五章系统测试草稿
  - 第六章总结与摘要草稿
  - 全卷打磨与格式核查报告
  - 参考文献整理与引文落位方案首版
  - 第一章引文落位首轮修订
  - 第六章摘要测试表述收稳
  - 官方来源清单首版
  - 第二章引文扩展
  - 第四章引文扩展
  - 第六章局限段引文扩展
  - 官方网络资源参考文献草案
  - 正文内部痕迹清理清单
  - 第一轮低风险清稿记录
  - 第四章谨慎清稿记录
  - 第三章与第五章条件性清稿策略
  - 终稿前最终补料清单
- 待我审核：
  - 面试会话断点是否通过审查
  - 简历解析断点是否接受“DeepSeek Key 待补”的边界状态
  - 基础设施 + 认证断点是否通过审查
  - 工程初始化断点是否通过审查
  - 第三章正式清稿
  - 第五章正式清稿
- 下一轮目标：
  - 完成最终构建、接口边界验证、敏感信息检查和 MVP 审查报告
- 当前待你审查的交付物：
  - thesis-assets/interview-session-breakpoint-report.md
  - thesis-assets/resume-breakpoint-report.md
  - thesis-assets/auth-breakpoint-report.md
  - thesis-assets/project-init-breakpoint-report.md
  - thesis-assets/citation-placement-plan.md
  - thesis-assets/official-source-register.md
  - thesis-assets/official-network-references-draft.md
  - thesis-assets/internal-trace-cleanup-checklist.md
  - thesis-assets/low-risk-cleanup-round1-report.md
  - thesis-assets/cautious-cleanup-round2-report.md
  - thesis-assets/conditional-cleanup-strategy.md
  - thesis-assets/final-supplement-checklist.md
  - thesis-assets/final-mvp-test-record.md
  - thesis-assets/final-mvp-review-report.md
  - thesis-assets/chapter-02-related-tech-draft.md
  - thesis-assets/chapter-04-implementation-draft.md
  - thesis-assets/chapter-01-introduction-draft.md
  - thesis-assets/chapter-06-conclusion-abstract-draft.md

## Codex 推进规则

1. 我默认按当前阶段推进，直到形成一个可审查交付物。
2. 通常情况下，每个阶段完成后我必须先提醒你进行人工审查，不会直接跨到下一阶段。
3. 当前完整 MVP 收尾实施已获你明确授权合并断点，因此本轮以“完成后统一交付”为准；若你退回修改，我会先完成修改再重新提交审查。
4. 只有在缺少真实证据时，我才会通知你补材料。
5. 在每个阶段中，我可以合理调用 skills 与 MCP 工具提升质量与效率，例如：
   - 用文献检索类工具补英文文献、题录与 BibTeX
   - 用 PDF 读取与抽取能力整理学校文件、论文与报告
   - 用浏览或检索工具核验公开资料
   - 用本地技能做结构化检查、语言打磨与格式辅助
   但所有阶段产出仍以真实材料和你已确认的信息为准。
6. 我通知你时只会说明：
   - 当前卡在哪一步
   - 还缺哪一类资料
   - 最低需要补什么
   - 补完后我会继续完成什么

## 阶段断点规则

建议按以下断点提交人工审查：

1. 文献整理完成后：
   - 交付文献证据映射表
   - 交付分主题归纳结果
2. 第一章完成后：
   - 交付第一章正文草稿
3. 第二章完成后：
   - 交付第二章正文草稿
4. 第三章完成后：
   - 交付第三章正文草稿
5. 第四章完成后：
   - 交付第四章各模块正文
6. 第五章完成后：
   - 交付测试章节与测试表
7. 第六章完成后：
   - 交付总结与中英文摘要
8. 全卷打磨完成后：
   - 交付润色、逻辑、引用、格式核查结果
9. 答辩材料完成后：
   - 交付开场白、PPT 大纲、题库与演练材料

> 若你没有明确批准，我默认停在当前阶段，不自动进入下一阶段。
