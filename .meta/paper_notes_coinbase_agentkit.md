# Paper Notes — Coinbase AgentKit

source_type: official developer documentation
title: Welcome to AgentKit - Coinbase Developer Documentation
publication_time: 页面未见明确披露
venue_or_source: Coinbase Developer Platform
institution_or_company: Coinbase
url: https://docs.cdp.coinbase.com/agent-kit/welcome

## problem_statement
AgentKit 要解决的问题是：如何让 AI agent 以较低集成门槛获得安全钱包管理与链上动作能力，从而不仅能“分析”，还能执行转账、交换、合约交互等 onchain actions。

## task_type
- official developer toolkit
- agent wallet / onchain action framework
- blockchain developer platform

## method_or_system
根据欢迎页顶部说明，AgentKit 是构建在 Coinbase Developer Platform (CDP) SDK 之上的 toolkit，用于让 AI agents 与 blockchain networks 交互。页面明确给出的能力包括：
- secure wallet management
- onchain actions
- multi-network support
- extensibility（custom actions / wallet providers）

页面可直接提取的能力表述：
1. Create and manage crypto wallets for your agents
2. Enable transfers, swaps, smart contract deployments, and more
3. Deploy on any EVM-compatible network or Solana
4. Add custom actions and wallet providers

## datasets_and_benchmarks
不适用；这是开发者文档，不是 benchmark。

## explicit_claims
1. AgentKit 是一个让 AI agents 能与 blockchain networks 交互的 toolkit。
2. 它提供 secure wallet management。
3. 它支持 onchain capabilities，包括 transfers、swaps、smart contract deployments 等。
4. 它支持 any EVM-compatible network or Solana。
5. 它允许添加 custom actions 和 wallet providers。
6. 它建立在 Coinbase Developer Platform (CDP) SDK 之上。

## results
不是实验结果，而是产品/开发平台能力边界：
- agents can have wallets
- agents can perform onchain actions
- support multiple networks
- extensible action framework

## limitations_or_undisclosed_items
- 欢迎页是概览页，不提供完整安全模型、默认权限边界、签名策略、风控策略与生产限制细节。
- 该页面证明“产品化开发入口已经存在”，但不等于默认就适合无人监管地执行真实资金操作。
- 还需要后续查看 Quickstart、wallet model、authentication、tool docs，才能判断它更适合 copilot、semi-autonomous，还是更接近 autopilot。

## reusable_for_sections
- AI Web3：agentic wallet / onchain action layer
- AI Finance × AI Web3：从研究 agent 到执行 agent 的产品化桥梁
- payment / settlement / DeFi copilot

## citation_clues
- 页面标题：Welcome to AgentKit
- 页面顶部可直接引用的介绍：
  - "AgentKit is a toolkit enabling AI agents to interact with blockchain networks with secure wallet management and comprehensive onchain capabilities."
  - "Built on the Coinbase Developer Platform (CDP) SDK..."
- 页面列出的能力：
  - Secure Wallet Management
  - Onchain Actions
  - Multi-Network Support
  - Add custom actions and wallet providers

## assessment
AgentKit 是你这轮研究里很关键的一条“产品化证据”。

如果 ERC-4337 说明了“标准层已经允许可编程账户”，那么 AgentKit 说明的是：
“主流开发平台已经开始把 AI agent -> 钱包 -> 链上动作 这条路径做成开发者工具链。”

因此它特别适合连接你原来的 AI Finance 主稿与 AI Web3 新方向：
- 上游是 research / decision agent
- 中间是 wallet / authorization / action tooling
- 下游是 payment / transfer / swap / contract interaction

这让“研究—决策—执行”不再只是概念链，而开始有明确 SDK 形态。