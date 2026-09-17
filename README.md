# 陈源浩 · qiandewucimi-cpu

**2027届本科生 · Forward Deployed Engineer（FDE）/ AI应用解决方案 / 交付工程师方向** · 上海，可出差 / 驻场
上海理工大学 管理科学（本科）｜国家励志奖学金 · 专业前21%

具备AI招聘产品客户服务与外贸ERP现场经历，能够深入业务现场梳理流程，将问题转化为需求、业务对象、操作边界和验收标准；以 **AI-native** 方式推进知识沉淀、原型实现、测试验收与迭代反馈，推动AI应用从业务问题走向可验证方案。

我的主要贡献集中在：**业务问题发现、需求与边界定义、方案取舍、实际测试、失败反馈和持续迭代**。项目原型使用AI开发工具辅助实现；以下指标均来自项目产物或本地测试，并保留当前验证边界。

## 精选项目

### 企业培训知识库问答助手 · LLM Wiki / GLM-4V OCR / 飞书WebSocket

面向培训资料分散、格式不统一和敏感信息混杂的问题，定义“资料可检索、回答可溯源、语料外不编造”的验收目标。

- **知识构建**：处理173份、153MB多源资料及633张截图，识别并处理8类敏感信息4,667处，形成121份、约105万字符脱敏语料；通过GLM-4V OCR提取截图内容，将119份去重语料编译为822页可溯源Wiki
- **检索与交互**：使用引擎内置的关键词与图谱扩展检索，支持来源引用和知识范围外拒答；以飞书长连接机器人作为员工问答入口
- **测试迭代**：使用真实业务问题测试正常问答、多轮追问和语料外拒答；发现用户提问与知识库术语不一致后，推动补充术语对照，5个专项问题由全部未命中提升至命中4个
- **当前边界**：[脱敏工程代码与评测材料已开源](https://github.com/qiandewucimi-cpu/smart-qa-assistant)；企业原始资料、私有知识库实例与真实运行数据不公开

### [erp-procurement-agent](https://github.com/qiandewucimi-cpu/erp-procurement-agent) · 外贸ERP安全操作Agent

源自外贸ERP实习中多款式BOM人工复核金额、单耗和字段兼容问题，使用合成数据构建BOM→采购单原型。

- **业务建模**：参考Ontology的“对象—关系—动作”方法，梳理BOM、物料、供应商、采购草稿和审批记录，以及“生成草稿—人工确认—审批—写入”的动作边界
- **Agent方案**：模型负责理解意图和编排工具；金额计算、业务校验及最终写入由确定性代码处理。通过Function Calling调用解析、校验、草稿生成和审批工具，并提供HTTP、MCP及飞书入口
- **知识检索**：内置基于Markdown标题切块与中文Bigram词面匹配的轻量RAG，用于采购规则检索、来源引用和知识范围外拒答
- **验证结果**：完成98项单元测试、核心包覆盖率89%及25条CI安全评测；本人端到端实测并推动修复“金额明细仍返回总额、确认后无响应”等回归问题
- **当前边界**：SQLite用于离线验证，HTTP API为ERP接入预留；项目不连接生产ERP，使用合成数据，模型不参与金额计算、业务校验和最终写入

### [intelligent-data-analysis-assistant](https://github.com/qiandewucimi-cpu/intelligent-data-analysis-assistant) · LLM数据分析沙箱引擎

源自在实习中处理后台导出数据和调研问卷汇总表的经历，希望减少Excel重复清洗和网页操作摩擦。

- **需求与边界**：提出自然语言分析、CLI入口、数据不直接外发和生成代码不裸跑等要求；默认仅向模型发送列结构与脱敏统计
- **受控执行**：生成的Pandas代码经AST白名单校验，禁止导入模块、文件读写等高风险操作，再放入一次性子进程执行；以超时、内存限制和进程树终止控制风险，结果仅以JSON回传
- **评测结果**：建立覆盖六类任务的18题基线评测集，GLM-4-Flash首轮正确15/18（83.3%），P50为16.4秒；3个失败均集中于问句理解，因此将下一轮重点确定为问句拆解
- **实际测试**：本人测试Web与CLI入口，推动修复启动报错和本地与GitHub版本不一致问题

## AI-native实践与ANC理解

我理解的AI-native，不是把AI当作末端插件，而是让AI进入知识沉淀、任务执行、人工确认、测试反馈和能力迭代的完整流程。

我关注开源项目 **[AI Native Company（ANC）](https://github.com/HA7CH/ai-native-company)** 提出的“共享知识层、一人一Agent、Skill迭代闭环”思路。目前的项目分别实践了Markdown知识库、飞书入口、工具调用、人工确认及回归评测，但**尚未完整部署ANC框架，也不将ANC作为本人开发的项目**。

## 其他项目

| 项目 | 一句话 | 技术栈 |
|---|---|---|
| [story-pages](https://github.com/qiandewucimi-cpu/story-pages) | 以JSON驱动的叙事故事网页生成器，加入构建校验和产物隔离 | React 19 · Vite 7 · TypeScript |
| [fde-mentor](https://github.com/qiandewucimi-cpu/fde-mentor) | 面向Codex的FDE教学Skill，按能力设计路线并要求练习真实验证 | Python · Skill · CI |
| [togethertrip](https://github.com/qiandewucimi-cpu/togethertrip) | 隐私优先的家庭旅行规划器，支持固定锚点、家庭分流和交通优化 | React 19 · Cloudflare Workers |
| [douyin-favorites-knowledge-skill](https://github.com/qiandewucimi-cpu/douyin-favorites-knowledge-skill) | 串联本地语音转写、关键帧筛选与OCR，形成可恢复的知识化流程 | Faster-Whisper · PaddleOCR · SQLite |

## 实习经历

**DLS数据助理** · 上海荣恒国际贸易｜2026.07–2026.09

- 梳理BOM导入、样板单、报价单、订单理单及采购核价的系统流转，沉淀订单理单全流程汇报与操作规范
- 处理多款式BOM中的首行说明、中英混排和主数据缺失问题，按款式拆分并规范字段，形成3份ERP可导入文件
- 独立完成5份报价单和4份核料单并推动技审通过；结合一线痛点提出企业知识库与ERP Agent原型方案

**客户成功实习生** · 北京牛客科技（AI招聘产品）｜2026.03–2026.07

- 直面3家企业客户、累计支持8家以上客户，完成产品配置、客户试测跟进、问题答疑与效果复盘
- 使用Excel、透视表及BI汇总20余家企业校招数据，制作客户复盘材料

**运营与教练** · Woodpark运动公园｜2025.10–2026.02

- 策划执行嘉兴、上海陆冲赛事，单场约60人并沉淀活动SOP；搭建Excel客流看板支持排期与运营复盘

## 能力与工具

- **业务与交付**：业务流程梳理、需求与边界定义、对象—关系—动作建模、客户沟通、测试验收及试点方案设计
- **AI应用**：RAG知识检索、来源引用、知识范围外拒答、LLM API、Function Calling、MCP及人工确认与审批机制
- **数据与技术**：Python、Pandas、SQL数据处理；了解FastAPI、HTTP API、Streamlit、SQLite、Docker Compose、Git及CI
- **原型与迭代**：使用AI开发工具推进原型实现，通过实际测试、失败反馈和回归验证推动迭代

![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?logo=github-actions&logoColor=white)

## 联系方式

Qiandewucimi@163.com（投递邮箱） · qiandewucimi@gmail.com（GitHub）
