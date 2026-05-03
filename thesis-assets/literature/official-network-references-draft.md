# 官方网络资源参考文献草案

## 说明

- 本文件用于整理第二章及后续参考文献中需要使用的官方网络资源条目。
- 当前格式按 GB/T 7714-2015 的网络资源思路先行整理，便于后续直接转入论文参考文献列表。
- 访问日期统一按本轮核验日期 `2026-04-15` 记录。
- 若学校对网络资源条目有更细的本地格式要求，后续以学校要求为准。

## 草案条目

[1] Spring. Spring Boot Reference[EB/OL]. [2026-04-15]. https://docs.spring.io/spring-boot/reference/index.html.

[2] Vue.js. Introduction | Vue.js[EB/OL]. [2026-04-15]. https://vuejs.org/guide/introduction.

[3] Apache PDFBox. Apache PDFBox - A Java PDF Library[EB/OL]. [2026-04-15]. https://pdfbox.apache.org/.

[4] DeepSeek. DeepSeek API Docs[EB/OL]. [2026-04-15]. https://platform.deepseek.com/api-docs.

[5] WHATWG. HTML Standard: Server-sent events[EB/OL]. [2026-04-15]. https://html.spec.whatwg.org/multipage/server-sent-events.html.

## 推荐挂接位置

- `[1]`：
  - 第二章 `2.4 Spring Boot 3 异步编程模型`
  - 后续正文中涉及 `ThreadPoolTaskExecutor`、任务执行与调度机制的位置

- `[2]`：
  - 第二章 `2.3 Vue 3 Composition API`
  - 后续正文中涉及 Composition API 官方定义与组织方式的位置

- `[3]`：
  - 第二章 `2.5 Apache PDFBox 3.0`
  - 后续正文中涉及 PDF 文本提取工具来源与开源属性的位置

- `[4]`：
  - 第二章 `2.1 大语言模型技术概述`
  - 第四章流式调用实现说明
  - 后续正文中涉及 DeepSeek 聊天接口、流式能力与 API 兼容性的描述

- `[5]`：
  - 第二章 `2.2 Server-Sent Events 技术`
  - 后续正文中涉及 `EventSource`、事件流规范与 SSE 标准定义的位置

## 当前注意事项

1. `[4] DeepSeek API Docs` 当前已确认官方 URL，可作为参考文献条目使用；若后续需要更细粒度到某个子页面标题，再单独补核。
2. `[5] HTML Standard` 更适合用于说明 `EventSource` 与事件流标准，不适合直接替代你对 `fetch + ReadableStream` 工程选型的整段论证。
3. 这些条目当前仍是“网络资源草案”，还没有与正文编号系统最终对齐；正式排版时需统一编号。
