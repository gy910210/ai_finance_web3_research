# Evidence Map — Agentic Finance Research System & 交易Agent

生成时间：2026-04-17  
来源：多轮 WebSearch，覆盖 arXiv、ACL、NeurIPS、KDD、ICAIF 等

---

## 方向 A：端到端金融AI研究系统框架

| # | 论文/资源 | 来源 | 类型 | 证据等级 | 要点 |
|---|-----------|------|------|----------|------|
| A1 | **FinRobot** — An Open-Source AI Agent Platform for Financial Applications using LLMs | [arXiv 2405.14767](https://arxiv.org/abs/2405.14767) · GitHub: AI4Finance-Foundation | academic · open-source | **直接** | 四层架构（Agent层/LLM算法层/LLMOps层/基础模型层）；7B-72B多模型评估；覆盖投研自动化、算法交易、风控 |
| A2 | **FinWorld** — All-in-One Open-Source Platform for End-to-End Financial AI Research | [arXiv 2508.02292](https://arxiv.org/abs/2508.02292) · TradeMaster-NTU | academic · open-source | **直接** | 统一支持 ML/DL/RL/LLM Agent 四类任务（时序预测/算法交易/组合管理/LLM应用）；800M+ 多模态样本；模块化架构 |
| A3 | **FinCon** — Synthesized LLM Multi-Agent System with Conceptual Verbal Reinforcement | [arXiv 2407.06567](https://arxiv.org/abs/2407.06567) · NeurIPS 2024 | academic | **直接** | 受真实投资机构结构启发，经理-分析师通信层级；"概念口头强化"提升决策；单股交易+组合管理均有效 |
| A4 | **LLM Agents for Investment Management** — Foundations, Benchmarks, Frontiers | [ACM ICAIF 2025](https://dl.acm.org/doi/10.1145/3768292.3770387) | academic · survey | **直接** | 覆盖组合优化/风险管理/信息检索/策略生成；含 benchmark 综述 |
| A5 | **FinGPT** — Open-Source Financial Large Language Models | [arXiv 2306.06031](https://arxiv.org/abs/2306.06031) · AI4Finance | academic · foundation model | **邻近** | 金融领域基础模型；RLHF+LoRA微调；情感分析、算法交易、robo-advising应用；持续更新至2025.11 |
| A6 | **MarketSenseAI 2.0** | 文献引用（无直接arxiv链接） | academic | **邻近** | RAG+LLM Agent 五专项分析（新闻/基本面/动量/宏观/信号生成）；CoT融合输出 |
| A7 | **Agentic AI in Financial Services** — Modeling and Model Risk Management | [arXiv 2502.05439](https://arxiv.org/abs/2502.05439) | academic · industry | **直接** | 金融服务中 Agentic 系统的建模流程与模型风险管理框架；human-in-the-loop 设计 |

---

## 方向 B：交易Agent（Trading Agent）

| # | 论文/资源 | 来源 | 类型 | 证据等级 | 要点 |
|---|-----------|------|------|----------|------|
| B1 | **TradingAgents** — Multi-Agents LLM Financial Trading Framework | [arXiv 2412.20138](https://arxiv.org/abs/2412.20138) · GitHub: TauricResearch | academic · open-source | **直接** | 7角色（基本面/情感/新闻/技术分析师、研究员、交易员、风控）；LangGraph；多LLM后端；Bull/Bear辩论机制；Sharpe↑ Drawdown↓ |
| B2 | **FinAgent** — Multimodal Foundation Agent for Financial Trading | [arXiv 2402.18485](https://arxiv.org/abs/2402.18485) · KDD 2024 | academic | **直接** | 首个多模态金融交易Agent（新闻+结构化价格+K线图）；工具增强+双层反射架构；对比12个SOTA基线平均提升36% |
| B3 | **FinMem** — Performance-Enhanced LLM Trading with Layered Memory | 文献引用 | academic | **邻近** | 分层记忆设计+角色设定；感知窗口微调；累积回报显著提升 |
| B4 | **AlphaAgents** — LLM Multi-Agents for Equity Portfolio Construction | [arXiv 2508.11152](https://arxiv.org/abs/2508.11152) · BlackRock | academic · industry | **直接** | BlackRock出品；三微Agent（基本面/情感/估值）；AutoGen框架；轮询辩论；风险偏好Prompt工程建模 |
| B5 | **Language Model Guided RL in Quantitative Trading** | [arXiv 2508.02366](https://arxiv.org/abs/2508.02366) · FLLM 2025 | academic | **直接** | LLM生成高层策略引导RL Agent；在4/6资产上优于纯RL基线；收益与风险指标均改善 |
| B6 | **TradingGroup** — Multi-Agent with Self-Reflection and Data-Synthesis | [arXiv 2508.17565](https://arxiv.org/abs/2508.17565) | academic | **直接** | 自我反射+数据合成机制；多Agent协同 |
| B7 | **Trade in Minutes** — Rationality-Driven Agentic System for Quantitative Financial Trading | [arXiv 2510.04787](https://arxiv.org/abs/2510.04787) | academic | **直接** | 理性驱动的量化交易Agentic系统 |
| B8 | **Can LLMs Trade?** — Testing Financial Theories with LLM Agents in Market Simulations | [arXiv 2504.10789](https://arxiv.org/abs/2504.10789) | academic | **直接** | 模拟市场中的LLM交易Agent验证；偏重理论检验 |
| B9 | **LLM Agents Do Not Replicate Human Market Traders** | [arXiv 2502.15800](https://arxiv.org/abs/2502.15800) | academic · contradiction | **反例** | 实验金融证据：LLM Agent与人类交易者行为存在系统性差异 |
| B10 | **TradeTrap** — Are LLM-based Trading Agents Truly Reliable? | [arXiv 2512.02261](https://arxiv.org/abs/2512.02261) | academic · evaluation | **直接** | 对抗性压力测试框架；假新闻注入/MCP工具劫持攻击；头寸集中度↑ 交易频率↑ 回撤↑；揭示可靠性缺陷 |

---

## 方向 C：综述与调查

| # | 论文/资源 | 来源 | 证据等级 | 要点 |
|---|-----------|------|----------|------|
| C1 | **LLM Agent in Financial Trading: A Survey** | [arXiv 2408.06361](https://arxiv.org/abs/2408.06361)，更新至2026.03 | **直接** | 架构分类：LLM as Trader vs LLM as Alpha Miner；覆盖数据输入/回测性能/挑战 |
| C2 | **LLM Agents in Finance: A Survey** | [EMNLP 2025 Findings](https://aclanthology.org/2025.findings-emnlp.972.pdf) | **直接** | EMNLP 2025；金融LLM Agent全景综述 |
| C3 | **Agentic Large Language Models: A Survey** | [arXiv 2503.23037](https://arxiv.org/abs/2503.23037) | **邻近** | 通用Agentic LLM架构与分类综述 |
| C4 | **AI Agents in Financial Markets** — Architecture, Applications, Systemic Implications | [arXiv 2603.13942](https://arxiv.org/abs/2603.13942) | **直接** | 系统性影响分析，含金融稳定性与监管讨论 |

---

## 方向 D：Benchmark 与评估

| # | 论文/资源 | 来源 | 证据等级 | 要点 |
|---|-----------|------|----------|------|
| D1 | **FinBen** — A Holistic Financial Benchmark for LLMs | [arXiv 2402.12659](https://arxiv.org/abs/2402.12659) · NeurIPS 2024 | **直接** | 42数据集/24任务/8维度；含股票交易评估；首个开源金融LLM评估基准；IJCAI 2024 & COLING 2025 共享任务 |
| D2 | **FinAgentBench** — Benchmark for Agentic Retrieval in Financial QA | 文献引用（2025） | **直接** | 专注金融Agent检索能力评估 |
| D3 | **XFinBench** — Complex Financial Problem Solving | [ACL 2025 Findings](https://aclanthology.org/2025.findings-acl.457.pdf) | **直接** | 研究生级金融题目；4235样本；多模态上下文 |
| D4 | **FinMaster** — Full-Pipeline Financial Workflow Benchmark | [arXiv 2505.13533](https://arxiv.org/abs/2505.13533) | **直接** | 全流程金融工作流评估 |
| D5 | **Open FinLLM Leaderboard** | [HuggingFace Blog](https://huggingface.co/blog/leaderboard-finbench) | **直接** | HuggingFace 托管的开放金融LLM榜单 |

---

## 方向 E：风险、治理与安全

| # | 论文/资源 | 来源 | 证据等级 | 要点 |
|---|-----------|------|----------|------|
| E1 | **The Agentic Regulator** — Risks for AI in Finance | [arXiv 2512.11933](https://arxiv.org/abs/2512.11933) | **直接** | 金融AI监管框架提案；涵盖Agent治理风险 |
| E2 | **Model Risk Management for GenAI in Finance** | [arXiv 2503.15668](https://arxiv.org/abs/2503.15668) | **直接** | 生成式AI的模型风险管理规范 |
| E3 | **TRiSM for Agentic AI** — Trust, Risk, Security | [arXiv 2506.04133](https://arxiv.org/abs/2506.04133) | **邻近** | 多Agent系统信任/风险/安全管理框架 |
| E4 | **FSB AI Monitoring Report** | [FSB 2025.10](https://www.fsb.org/uploads/P101025.pdf) | **直接** | 金融稳定委员会：AI在证券市场应用的监测报告 |

---

## 方向 F：产业官方信号

| # | 来源 | 类型 | 证据等级 | 要点 |
|---|------|------|----------|------|
| F1 | JPMorgan Chase — $18B AI战略，LLM Suite (OpenAI+Anthropic) 向25万员工开放 | [AI News](https://www.artificialintelligence-news.com/news/jpmorgan-chase-ai-strategy-2025/) | official · industry | **直接** | 投行级AI应用：30秒生成路演材料、自动起草M&A文件 |
| F2 | Anthropic — 面向金融服务发布专项软件套件 | [Bloomberg 2025.07.15](https://www.bloomberg.com/news/articles/2025-07-15/openai-rival-anthropic-courts-finance-industry-with-new-ai-tools) | official | **直接** | 针对金融分析师工作流优化 |
| F3 | OpenAI — 发布金融服务工具，竞争Anthropic市场 | [Bloomberg 2026.03.05](https://www.bloomberg.com/news/articles/2026-03-05/openai-releases-new-financial-services-tools-rivaling-anthropic) | official | **直接** | GPT-5.4；电子表格/文档/演示文稿生成 |
| F4 | BlackRock — AlphaAgents 研究 | arXiv 2508.11152 | industry · academic | **直接** | 顶级资管机构公开发布多Agent投研系统研究 |

---

## Support / Contradiction / Gap 视角小结

### 支持性证据（Support）
- 多Agent分工明显优于单Agent（TradingAgents, AlphaAgents, FinCon）
- LLM+RL混合优于纯RL（Language Model Guided RL）
- 多模态输入提升交易性能（FinAgent: +36%）
- 工业界大规模落地进行中（JPMorgan、BlackRock、Anthropic、OpenAI）

### 矛盾/反例（Contradiction）
- LLM Agent与人类交易者行为存在系统差异（arXiv 2502.15800）
- 对抗攻击下可靠性严重下降（TradeTrap: 假新闻注入导致大幅回撤）
- LLM在复杂推理任务上仍落后（FinBen评估结论）

### 空白/开放问题（Gap）
- 真实市场（非回测）的持续验证数据极少
- 监管合规的技术实现方案缺乏
- 多Agent协作中的噪声放大与错误传播机制
- 幻觉在金融决策中的定量风险建模
- 中文市场/A股场景的专项研究较少

---

## 优先精读队列

| 优先级 | 论文 | 理由 |
|--------|------|------|
| ⭐⭐⭐ | TradingAgents (2412.20138) | 架构最完整、可复现、开源；主稿核心 |
| ⭐⭐⭐ | FinAgent (2402.18485) | KDD 2024；多模态+反射；性能基准 |
| ⭐⭐⭐ | LLM Agent in Financial Trading: A Survey (2408.06361) | 最新综述（更新至2026.03）；分类框架完整 |
| ⭐⭐⭐ | FinBen (2402.12659) | NeurIPS 2024；评估基准必读 |
| ⭐⭐ | FinCon (2407.06567) | NeurIPS 2024；多Agent协同机制 |
| ⭐⭐ | AlphaAgents (2508.11152) | BlackRock背书；辩论机制+风险偏好建模 |
| ⭐⭐ | TradeTrap (2512.02261) | 可靠性与安全性；反例必读 |
| ⭐⭐ | Language Model Guided RL (2508.02366) | LLM+RL混合机制 |
| ⭐ | FinWorld (2508.02292) | 平台性工作；了解即可 |
| ⭐ | Agentic Regulator (2512.11933) | 监管视角；补充背景 |
