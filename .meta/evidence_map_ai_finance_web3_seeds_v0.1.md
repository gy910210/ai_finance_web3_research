# Evidence Map Seeds — AI Finance × AI Web3

生成时间：2026-04-24
说明：本文件是“下一轮精确核验前”的 seed evidence map。凡未逐条核精确发布日期/URL/正文表述者，统一按“待核验种子来源”处理，不直接当成熟结论使用。

---

## Cluster A — AI Finance: research workflow / grounded copilot

| title | source_type | time | directness | stance | note |
|------|-------------|------|------------|--------|------|
| FinanceBench | benchmark / paper | 2024 | direct | support | 指向“金融问答与投研助手必须 grounded / cited / numerically faithful” |
| Bloomberg AI / research workflow 官方材料 | official product | 2024-2025 | direct | support | 指向头部金融信息厂商正在把 AI 嵌入研究工作流，而非先推全自动交易 |
| FactSet / S&P Global / Moody’s 金融 AI 助手产品页 | official product | 2024-2025 | direct | support | 说明 analyst productivity / document workflow 是现实落地主线 |

## Cluster B — AI Finance: risk / compliance / assurance

| title | source_type | time | directness | stance | note |
|------|-------------|------|------------|--------|------|
| FSB AI 与金融稳定相关报告 | official report | 2024-2025 | direct | support+warning | 既支持采用上升，也强调模型同质化、第三方集中、系统性风险 |
| BIS generative AI and financial system 相关材料 | official research | 2024-2025 | direct | support+warning | 强化“治理与稳定性约束”视角 |
| BoE / FCA AI in financial services 调查材料 | official survey | 2024-2025 | direct | support | 有助判断真实使用场景分布 |
| ECB / IMF 关于银行/金融 AI 使用的研究 | official research | 2024-2025 | direct | support | 为银行与宏观监管线补充一手来源 |
| NIST AI RMF | official framework | 2023+ | adjacent | support | 非金融专属，但适合作为 AI assurance 的方法底座 |

## Cluster C — AI Finance: benchmark / evaluation / robustness

| title | source_type | time | directness | stance | note |
|------|-------------|------|------------|--------|------|
| FinBen | benchmark / paper | 2024 | direct | support | 金融 benchmark 基础盘 |
| FinanceBench | benchmark / paper | 2024 | direct | support | grounded QA / citation / numerical fidelity |
| TradeTrap | paper / evaluation | 2024-2025 | direct | contradiction | 提示交易 agent 在对抗扰动下极不稳健 |
| 通用 agent benchmark（GAIA / Tau-bench 等） | benchmark | 2023-2025 | adjacent | open-gap | 可借鉴 workflow eval 思路，但不是金融专用 |

## Cluster D — AI Web3: agentic wallet / execution layer

| title | source_type | time | directness | stance | note |
|------|-------------|------|------------|--------|------|
| EIP-4337 | standard | 2023+ | direct | support | account abstraction 是 agent wallet 的关键底座 |
| ERC-7579 | standard | 2024 | direct | support | 模块化智能账户，适合 policy / session key / guardian / limit |
| Safe Docs | official docs | ongoing | direct | support | 多签、模块、权限控制，是 agent wallet 的现实落点 |
| Coinbase AgentKit | official docs | 2024 | direct | support | 官方化的 AI agent → 链上动作接口层 |

## Cluster E — AI Web3: onchain copilot / DeFi / prediction / payment

| title | source_type | time | directness | stance | note |
|------|-------------|------|------------|--------|------|
| Polymarket Docs | official docs | ongoing | direct | support | prediction market 是 agent 在线评估的良好实验场 |
| Circle Programmable Wallets | official docs | 2024 | direct | support | 机器支付/结算层的现实底座 |
| Olas / Autonolas | official docs | ongoing | direct | support | autonomous services / agent economy |
| ElizaOS | framework docs | 2024 | direct | support | 多 agent 编排层，可做 onchain copilot orchestration |
| DEX 聚合 API（1inch/0x/Jupiter 等） | official APIs | ongoing | adjacent | support | 说明 DeFi 执行面已有较成熟 API 栈 |

## Cluster F — AI Web3: trusted execution / identity / provenance

| title | source_type | time | directness | stance | note |
|------|-------------|------|------------|--------|------|
| Phala Docs | official docs | ongoing | direct | support | TEE / confidential execution 适合 agent 私钥与推理保护 |
| Oasis ROFL | official docs | 2024 | direct | support | 将可信执行与链上应用连接 |
| Ritual Network Docs | official docs | 2024 | direct | support | AI-native chain infra 样本 |
| Bittensor Docs | official docs | ongoing | direct | support | decentralized AI network 的代表样本 |

---

## support_vs_contradiction_seeds

### support
- AI Finance：工作流 copilot、投研助手、文档证据编排、风控治理是更现实的落地主线
- AI Web3：account abstraction + modular account + agent SDK 已让“可执行 agent”具备明确底座
- 两边都越来越强调：权限、风险约束、审计留痕、在线评估

### contradiction
- 金融侧：产品化信号很强，但公开可复现实证弱；提效证据强于 alpha 证据
- Web3 侧：能调链上动作不等于有金融价值；copilot 与 autopilot 必须分开
- 交易类 agent 在两边都面临：鲁棒性、尾部风险、合规边界、责任归属问题

### open_gap
- 金融 workflow assurance 的公开 benchmark 仍不足
- crypto-native benchmark / replay / simulation 体系仍缺统一标准
- agentic wallet 的安全边界、policy engine 与可验证执行仍需系统化整理

---

## route_family_candidates

1. 证据优先的金融研究代理
2. 金融风险/合规/assurance 代理
3. agentic wallet / execution policy stack
4. onchain copilot（DeFi / prediction / payment）
5. trusted execution + identity + provenance
6. benchmark / replay / simulation evaluation
