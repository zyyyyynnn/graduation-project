# 第六章 总结与展望及中英文摘要

## 6.1 总结与展望

本文围绕“基于大语言模型的沉浸式模拟面试与简历诊断系统”展开研究与实现，围绕高校毕业生在简历准备、面试训练与过程反馈方面的现实需求，构建了一套覆盖简历解析、岗位驱动问答、流式交互和总结评估的完整业务闭环。系统以前端 Vue 3 与后端 Spring Boot 3 为基础框架，结合 MySQL 进行业务数据持久化管理，并调用 DeepSeek API 完成结构化提取、动态问答生成与评估报告输出。在实现路径上，系统首先通过 PDFBox 提取用户简历文本，再借助大语言模型完成技能与项目经历的结构化抽取；随后，系统根据用户选择的岗位模板创建面试会话，并将岗位提示词作为系统消息纳入上下文；在多轮交互阶段，系统采用基于 `SseEmitter` 的流式推送机制，将模型增量生成内容实时返回前端；最后，系统依据完整会话历史生成结构化评估报告，帮助用户完成面试复盘与能力自查。

从整体结果看，本文所实现的系统在技术链路上完成了“PDF 简历解析与结构化提炼—岗位模板驱动的动态面试启动—多轮上下文感知的流式对话—AI 生成评估报告”的闭环设计，能够较好体现大语言模型在求职训练场景中的辅助价值。与单纯的静态题库或一次性问答方式相比，该系统更加注重用户个体简历信息与岗位语境之间的关联，并通过流式反馈提升交互的即时性与沉浸感。同时，围绕系统实现，本文还从功能需求、数据库设计、流式交互机制和测试方案等方面进行了较为系统的论述，为后续进一步扩展和优化奠定了基础。

尽管如此，当前系统仍存在若干不足。首先，现有上下文管理策略主要采用固定消息数量截断方式，即保留首条系统消息与最近若干条对话记录。这种方法虽然能够有效控制 Token 消耗，但尚未引入摘要压缩或长期记忆机制，随着对话轮数增加，早期关键信息可能被丢弃，从而影响长程面试场景下的连贯性[4-5]。其次，大语言模型输出本身具有一定不确定性，系统目前尚未建立完备的内容过滤、事实核验与结果校正机制，因此在特定场景下仍存在幻觉风险和不稳定输出问题[4-5]。最后，当前系统交互形式仍以文本为主，虽然已经实现了流式问答与报告反馈，但尚未覆盖语音输入、语音播报、视频面试或非语言行为分析等更强沉浸式训练需求[3]。

基于上述不足，后续工作可从以下几个方向展开。其一，可引入基于摘要压缩或长期上下文管理的优化策略，在控制上下文长度的同时保留早期关键信息，以提升长轮次对话的稳定性与一致性[4-5]。其二，可围绕模型输出增加规则过滤、结果复检或外部知识约束机制，以降低幻觉风险并提高评估反馈的可信度[4-5]。其三，可进一步扩展系统的人机交互形式，例如结合 WebRTC、语音识别、语音合成及多模态模型能力，探索语音模拟面试、视频表达训练和非语言行为评估等更具沉浸感的训练方式[3]。总体而言，本文实现的系统已经完成了基础业务闭环，但在上下文管理、内容可靠性与多模态交互方面仍有较大的扩展空间。

## 中文摘要

随着就业竞争加剧和高校毕业生规模持续扩大，传统依赖人工经验与静态题库的求职训练方式已难以满足个性化、连续化和即时化的训练需求。针对这一问题，本文设计并实现了一种基于大语言模型的沉浸式模拟面试与简历诊断系统。系统采用 Vue 3、TypeScript、Spring Boot 3 与 MySQL 构建前后端业务框架，并结合 DeepSeek API、Apache PDFBox 与 SSE 流式通信机制，实现了简历解析、岗位驱动的多轮问答、流式面试交互与评估报告生成等核心功能。

在具体实现中，系统首先通过 PDF 文本提取与大语言模型结构化输出，对用户简历中的技能和项目经历进行提炼；随后根据岗位模板构建面试会话上下文，驱动模型围绕用户履历生成更具针对性的面试问题；在交互阶段，系统采用 `SseEmitter` 与前端流式接收机制实现增量式内容展示，以提升反馈即时性；在总结阶段，系统结合会话历史生成包含技术匹配度、表达清晰度、优势总结与改进建议的结构化报告。从系统设计与实现链路看，该系统已经形成较为完整的“简历诊断—模拟面试—结果反馈”业务闭环，能够支撑后续真实测试与功能验证工作的展开。

本文工作表明，大语言模型在求职训练场景中具有较好的应用潜力，但系统在长程上下文管理、内容可靠性与多模态交互方面仍存在进一步优化空间。后续可围绕摘要压缩、事实核验和语音化扩展等方向展开改进，以增强系统的稳定性、真实性与沉浸体验。

**关键词：** 大语言模型；模拟面试；简历解析；流式响应；上下文管理

## English Abstract

With the intensifying competition in the job market and the continuous growth in the number of university graduates, traditional interview preparation methods based on manual guidance and static question banks can no longer fully satisfy the needs for personalized, continuous, and timely training. To address this problem, an immersive mock interview and resume diagnosis system based on large language models is designed and implemented in this study. The system is built with Vue 3, TypeScript, Spring Boot 3, and MySQL, while DeepSeek API, Apache PDFBox, and Server-Sent Events are integrated to support resume parsing, position-oriented multi-turn interviewing, streaming interaction, and automated report generation.

In the implementation process, resume text is first extracted from PDF files and then transformed into structured information, including skills and project experience, with the assistance of a large language model. On this basis, interview sessions are initialized with position templates so that subsequent questions can be generated according to both the target role and the user’s resume context. During the interview process, incremental model outputs are pushed to the front end through streaming communication, which improves immediacy and interaction continuity. After the interview is finished, the dialogue history is reorganized to produce a structured evaluation report covering technical matching, clarity of expression, strengths, and improvement suggestions. From the perspective of system design and implementation, the system has formed a relatively complete business loop covering resume diagnosis, mock interview interaction, and result feedback, which provides a basis for subsequent real-world testing and verification.

The study demonstrates that large language models have practical potential in job interview training scenarios. However, limitations still remain in long-context management, output reliability, and multimodal interaction. Future work may focus on summary-based context compression, fact verification, and the integration of speech and multimodal technologies to improve system robustness, credibility, and immersion.

**Keywords:** large language model; mock interview; resume parsing; streaming response; context management
