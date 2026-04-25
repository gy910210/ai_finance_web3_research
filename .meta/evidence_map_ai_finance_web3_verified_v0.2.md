# Evidence Map — AI Finance × AI Web3（已核验版 v0.2）

生成时间：2026-04-24
说明：本版优先保留“已做 URL 可达性与标题核验”的高置信一手来源。少数条目若日期未在页面显式披露，则写为“未披露”，不做猜测。

---

## A. AI Finance：workflow / governance / assurance

| title | exact_url | publication_or_update_date | source_type | directness | stance | 核心用途 |
|------|-----------|----------------------------|-------------|------------|--------|----------|
| FinanceBench: A New Benchmark for Financial Question Answering | https://arxiv.org/abs/2311.11944 | 2023-11-20 | benchmark / arXiv paper | direct | support | 证明金融文档问答与投研助手需要专门 benchmark，而不是直接复用通用 QA |
| BloombergGPT: A Large Language Model for Finance | https://arxiv.org/abs/2303.17564 | 2023-03-30 | company-affiliated research paper | direct | support | 证明头部金融信息服务商已将金融专用 LLM 作为核心研究与工作流能力建设 |
| Artificial intelligence in UK financial services - 2024 | https://www.bankofengland.co.uk/report/2024/artificial-intelligence-in-uk-financial-services-2024 | 21 November 2024 | official report (Bank of England / FCA) | direct | support+warning | 证明金融机构 AI 采用已扩展到生产率、运营、客户支持与风控，同时监管强调治理、第三方依赖与模型风险 |
| Artificial intelligence and machine learning in financial services: Market developments and financial stability implications | https://www.fsb.org/wp-content/uploads/P011117.pdf | 1 November 2017 | official report (FSB) | direct | support+warning | 为“AI 采用与金融稳定风险并存”提供国际金融稳定监管层的一手基线 |
| FactSet AI \| Fluent in Finance \| Financial Intelligence | https://www.factset.com/lp/fluent-in-finance-ai | 2026-04-23（sitemap lastmod） | official product page | direct | support | 证明头部金融数据/分析厂商已把 AI 明确产品化并定位为金融 intelligence 能力层 |
| AI and GenAI Risk Solutions – Moody's | https://www.moodys.com/web/en/us/capabilities/gen-ai.html | 未披露 | official product page | direct | support | 直接把 GenAI 与 credit analysis、research、origination、monitoring 等金融工作流绑定 |
| Moody’s AI-powered Credit Memos | https://www.moodys.com/web/en/us/capabilities/gen-ai/agentic-solutions/credit-memo.html | 未披露 | official product page | direct | support | 直接展示 agentic / AI 工作流已进入 credit memo 生成与信用分析流程 |

### finance notes
1. FinanceBench 更适合支撑“AI Finance 的研究工作流 / grounded copilot”主线，而不是直接支撑“金融机构已大规模采用”。
2. BloombergGPT 是“金融工作流产品/能力建设”的强证据，但偏底模与研究基础设施，不等于真实业务效果已被验证。
3. BoE/FCA 报告是目前最适合接到 risk/compliance/assurance 主线的一手来源。
4. FSB 报告补上了国际金融稳定层面的风险基线；FactSet 与 Moody’s 页面则补强了“金融工作流 AI 已产品化”的厂商证据链。

---

## B. AI Web3：agentic wallet / execution / payment / market access

