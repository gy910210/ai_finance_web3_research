# Context Brief — AI Finance × AI Web3 方向扩展

生成时间：2026-04-24
版本：v0.2（基于既有 Agentic Finance 项目增量扩展）

---

## 1. research_topic

在既有 `Agentic Finance Research System 与交易 Agent` 研究基础上，扩展为：
- AI Finance：金融研究/投研/交易/风控/合规/benchmark/工作流 agent
- AI Web3：agentic wallet、onchain copilot、DeFi / prediction market / payment agent、可信执行与身份层、crypto-native benchmark
- 重点不是泛泛“AI+金融/AI+区块链”，而是找出 2024-2026 最值得继续跟踪的方向簇、主线能力层与交叉地带。

---

## 2. domain_summary

当前项目已有较成熟的 AI Finance 主稿，重点覆盖：
- Agentic 金融研究系统（FinRobot / FinWorld / FinCon 等）
- 交易 Agent（FinAgent / TradingAgents / AlphaAgents / TradeTrap 等）
- Benchmark 与评估（FinBen / XFinBench / FinMaster 等）
- 风险、安全与治理

本轮新增目标：
- 把既有 AI Finance 主稿从“交易 Agent”扩展到“工作流 agent / assurance / risk-compliance / 文档证据编排”
- 新开 AI Web3 方向，不只看链上交易，而是看可执行层、支付层、可信层与评估层
- 找出 AI Finance 与 AI Web3 的公共能力栈：
  1. 研究与证据编排
  2. 风险约束与审计
  3. 可执行账户/支付/结算
  4. benchmark 与在线评估

---

## 3. user_constraints_and_preferences

- 默认中文输出
- 默认把结果落盘为 Markdown
- 不覆盖旧稿，先产出新稿或中间工件
- 明确区分：直接证据 / 邻近证据 / 综合判断 / 待验证假设
- 对 AI Finance 的新增方向，不要只停留在 trading alpha 叙事
- 对 AI Web3 的新增方向，不要泛泛而谈“AI+区块链”
- 优先寻找能与既有主稿衔接的方向，而不是完全平行的新领域

---

## 4. existing_files

| path | role |
|------|------|
| `INDEX.md` | 索引 |
| `agentic-finance-research-v0.1.md` | 主稿·增量探索稿 |
| `ai-trader-deep-dive.md` | 专题稿 |
| `.meta/context_brief.md` | 中间产物·旧版 context brief |
| `.meta/evidence_map.md` | 中间产物·旧版 evidence map |
| `.meta/paper_notes.md` | 中间产物·核心精读笔记 |
| `.meta/evidence_audit.md` | 中间产物·证据审校 |

---

## 5. existing_conclusions

### 已形成的高置信结论
- 现有 LLM 交易 Agent 文献仍以历史回测为主，缺乏实盘验证。
- 多 Agent / 多模态 / 反射机制是当前金融 agent 的主流技术路线。
- 风险、治理与对抗鲁棒性是交易 Agent 能否走向真实部署的核心瓶颈。
- FinBen / XFinBench / FinMaster 等 benchmark 表明金融场景需要专门化评估，而不能直接套通用 benchmark。

### 本轮新增的方向判断（暂作 agenda 级判断，非成熟结论）
- AI Finance 的下一阶段重点，可能从“autonomous trading”部分转向“evidence-grounded research workflow + risk/compliance/assurance”。
- AI Web3 的最高价值主线，可能不是一般性“AI+链”，而是：
  - agentic wallet / account abstraction
  - onchain copilot / DeFi research agent
  - payment / stablecoin / settlement agent
  - trusted execution / identity / provenance
  - crypto-native evaluation
- AI Finance 与 AI Web3 的重叠层，可能在“可控执行 + 风险约束 + 审计留痕 + 在线评估”。

---

## 6. open_questions

### AI Finance 增量问题
- 投研工作流 agent 的一手 benchmark / 官方产品化证据，哪些最值得纳入主稿？
- risk/compliance/copilot 与 model governance 的技术实现，是否已有较成体系的公开框架？
- 现有金融 benchmark 如何从“静态问答”升级为“workflow + assurance”评估？

### AI Web3 启动问题
- agentic wallet 的主流技术底座，哪些是标准、哪些是厂商实现？
- onchain copilot 与 autopilot 的边界如何划分？
- 哪些 Web3 方向最适合作为 AI Finance 的延伸，而不是平行支线？
- 是否存在值得单独深挖的 crypto-native benchmark / replay / simulation 评估路线？

### 交叉问题
- “研究—决策—执行—支付/结算—审计”能否成为 AI Finance × AI Web3 的统一分析框架？
- 可信执行、权限控制、session key、policy engine 能否构成跨两个方向的共用基础设施层？

---

## 7. seed_sources

### 既有 AI Finance 种子
- FinRobot / FinWorld / FinCon / FinAgent / TradingAgents / TradeTrap / FinBen / XFinBench / FinMaster
- FSB / IMF / Bloomberg 等既有产业与治理来源

### 新增 AI Finance 种子（需下一轮精确核验）
- FinanceBench
- Bloomberg / FactSet / S&P Global / Moody’s 等面向金融工作流的官方 AI 产品页面
- FSB / BIS / BoE / FCA / ECB / NIST 等治理与 assurance 来源

### 新增 AI Web3 种子（需下一轮精确核验）
- EIP-4337
- ERC-7579
- Safe 官方文档
- Coinbase AgentKit
- Circle Programmable Wallets
- Polymarket Docs
- Olas / Autonolas
- Phala / Oasis ROFL / Ritual / Bittensor

---

## 8. version_chain

```text
v0.1 — 2026-04-17
  主题：Agentic Finance Research System 与交易 Agent
  状态：主稿完成，AI-Trader 专题稿完成

v0.2 — 2026-04-24（本轮启动）
  主题：扩展为 AI Finance × AI Web3 方向图谱
  目标：先做 agenda + 种子 evidence map，再决定是否分成双主稿或“主稿 + Web3 专题稿”
```

---

## 9. initial_scope_decision

本轮暂不直接改写旧主稿，先生成：
1. 新的 research_agenda
2. AI Finance × AI Web3 的 seed evidence map
3. 下一轮 priority reading queue

待证据更稳定后，再决定：
- 方案 A：在原主稿中新增“AI Finance 新主线 + AI Web3 延展”章节
- 方案 B：保留原主稿为 AI Finance 主稿，另开 `report_ai_web3_directions_v0.1.md` 专题稿
- 方案 C：做一篇 `双视角稿` 或 `方向比较稿`

---

## 10. next_step

推荐下一步进入 `已有报告增量扩展` 主流程，并带一个 `概念边界辨析` 次流程：
- 主流程：把 AI Finance 主稿扩到 workflow / assurance / risk-compliance
- 次流程：界定 AI Finance 与 AI Web3 的交叉层、边界层与可并回主稿的小节
