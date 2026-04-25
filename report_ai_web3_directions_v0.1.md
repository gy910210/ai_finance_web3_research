# AI Web3 方向图谱：从 Agentic Wallet 到可执行金融基础设施

版本：v0.1 专题稿
生成日期：2026-04-24
时间窗口：以 2023-2026 可核一手来源为主
证据来源：Ethereum EIP、Safe、Coinbase Developer Platform、Circle、Polymarket、Olas、Oasis，以及 AI Finance 侧的 FinanceBench、BoE/FCA、FSB、FactSet、Moody’s

> 证据等级说明  
> `[直接]` = 标准、官方文档、官方产品页或官方报告直接支持；`[邻近]` = 相邻方向的可信支持；`[综合判断]` = 跨来源归纳；`[待验证]` = 目前证据不足，不应写成成熟结论

---

## 摘要

如果把 AI Web3 简单理解成“AI + 区块链”，很容易落入两个误区：
1. 把所有带 token、带 agent、带 chatbot 的项目都算作同一方向；
2. 过度强调“自治交易”或“去中心化 AI”叙事，而忽略真正决定落地能力的执行、权限、支付与审计基础设施。

基于当前可核的一手来源，更稳妥的写法是：**AI Web3 的主线并不是泛化的 AI+链，而是让 agent 获得可控、可编排、可支付、可审计的链上执行能力。** 在这个框架下，最值得关注的不是“更会聊天的链上 bot”，而是五类能力层：
- account abstraction / smart accounts
- agent toolkit / onchain action layer
- payment / settlement infrastructure
- callable market interfaces
- trusted execution / privacy-preserving off-chain logic

如果再把它与既有 AI Finance 主稿对接，那么 AI Web3 最有价值的位置不是平行赛道，而是**AI Finance 的执行基础设施扩展层**：上游是研究与决策 agent，下游是账户、支付、交易、结算与审计。

---

## 1. 为什么 AI Web3 不该被写成泛 AI+链

从当前一手来源看，AI Web3 里真正成熟或正在成熟的部分，并不是“完全自治的链上智能体社会”，而是更具体的能力栈：

1. 如何让 agent 拥有可编程账户，而不再受传统 EOA 限制
2. 如何让 agent 在权限、额度、签名和恢复规则下执行动作
3. 如何让 agent 调用支付、转账、交换、合约交互等 onchain actions
4. 如何让这类动作与真实金融工作流连接，而不只是 demo
5. 如何让执行层具备可信运行、隐私与策略保护能力

`[综合判断]` 因此，AI Web3 更适合作为“agent execution stack”来写，而不是写成“所有 Web3 项目都在做 AI”。

---

## 2. 执行层：ERC-4337 与 ERC-7579 让 Agentic Wallet 成为可能

### 2.1 ERC-4337：账户抽象的底层标准 `[直接]`

ERC-4337 提供了当前最关键的 account abstraction 技术骨架：
- 不修改 Ethereum 共识层
- 引入 `UserOperation` 作为更高层伪交易对象
- 用户把 `UserOperation` 发到单独 mempool
- bundlers 打包后调用 `EntryPoint.handleOps`
- 账户验证逻辑由 Smart Contract Account 自定义

这带来几个直接后果：
- 用户不必再把 EOA 作为唯一主账户
- 验签逻辑可以被编程化
- 支持多签、自定义恢复、不同签名方案
- 支持 sponsored transactions
- 支持用 token 支付 gas
- 支持 bundled / atomic multi-operations

`[综合判断]` 对 AI Web3 而言，ERC-4337 的意义不只是“钱包升级”，而是把 agent 的执行主体从“私钥直接签名的账户”推进到了“可编程策略账户”。这为权限限制、风险约束、session-like capabilities 和可审计执行奠定了基础。

### 2.2 ERC-7579：模块化智能账户 `[直接]`

如果说 ERC-4337 解决的是“账户抽象”，那么 ERC-7579 解决的是“抽象账户如何模块化”。它更适合承载：
- policy 模块
- session key / session 权限
- guardian / recovery
- risk limit / spending limit
- hook / plugin 风格的安全与执行逻辑

`[综合判断]` 这让 AI agent 的执行层不只是“能签名”，而是“能被规则化和插件化管理”。从研究价值看，这比单纯讨论 agent wallet 是否存在更重要，因为真正进入金融与支付场景的关键，恰恰是这些限制条件。

### 2.3 Safe：标准已进入主流 smart account 基础设施 `[直接]`

Safe 的 ERC-4337 官方文档说明，这套能力已经不只是 EIP 层提案，而是被主流 smart account 基础设施吸收。它带来的含义是：
- account abstraction 不再只是理论设计
- 主流 smart account 生态正在与 ERC-4337 汇流
- 机构级、多签级、权限控制级钱包能力，开始与 agent execution 发生连接

`[综合判断]` 这使得“agentic wallet”可以更自然地接入现实世界中的多签、组织账户、权限分层和恢复机制，而不是停留在个人开发者实验。

---

## 3. 工具层：Coinbase AgentKit 把 Agent 执行做成 SDK

