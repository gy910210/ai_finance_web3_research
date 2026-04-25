# One-pager — Agentic Finance × AI Web3

版本：v0.2 一页版分享摘要
生成日期：2026-04-24
对应摘要：`executive-summary-agentic-finance-v0.2.md`
对应主稿：`agentic-finance-research-v0.2.md`

## 一句话判断

AI Finance 正在从“自治交易 agent”转向“grounded workflow + governance + semi-autonomous deployment”；AI Web3 最有价值的角色，则是为这些 agent 提供账户、执行、支付/结算与审计基础设施。

## 为什么现在值得看

过去讨论金融 agent，容易把重点放在“能不能做交易决策”。但当前更关键的问题已经变成：
- 能否在金融文档场景下稳定给出 grounded、可引用、数值一致的结果
- 能否在真实机构流程中满足治理、责任、第三方依赖与安全要求
- 能否把研究与决策真正接到可控执行、支付和审计层

## 5 个最重要结论

1. 金融 AI 的现实主线已经从“交易 alpha”扩展到研究工作流、信用分析、风险治理与受约束自动化。
2. fully autonomous 在真实金融机构中仍极少，semi-autonomous 才是更现实的部署形态。
3. AI Web3 不该被写成泛“AI+链”，而应被理解为执行基础设施栈。
4. 这套基础设施的核心是：账户抽象、可编程钱包、agent toolkit、支付/结算、可信执行。
5. 更完整的下一代金融 agent，应被写成一个五层闭环：Research → Decision → Execution → Settlement → Audit。

## 最关键证据

### AI Finance
- FinanceBench：金融文档问答需要专门 benchmark，强模型在此场景仍不可靠
- BoE / FCA 2024：75% 机构已用 AI，但 fully autonomous 仅 2%
- FSB：AI 采用与金融稳定风险并存
- FactSet / Moody’s：workflow AI 已进入 intelligence、credit analysis、origination、monitoring、credit memo

### AI Web3
- ERC-4337：账户抽象底层标准
- ERC-7579：模块化智能账户
- Safe：主流 smart account 基础设施已接入 4337
- AgentKit：AI agent → 钱包 → 链上动作 已 SDK 化
- Circle：payment / settlement 基础设施
- Oasis ROFL：trusted execution / private logic

## 最稳妥的统一框架

1. Research
2. Decision
3. Execution
4. Settlement / Payment
5. Audit / Governance

这个框架的意义是：
- AI Finance 负责“知道什么、如何判断”
- AI Web3 负责“如何在规则内行动”

## 当前不应过度宣称的内容

- fully autonomous trading agent 已接近生产可用
- AI Web3 已证明 agent 能可靠管理真实资金并持续创造 alpha
- 单一 demo 或 benchmark 足以代表真实金融部署能力

以上三点，当前证据都不支持。

## 如果你只读 3 个文件

1. `onepager-agentic-finance-ai-web3-v0.2.md`
2. `executive-summary-agentic-finance-v0.2.md`
3. `agentic-finance-research-v0.2.md`

## 最适合对外复述的一句话

AI Finance 决定 agent 知道什么、如何判断；AI Web3 决定 agent 如何在规则内行动。下一阶段真正有价值的，不是更会说话的自治交易 agent，而是能在研究、决策、执行、结算与审计之间形成闭环的受约束金融 agent 系统。