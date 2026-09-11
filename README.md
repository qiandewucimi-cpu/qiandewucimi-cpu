# 陈源浩 · qiandewucimi-cpu

**2027 届本科生 · AI 交付工程师（FDE）/ AI 解决方案方向** · 上海，可出差 / 驻场
上海理工大学 管理科学（本科）｜国家励志奖学金 · 专业前 21%

把"BOM → 采购 PO"这类高频、易错、依赖人工核对的流程，改造成**模型编排工具、确定性代码兜底**的 Agent 应用——这是我正在做的事，也是我最想做的事。

## 精选项目

**企业培训智能问答助手 · 飞书知识库机器人**（本地运行中，可现场演示）
把分散的培训资料变成群内 @ 即答的飞书机器人：答案强制带来源引用、免公网部署，支持多轮追问。

- 数据工程：173 份/153MB 资料清洗，OCR 566 张截图，产出 121 份/105.2 万字；8 类敏感信息脱敏 4,667 处、零残留
- 知识库：LLM-Wiki 编译式方法论，119 份语料编译为可溯源互链知识库，替代临时检索 RAG，支持一键重建
- 评测：自建 22 题六类评测集（概念/对比/流程/操作/报价配比/机制），脚本自动判定；batch1 基线：命中 11/15、幻觉 0/15（95% 置信上界 18.1%）、引用可溯源率 100%
- 落地：飞书自建应用机器人（WebSocket 长连接、免公网），群内 @ 即答，卡片展示答案与来源，支持多轮追问
- 状态：源码打磨中暂未开源，支持现场演示飞书机器人

**[erp-procurement-agent](https://github.com/qiandewucimi-cpu/erp-procurement-agent) · 外贸 ERP 安全操作 Agent（开源主推）**
基于实习场景、以合成数据构建 BOM→PO 原型：模型自主编排工具，金额计算、业务校验与写入口令由确定性代码兜底——断网或模型幻觉也不会造成错误写入。

- 技术：FastAPI · Streamlit · SQLite · Function Calling 工具循环 · FastMCP（7 工具）· RAG · Docker · Ollama 本地部署
- 质量：58 项单元测试 · 覆盖率 89% · 能力评测 15/15 · Docker 冒烟 8/8
- 安全：写前确认、幂等写入、审计回滚、异常 BOM 工具层阻断；密钥仅落 .env 并完成轮换
- 部署：支持 Ollama 本地离线与云端智谱；飞书长连接对话入口（免公网），支持文件直传与多轮上下文

**其他项目**

| 项目 | 一句话 | 技术栈 |
|---|---|---|
| [story-pages](https://github.com/qiandewucimi-cpu/story-pages) | 实例驱动的叙事故事网页生成器：一份 JSON 生成完整故事页，构建期隔离校验 | React 19 · Vite 7 · TypeScript |
| [fde-mentor](https://github.com/qiandewucimi-cpu/fde-mentor) | 面向 Codex 的 FDE 教学 Skill：按能力设计路线，练习必须真实验证 | Python · Skill · CI |
| [togethertrip](https://github.com/qiandewucimi-cpu/togethertrip) | 隐私优先的家庭旅行规划器：固定锚点 + 家庭分流 + 交通优化 | React 19 · Cloudflare Workers |
| [douyin-favorites-knowledge-skill](https://github.com/qiandewucimi-cpu/douyin-favorites-knowledge-skill) | 抖音收藏转本地知识笔记：转写 + OCR + 可恢复队列，本地优先 | faster-whisper · PaddleOCR · SQLite |
| [intelligent-data-analysis-assistant](https://github.com/qiandewucimi-cpu/intelligent-data-analysis-assistant) | 本地 Excel/CSV 智能分析助手：问答 + 图表 + 报告，默认脱敏 | Streamlit · pandas · LLM |

## 实习经历

**客户成功实习生** · 北京牛客科技（AI 招聘产品）｜2026.03–2026.07
- 服务 8+ 家企业客户，直连 3 家消费/宠物/教育行业客户：AI 寻聘产品配置、答疑、效果跟踪与试测复盘
- 基于 Excel/透视表/BI 产出材料，制作 20+ 家企业校招复盘 PPT 交付

**DLS 数据助理（实习）** · 上海荣恒国际贸易（外贸 ERP）｜2026.07–2026.09
- 梳理订单/理单/核料/核价全流程，拆解为 9 环节，输出 16 页考核汇报；处理多款式 BOM，输出 3 份可导入文件
- 完成 5 份报价单、4 份核料单并推动技审通过；提出飞书知识库与 ERP Agent 方案（实习后已落地为开源项目）

**运营 & 教练（实习）** · Woodpark 运动公园｜2025.10–2026.02
- 策划执行全国陆冲循环赛（单场 60 人），沉淀可复用活动 SOP；搭建 Excel 客流看板驱动排期

## 技术栈

![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?logo=react&logoColor=black)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?logo=fastapi&logoColor=white)
![Ollama](https://img.shields.io/badge/-Ollama-000000)
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?logo=github-actions&logoColor=white)

MCP · RAG · LLM-Wiki · SQLite · Streamlit · Ollama 本地部署 · Faster-Whisper · PaddleOCR · Function Calling · 飞书开放平台

## 荣誉

- 全国大学生统计建模大赛 · 二等奖
- 国家励志奖学金、学习优秀奖学金（多次）｜专业前 21%

## 做事方式

- 每个项目都带：测试、CI、隐私声明
- 安全边界：AI 只编排，金额、校验、写入由确定性代码完成
- 数据边界：合成数据、本地优先、敏感内容不进仓库
- AI 协作开发：主导需求、架构决策与质量把关，AI 承担编码实现

## 联系

Qiandewucimi@163.com（投递邮箱）· qiandewucimi@gmail.com（GitHub）