Coinbase Developer Platform 的 AgentKit 是本轮调研里最关键的产品化证据之一 `[直接]`。

欢迎页直接给出的能力包括：
- secure wallet management
- onchain actions
- transfers, swaps, smart contract deployments, and more
- support for EVM-compatible networks and Solana
- custom actions and wallet providers

这意味着：
1. AI agent 拿到钱包与链上动作，不再只是手写 glue code
2. 主流平台已经把“agent -> wallet -> action”这条链做成了开发者入口
3. 执行层已经开始从“概念”进入“工具化”

`[综合判断]` 如果 ERC-4337 代表标准层，那么 AgentKit 代表平台层。两者叠加，说明 AI Web3 正在从“能否上链”转向“如何以可复用、可扩展、可管理的方式上链”。

这也是它与 AI Finance 的一个关键交点：
- 上游：research / analysis / decision agent
- 中游：wallet / authorization / action tooling
- 下游：payment / transfer / swap / contract interaction

---

## 4. 支付与结算层：Circle Wallets 让 Machine-Native Finance 更现实

Circle Wallets / Programmable Wallets 提供的不是“投机型 agent”的叙事，而是更贴近企业与支付基础设施的路线 `[直接]`：
- 钱包即服务
- 可编程账户能力
- 资产管理与签名能力嵌入产品
- 更容易与稳定币支付、结算、托管和企业工作流连接

`[综合判断]` 这条线的重要性在于，它把 AI Web3 从“链上交易 agent”扩展到了“支付 / settlement agent”。而这恰好比高风险的自治交易更接近真实商业化：
- 更强调可靠性而不是 alpha
- 更强调策略与权限而不是自由度
- 更容易与企业级金融工作流结合

因此，在 AI Finance × AI Web3 的统一图谱里，Circle 这类基础设施更适合放在“支付 / 结算执行层”，而不是“交易智能体”层。

---

## 5. 市场接口层：Polymarket 与 Olas 代表两类不同扩展方向

### 5.1 Polymarket：可调用市场接口 `[直接]`

Polymarket 的官方文档表明，它是一个可程序化接入的市场接口。它在本图谱中的价值主要有两点：
1. 它为 agent 提供了结构化、可调用的链上市场环境
2. 它比一般叙事型 DeFi demo 更适合做在线评估、策略实验和行为观察

`[综合判断]` 因此，Polymarket 更适合作为“agent 可调用的金融市场接口”案例，而不是账户基础设施本身。它处于统一框架中的“市场与执行目标”层。

### 5.2 Olas：从单个 agent 扩展到 autonomous services / agent economy `[直接]`

Olas 文档强调的是 autonomous services / agents 的网络化与协同化。它所代表的不是单个钱包或单个执行动作，而是：
- agent 作为服务单元
- 多 agent / 多服务编排
- 通过网络与激励机制组织自治服务

`[综合判断]` 在你的项目语境里，Olas 适合作为“从单个 agent wallet 走向 agent network”这条扩展路线的代表，但现阶段它更适合作为 AI Web3 专题稿的后半部分，而不是一开始的主轴。

---

## 6. 可信层：Oasis ROFL 补上 trusted execution / private logic

Oasis 的 ROFL（Runtime Off-Chain Logic）文档为 AI Web3 补上了一个经常被忽略但极重要的层：**agent 不是只需要执行，还需要可信地执行。** `[直接]`

它的价值在于：
- 把敏感逻辑放在更可信的运行环境中
- 让策略、私钥、隐私数据处理不必完全暴露在普通执行环境
- 为 AI agent 的 off-chain logic 与链上交互建立更稳固的桥梁

`[综合判断]` 这类路线在今天还不如 wallet / toolkit / payment 那么主流，但它非常可能成为后续 AI Finance × AI Web3 的关键基础设施之一。因为一旦 agent 需要：
- 处理私有研究数据
- 保管执行策略
- 使用受限密钥
- 对外证明执行可信性
那么 trusted execution / privacy-preserving logic 就不再是锦上添花，而是必要组件。

---

## 7. 与 AI Finance 的真正交叉：Research → Decision → Execution → Settlement → Audit

本轮最值得保留的综合判断是：

AI Web3 不应被当作 AI Finance 的平行主题，而更适合作为它的执行基础设施扩展层。

一个更完整的统一框架可以写成：

1. Research
- 金融文档、财报、市场信息的检索与问答
- 对应证据：FinanceBench、BloombergGPT、FactSet、Moody’s

2. Decision
- 风险分析、信用判断、工作流中的建议生成
- 对应证据：BoE/FCA、Moody’s Credit Memo、Moody’s GenAI

3. Execution
- 账户抽象、智能账户、动作编排、链上操作
- 对应证据：ERC-4337、ERC-7579、Safe、AgentKit

4. Settlement / Payment
- 钱包、转账、稳定币、支付与资金交割
- 对应证据：Circle Wallets

5. Audit / Governance
- fully autonomous 的边界、第三方依赖、治理责任、可信执行
- 对应证据：BoE/FCA、FSB、Oasis ROFL

