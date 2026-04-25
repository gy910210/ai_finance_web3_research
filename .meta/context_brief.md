# Context Brief — Agentic Finance Research System & 交易Agent

生成时间：2026-04-17  
版本：v0.1（初稿，无现有材料，纯目标驱动）

---

## 1. 概览

| 字段 | 内容 |
|------|------|
| 研究目标 | 梳理"Agentic Finance Research System"与"交易Agent"两个方向的技术现状、代表工作与开放问题 |
| 时间窗口 | 2024-01 ~ 2026-04（重点覆盖最近一年） |
| 产出类型 | 中文增量探索稿（Markdown，落盘到项目目录） |
| 现有材料 | **无**（全新项目，零起点） |
| 版本链 | 本次为 v0.1 初稿 |

---

## 2. 核心研究问题

### 方向 A：Agentic Finance Research System
- LLM/Agent 如何替代或增强量化研究员的工作流（数据获取→因子挖掘→策略生成→回测→报告）？
- 有哪些端到端的金融研究 Agent 框架（FinAgent、FinRobot、TradingGPT 等）？
- 多Agent协同如何在金融研究中分工（数据Agent、分析Agent、报告Agent）？
- 金融专属 benchmark 有哪些（FinBench、FinQA、TAT-QA、ConvFinQA 等）？

### 方向 B：交易Agent（Trading Agent）
- 基于 LLM 的自主交易Agent的决策机制是什么（ReAct、CoT、Tool Use）？
- 强化学习与 LLM 如何结合用于交易（RLHF、RLAIF、DPO in finance）？
- 风险控制、仓位管理、执行优化在 Agent 架构中如何建模？
- 多模态输入（新闻、财报、价格序列、图表）如何融合？
- 现有交易Agent的实盘/模拟盘验证情况如何？

---

## 3. 种子术语

**核心概念：** Agentic Finance, LLM Trading Agent, Financial Research Agent, Multi-Agent System for Finance, FinLLM, Autonomous Trading, AlphaAgent

**技术组件：** ReAct, Tool Use, RAG, Chain-of-Thought, RLHF, Function Calling, Memory Module, Reflection

**评估维度：** Sharpe Ratio, Max Drawdown, Alpha Generation, Latency, Hallucination Rate, Task Completion Rate

**关键 Benchmark：** FinBench, FinQA, TAT-QA, ConvFinQA, FinanceBench, FLARE, BBF (Bloomberg Finance)

---

## 4. 种子来源（待验证）

| 类型 | 来源 |
|------|------|
| 论文库 | arXiv cs.AI + q-fin, ACL Anthology, NeurIPS/ICML/ICLR 2024-2025 |
| 代码库 | FinAgent, FinRobot, TradingGPT, FinGPT, Storm (Stanford), OpenBB |
| 官方资料 | Anthropic/OpenAI 金融案例, Bloomberg AI, JPMorgan AI Research |
| 综述 | "A Survey of LLMs for Finance" 系列 |

---

## 5. 已有结论

**无**（全新项目）

---

## 6. 未解问题 / Open Questions

- [ ] FinRobot vs FinAgent：架构差异与性能对比
- [ ] 交易Agent在真实市场的可复现验证结果是否可信？
- [ ] 多Agent框架相比单Agent是否有显著收益？
- [ ] LLM 幻觉在金融决策中的风险量化方法？
- [ ] 监管合规与可解释性在Agent架构中如何处理？

---

## 7. 约束与偏好

- 证据分级：直接证据 > 邻近证据 > 综合判断
- 不可靠来源需标注，待验证假设单独列出
- 输出中文，术语保留英文原名并附括号说明
- 不覆盖旧稿，仅增量追加

---

## 8. 下一步

→ 交棒 `literature-scout-zh`：按上述种子术语与时间窗口检索论文与官方资料
