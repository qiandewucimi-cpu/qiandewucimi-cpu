# 陈源浩

**2027届本科生 · AI 应用交付 / FDE 方向**

上海理工大学 · 管理科学｜上海，可出差 / 驻场

从业务现场的问题出发，把流程拆成明确的对象、操作边界和验收标准，再用 AI 辅助完成原型与测试迭代。已有外贸 ERP 现场和 AI 招聘产品客户服务实习经历。

## 代表项目

### 01 · [外贸采购 Agent](https://github.com/qiandewucimi-cpu/erp-procurement-agent)

把反复核对物料、数量和金额的 BOM 流程，转为可预览、可审批、可追溯的采购草稿。
- **我的工作：**梳理业务流程、定义模型与人工的操作边界、设计验收场景，并根据实际测试反馈推进修复。
- **关键设计：**模型编排工具，确定性代码计算金额和校验；使用合成数据与 SQLite，未接入生产 ERP。
- **查看：**[64秒执行回放](https://github.com/qiandewucimi-cpu/erp-procurement-agent/blob/main/docs/demo/README.md) · [离线验证与边界](https://github.com/qiandewucimi-cpu/erp-procurement-agent/blob/main/docs/验证索引.md) · [架构决策](https://github.com/qiandewucimi-cpu/erp-procurement-agent/blob/main/docs/03_架构决策记录_ADR.md)

### 02 · [企业培训知识库问答](https://github.com/qiandewucimi-cpu/smart-qa-assistant)

把分散的文档和截图整理成可检索的知识，通过飞书回答业务问题并提供来源。
- **我的工作：**明确资料范围和脱敏要求，用业务问法测试回答、追问与拒答，推动术语对照和入口迭代。
- **关键证据：**公开历史评测与失败分析；私有语料不公开，离线验收与在线问答验证分开说明。
- **查看：**[架构与演示](https://github.com/qiandewucimi-cpu/smart-qa-assistant/blob/main/docs/架构与演示.md) · [评测证据](https://github.com/qiandewucimi-cpu/smart-qa-assistant/blob/main/eval/README.md)

### 03 · [LLM 数据分析助手](https://github.com/qiandewucimi-cpu/intelligent-data-analysis-assistant)

用自然语言完成 CSV / Excel 分析，将生成的 Pandas 代码放入受限子进程执行。
- **我的工作：**提出数据与执行边界，设计分析问题、核对统计口径，并通过 Web / CLI 实测反馈问题。
- **关键证据：**18 题历史评测首轮通过 15 题，保留失败归因；本地执行，模型调用仍涉及信息外发，具体范围见项目说明。
- **查看：**[快速运行](https://github.com/qiandewucimi-cpu/intelligent-data-analysis-assistant#快速开始) · [设计取舍](https://github.com/qiandewucimi-cpu/intelligent-data-analysis-assistant/blob/main/docs/DESIGN_DECISIONS.md) · [历史评测](https://github.com/qiandewucimi-cpu/intelligent-data-analysis-assistant/blob/main/analyzer/evals/results/eval_report.md)

## 本人贡献与实现方式

我主要负责业务问题发现、需求与边界定义、方案取舍、实际测试和失败反馈。项目代码使用 AI 开发工具辅助实现；公开仓库展示原型与验证材料，具体生产接入和效果以各项目说明为准。

## 相关经历

- **外贸 ERP / DLS 数据助理**：参与 BOM、报价、核料和订单流转，处理字段兼容与导入问题。
- **AI 招聘产品客户成功实习生**：参与企业客户配置、试测跟进、问题答疑与数据复盘。

[完整背景与实践](docs/背景与实践.md)

## 其他实践

| 项目 | 内容 |
|---|---|
| [story-pages](https://github.com/qiandewucimi-cpu/story-pages) | JSON 驱动的叙事网页生成器 · [在线示例](https://qiandewucimi-cpu.github.io/story-pages/) |
| [TogetherTrip](https://github.com/qiandewucimi-cpu/togethertrip) | 家庭旅行规划器，组织固定事项、成员分流与预算 |
| [fde-mentor](https://github.com/qiandewucimi-cpu/fde-mentor) | 面向 Codex 的 FDE 教学 Skill 与练习验证 |
| [抖音收藏知识提取](https://github.com/qiandewucimi-cpu/douyin-favorites-knowledge-skill) | 本地转写、关键帧筛选、OCR 与可恢复队列 |

## 联系

投递邮箱：Qiandewucimi@163.com
