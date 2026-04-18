# 官方来源清单

## 说明

- 本清单用于管理第二章及后续参考文献整理中需要使用的官方文档或标准来源。
- 这些来源与研究论文分工不同：研究论文用于支撑“已有研究如何看待该问题”，官方文档用于支撑“该技术或框架本身如何定义、如何使用”。
- 本清单当前只记录已确认的官方来源入口与推荐使用位置，不等于已经完成最终 GB/T 7714-2015 排版。

## 已确认来源

### 1. Spring Boot Reference

- 来源名称：Spring Boot Reference
- 官方地址：[https://docs.spring.io/spring-boot/reference/index.html](https://docs.spring.io/spring-boot/reference/index.html)
- 核验日期：2026-04-12
- 适用位置：
  - 第二章 `2.4 Spring Boot 3 异步编程模型`
  - 后续参考文献网络资源条目整理
- 推荐用途：
  - Spring Boot 参考文档入口
  - `Task Execution and Scheduling`
  - Web 应用与任务执行能力说明

### 2. Vue 3 Guide Introduction

- 来源名称：Introduction | Vue.js
- 官方地址：[https://vuejs.org/guide/introduction](https://vuejs.org/guide/introduction)
- 核验日期：2026-04-12
- 适用位置：
  - 第二章 `2.3 Vue 3 Composition API`
  - 后续参考文献网络资源条目整理
- 推荐用途：
  - Vue 3 官方入门说明
  - Options API 与 Composition API 的官方对比入口

### 3. Apache PDFBox

- 来源名称：Apache PDFBox - A Java PDF Library
- 官方地址：[https://pdfbox.apache.org/](https://pdfbox.apache.org/)
- 核验日期：2026-04-12
- 适用位置：
  - 第二章 `2.5 Apache PDFBox 3.0`
  - 后续参考文献网络资源条目整理
- 推荐用途：
  - PDFBox 开源属性
  - 文本提取能力
  - 官方主页与功能简介

### 4. DeepSeek API Docs

- 来源名称：DeepSeek API Docs
- 官方地址：[https://platform.deepseek.com/api-docs](https://platform.deepseek.com/api-docs)
- 核验日期：2026-04-12
- 适用位置：
  - 第二章 `2.1 大语言模型技术概述`
  - 第四章流式调用实现说明
  - 后续参考文献网络资源条目整理
- 推荐用途：
  - DeepSeek 聊天接口说明
  - 流式能力说明
  - 与 OpenAI 协议兼容的接口使用说明
- 备注：
  - 当前抓取环境可确认该官方文档入口 URL 存在，但页面正文在当前抓取结果中未完整展开。
  - 在最终整理网络资源参考文献时，可直接使用该官方 URL；若后续需要页内更细粒度引注，可再人工打开页面补核具体标题。

### 5. HTML Standard: Server-Sent Events

- 来源名称：HTML Standard - Server-Sent Events
- 官方地址：[https://html.spec.whatwg.org/multipage/server-sent-events.html](https://html.spec.whatwg.org/multipage/server-sent-events.html)
- 核验日期：2026-04-12
- 适用位置：
  - 第二章 `2.2 Server-Sent Events 技术`
  - 后续参考文献网络资源条目整理
- 推荐用途：
  - `EventSource` 接口定义
  - `text/event-stream` 事件流规范
  - SSE 标准来源说明

## 当前使用策略

### 研究文献优先用于

- 研究背景
- 国内外研究现状
- 多轮对话风险
- 简历解析与语义匹配研究进展
- 多模态/多智能体训练系统发展方向

### 官方来源优先用于

- 框架功能定义
- 协议机制说明
- API 接口能力说明
- 开源授权与工具功能简介

## 下一步建议

在后续“参考文献整理”阶段，可基于本清单继续做两件事：

1. 将这些官方来源统一整理成符合学校要求的网络资源条目。
2. 为第二章涉及框架原理的段落补入正式引用，而不是继续用研究论文替代官方来源。
