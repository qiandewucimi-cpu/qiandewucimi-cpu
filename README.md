# 陈源浩 · qiandewucimi-cpu

**2027 届 · FDE（AI 交付工程师）** · 用 Agent 解决真实业务问题
正在寻找 FDE / AI 应用工程方向校招岗位 · 上海，可出差 / 驻场 / 客户现场交付

把"BOM → 采购 PO"这类高频、易错、依赖人工核对的流程，改造成**模型编排工具、确定性代码兜底**的 Agent 应用——这是我正在做的事，也是我最想做的事。

## 精选项目

**[erp-procurement-agent](https://github.com/qiandewucimi-cpu/erp-procurement-agent) · 外贸 ERP 安全操作 Agent（主推）**
自然语言对话即可生成采购 PO：模型自主编排工具，金额计算、业务校验与写入口令由确定性代码兜底——断网或模型幻觉也不会造成错误写入。

- 技术：FastAPI · Streamlit · SQLite · Function Calling Agent · MCP（7 个工具）· RAG · Docker
- 质量：58 项单元测试 · 覆盖率 89% · 能力评测 8/8 与 15/15 通过 · Docker 冒烟 8/8
- 部署：支持 Ollama 本地离线部署与云端智谱；可选飞书长连接机器人，免公网接入
- 演示与启动：见仓库 README（含 UI 工作台、Docker Compose、MCP 验证）

**[企业培训智能问答助手 · 飞书知识库机器人](https://github.com/qiandewucimi-cpu)（可现场演示）**
把分散的培训资料变成群内 @ 即答的飞书知识库机器人：资料清洗 + 截图 OCR + 编译式知识库，答案 100% 带来源引用，免公网部署。

- 数据：173 份资料清洗、566 张截图 OCR、8 类敏感信息脱敏、零残留
- 评测：自建 22 题六类评测集，实测幻觉率 0%
- 状态：本地运行中，源码打磨中暂未开源，支持现场演示飞书机器人

**其他项目**

| 项目 | 一句话 | 技术栈 |
|---|---|---|
| [story-pages](https://github.com/qiandewucimi-cpu/story-pages) | 实例驱动的叙事故事网页生成器：一份 JSON 生成完整故事页，构建期隔离校验 | React 19 · Vite 7 · TypeScript |
| [fde-mentor](https://github.com/qiandewucimi-cpu/fde-mentor) | 面向 Codex 的 FDE 教学 Skill：按能力设计路线，练习必须真实验证 | Python · Skill · CI |
| [togethertrip](https://github.com/qiandewucimi-cpu/togethertrip) | 隐私优先的家庭旅行规划器：固定锚点 + 家庭分流 + 交通优化 | React 19 · Cloudflare Workers |
| [douyin-favorites-knowledge-skill](https://github.com/qiandewucimi-cpu/douyin-favorites-knowledge-skill) | 抖音收藏转本地知识笔记：转写 + OCR + 可恢复队列，本地优先 | faster-whisper · PaddleOCR · SQLite |
| [intelligent-data-analysis-assistant](https://github.com/qiandewucimi-cpu/intelligent-data-analysis-assistant) | 本地 Excel/CSV 智能分析助手：问答 + 图表 + 报告，默认脱敏 | Streamlit · pandas · LLM |

## 实习经历

**客户成功实习生** · 牛客网（AI 招聘产品）｜2026.03–2026.07
- 直接对接 3 家客户、参与服务 8+ 家头部互联网及上市企业
- 负责 AI 寻聘产品部署与配置跟踪、客户答疑、模型效果调整与复盘，完成 10+ 份分析/复盘材料

**DLS 数据助理（实习）** · 上海荣恒国际贸易（外贸 ERP）｜2026.07–2026.08
- 培训/测试环境完成订单→理单→核价→配置 CP 全流程，独立输出 3 份系统可导入 BOM
- 将客户下单至理单拆解为 9 环节并完成脱稿考核汇报；提出 ERP Agent 构想，实习后已落地为开源项目

## 技术栈

![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?logo=react&logoColor=black)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?logo=fastapi&logoColor=white)
![Ollama](https://img.shields.io/badge/-Ollama-000000)
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?logo=github-actions&logoColor=white)

MCP · RAG · SQLite · Streamlit · Ollama 本地部署 · Faster-Whisper · PaddleOCR

## 做事方式

- 每个项目都带：测试、CI、隐私声明
- 安全边界：AI 只编排，金额、校验、写入由确定性代码完成
- 数据边界：合成数据、本地优先、敏感内容不进仓库
- AI 协作开发：主导需求、架构决策与质量把关，AI 承担编码实现

## 联系

qiandewucimi@gmail.com