`[综合判断]` 这个框架的好处在于，它既能解释 AI Finance 当前为何从“纯交易 agent”转向“workflow + governance”，也能解释 AI Web3 为何最有价值的不是炒作型 DeAI，而是执行与结算基础设施。

---

## 8. 支持与矛盾

### 8.1 当前支持什么
- `[直接]` account abstraction 与 smart account 基础设施已经存在，不是空谈
- `[直接]` AI agent 调钱包、做链上动作的 SDK 已存在
- `[直接]` 支付/钱包/市场接口层已有明确官方产品和文档
- `[直接]` 金融机构 AI 采用在上升，但主流场景仍偏 workflow、运营、风险与分析

### 8.2 当前不支持什么
- `[直接]` BoE/FCA 报告显示 fully autonomous 用例极少
- `[综合判断]` 因此“自治交易 agent 很快大规模进入真实金融生产环境”的叙事仍然证据偏弱
- `[综合判断]` AI Web3 当前更像“让 agent 获得执行与支付能力”，而不是“证明 agent 已经可靠地管理资金并持续跑赢市场”

### 8.3 应保留为 open question 的问题
- `[待验证]` trusted execution / provenance 是否会从辅助层升为 AI Web3 主线
- `[待验证]` tokenized asset / tokenized securities workflow 是否值得单独成章
- `[待验证]` crypto-native benchmark / replay / simulation evaluation 是否会成为下一波关键研究抓手

---

## 9. 当前最值得优先研究的 AI Web3 子方向

基于本轮证据，优先级建议如下：

### P1：最成熟、最值得先写
1. Agentic wallet / account abstraction
2. Smart account / policy-constrained execution
3. Agent toolkit / onchain action layer
4. Payment / settlement infrastructure

### P2：很重要，但更适合专题深化
5. Callable market interfaces
6. Autonomous services / agent economy
7. Trusted execution / privacy-preserving logic

### P3：保留观察，不宜过早写成成熟结论
8. 完全自治交易 agent
9. tokenized securities agentic workflow
10. crypto-native benchmark / replay / simulation evaluation

---

## 10. 对现有 AI Finance 主稿的回写建议

当前最适合并回 `agentic-finance-research-v0.1.md` 的，不是整篇 Web3 内容，而是三个新增小节：

### 可并回的 3 个小节
1. workflow / assurance 新主线
- 已并回 `agentic-finance-research-v0.2.md` §6.2
- 用 FinanceBench、BoE/FCA、FSB、FactSet、Moody’s 支撑

2. execution layer 新小节
- 已并回 `agentic-finance-research-v0.2.md` §6.3
- 用 ERC-4337、ERC-7579、Safe、AgentKit 支撑

3. research-to-execution stack
- 已并回 `agentic-finance-research-v0.2.md` §8.3
- 用 Circle、Polymarket、Oasis 补成“决策到执行到结算与审计”的统一图

### 更适合保留在本专题稿中的内容
- Olas 的 network / agent economy 叙事
- trusted execution 作为独立层的展开
- tokenized assets / benchmark / replay 这些更前瞻的路线

---

## 11. 结论

本轮最稳妥的结论不是“AI Web3 将重塑所有金融”，而是：

1. AI Web3 的核心正在从泛 AI+链叙事，收敛到一套更具体的执行基础设施栈。
2. 这套栈的中心是：账户抽象、可编程账户、agent toolkit、支付/结算、可信执行。
3. 它与 AI Finance 的最佳结合点，不是再造一个更会说话的交易 agent，而是为研究与决策 agent 提供真实、受约束、可审计的执行层。

换句话说，**AI Finance 决定 agent 知道什么、如何判断；AI Web3 决定 agent 如何在规则内行动。**

这比“AI + 区块链”这种宽泛说法，更接近当前证据真正支持的方向。

---

## 参考来源（本稿直接依赖）

- FinanceBench: https://arxiv.org/abs/2311.11944
- BloombergGPT: https://arxiv.org/abs/2303.17564
- BoE/FCA 2024 report: https://www.bankofengland.co.uk/report/2024/artificial-intelligence-in-uk-financial-services-2024
- FSB report: https://www.fsb.org/wp-content/uploads/P011117.pdf
- FactSet AI: https://www.factset.com/lp/fluent-in-finance-ai
- Moody’s GenAI: https://www.moodys.com/web/en/us/capabilities/gen-ai.html
- Moody’s Credit Memo: https://www.moodys.com/web/en/us/capabilities/gen-ai/agentic-solutions/credit-memo.html
- ERC-4337: https://eips.ethereum.org/EIPS/eip-4337
- ERC-7579: https://eips.ethereum.org/EIPS/eip-7579
- Safe ERC-4337 overview: https://docs.safe.global/advanced/erc-4337/overview
- Coinbase AgentKit: https://docs.cdp.coinbase.com/agent-kit/welcome
- Circle Wallets: https://developers.circle.com/w3s/programmable-wallets
- Polymarket Docs: https://docs.polymarket.com/
- Olas Docs: https://docs.olas.network/
- Oasis ROFL: https://docs.oasis.io/build/rofl/
