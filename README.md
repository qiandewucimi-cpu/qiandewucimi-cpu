# 陈源浩 · qiandewucimi-cpu

**FDE / AI 应用工程方向** · 用 Agent 解决真实业务问题

把"BOM → 采购 PO"这类高频、易错、依赖人工核对的流程，改造成**模型编排工具、确定性代码兜底**的 Agent 应用——这是我最想做的事。

## 项目

| 项目 | 一句话 | 技术栈 |
|---|---|---|
| [erp-procurement-agent](https://github.com/qiandewucimi-cpu/erp-procurement-agent) | 外贸 ERP 安全操作 Agent：自然语言生成采购 PO，写前确认、幂等、审计、回滚 | FastAPI · Streamlit · MCP · RAG · SQLite · Docker |
| [story-pages](https://github.com/qiandewucimi-cpu/story-pages) | 实例驱动的叙事故事网页生成器：一份 JSON 生成完整故事页，构建期隔离校验 | React 19 · Vite 7 · TypeScript |
| [fde-mentor](https://github.com/qiandewucimi-cpu/fde-mentor) | 面向 Codex 的 FDE 教学 Skill：按能力设计路线，练习必须真实验证 | Python · Skill · CI |
| [togethertrip](https://github.com/qiandewucimi-cpu/togethertrip) | 隐私优先的家庭旅行规划器：固定锚点 + 家庭分流 + 交通优化 | React 19 · Cloudflare Workers |
| [douyin-favorites-knowledge-skill](https://github.com/qiandewucimi-cpu/douyin-favorites-knowledge-skill) | 抖音收藏转本地知识笔记：转写 + OCR + 可恢复队列，本地优先 | faster-whisper · PaddleOCR · SQLite |
| [intelligent-data-analysis-assistant](https://github.com/qiandewucimi-cpu/intelligent-data-analysis-assistant) | 本地 Excel/CSV 智能分析助手：问答 + 图表 + 报告，默认脱敏 | Streamlit · pandas · LLM |

## 技术栈

![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?logo=react&logoColor=black)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?logo=github-actions&logoColor=white)

MCP · RAG · SQLite · Streamlit · Faster-Whisper · PaddleOCR

## 做事方式

- 每个项目都带：测试、CI、隐私声明
- 强调安全边界：AI 只编排，金额、校验、写入由确定性代码完成
- 数据边界清晰：合成数据、本地优先、敏感内容不进仓库

## 联系

qiandewucimi@gmail.com