| title | exact_url | publication_or_update_date | source_type | directness | stance | 核心用途 |
|------|-----------|----------------------------|-------------|------------|--------|----------|
| ERC-4337: Account Abstraction Using Alt Mempool | https://eips.ethereum.org/EIPS/eip-4337 | 2021-09-29 | official standard (Ethereum EIP) | direct | support | account abstraction 的底层标准；是 agent wallet 的关键执行基础设施 |
| ERC-7579: Minimal Modular Smart Accounts | https://eips.ethereum.org/EIPS/eip-7579 | 未披露 | official standard (Ethereum EIP) | direct | support | 模块化智能账户标准；适合挂接 policy、session key、guardian、limit 等能力 |
| What is ERC-4337? - Safe Docs | https://docs.safe.global/advanced/erc-4337/overview | 未披露 | official docs | direct | support | 证明主流 smart account 基础设施已明确接入 ERC-4337 生态 |
| Welcome to AgentKit - Coinbase Developer Documentation | https://docs.cdp.coinbase.com/agent-kit/welcome | 未披露 | official developer docs | direct | support | 证明“AI agent -> 链上动作”已被主流开发平台产品化 |
| Circle Wallets - Circle Docs | https://developers.circle.com/w3s/programmable-wallets | 未披露 | official product docs | direct | support | 可编程钱包/钱包即服务；适合衔接 payment / settlement agent |
| Overview - Polymarket Documentation | https://docs.polymarket.com/ | 未披露 | official docs | direct | support | prediction market 作为 agent 可调用的链上金融市场接口 |
| Olas Docs | https://docs.olas.network/ | 未披露 | official docs | direct | support | autonomous services / agent economy 基础设施 |
| Runtime Off-Chain Logic (ROFL) \| Oasis Documentation | https://docs.oasis.io/build/rofl/ | 未披露 | official docs | direct | support | trusted execution / off-chain logic 路线，为 agent 私钥、策略与隐私计算提供更可信运行面 |

### web3 notes
1. 4337 + 7579 可以构成“账户抽象 + 模块化账户”的技术骨架，是 AI Web3 最适合与 AI Finance 主稿衔接的标准层证据。
2. Safe 页面证明这套标准并非停留在提案层，而是已经被主流 smart account 基础设施吸收。
3. AgentKit 说明“代理执行层”已从概念进入 SDK/开发平台阶段。
4. Circle Wallets 让“稳定币支付 / 结算 agent”比“投机型 agent”更接近真实商业路径。
5. Polymarket 更适合作为“在线评估 / 可调用市场接口”案例，而不是账户层基础设施。
6. Oasis ROFL 补上了 trusted execution / privacy-preserving off-chain logic 这一层。

---

## C. 当前最值得进入正式主稿的 P1 条目

### AI Finance
1. FinanceBench
2. BloombergGPT
3. BoE/FCA: Artificial intelligence in UK financial services - 2024
4. FSB: AI/ML in financial services and financial stability implications
5. FactSet AI
6. Moody’s GenAI / Credit Memo pages

### AI Web3
7. ERC-4337
8. ERC-7579
9. Safe ERC-4337 overview
10. Coinbase AgentKit
11. Circle Wallets / Programmable Wallets
12. Polymarket Docs
13. Oasis ROFL

---

## D. 本轮可形成的高置信方向判断

### 直接证据支持的判断
- AI Finance 的高价值新增方向，正在从“纯交易 agent”扩展到“grounded workflow + governance/assurance”。
- AI Web3 的高价值新增方向，核心不是泛 AI+链，而是“agent wallet / execution / payment / callable market interfaces”。
- 两个方向的交叉层，最适合写成：研究—决策—执行—支付/结算—审计 的统一框架。

### 仍需下一轮补证据的判断
- 头部金融信息厂商是否已普遍把 workflow AI 产品化到一致水平：已有 BloombergGPT、FactSet、Moody’s 证据，但仍可继续补 S&P Global
- 国际组织层面对 generative AI / agentic finance 的宏观治理口径是否已收敛（还可继续补 BIS / IMF / ECB）
- AI Web3 的 trusted execution / identity / provenance 是否足以单独升为主线（Oasis 已补，仍可继续补 Phala 等）

---

## E. open_gaps
- Finance 侧还缺：BIS / IMF / ECB / S&P Global 的精确一手条目补齐
- Web3 侧还缺：Phala 或其他 trusted execution / privacy compute 一手条目、tokenized asset / security 方向是否值得升为主线
- 交叉侧还缺：crypto-native benchmark / replay / simulation evaluation 的系统化来源
