# Synthesis Packet — AI Finance × AI Web3（第 1 轮精读后）

生成时间：2026-04-24

## target_output_type
双视角稿 / 方向比较稿 的前置 synthesis packet

## section_outline
1. 为什么 AI Finance 的重点正在从交易 alpha 叙事扩展到 grounded workflow 与 assurance
2. 为什么 AI Web3 的重点不该是泛 AI+链，而是账户抽象与执行层
3. 统一框架：研究—决策—执行—支付/结算—审计
4. AI Finance × AI Web3 的交叉机会与边界
5. 下一轮必须补齐的证据缺口

## evidence_backed_claims
1. FinanceBench 直接证明：金融文档问答与投研助手需要专门 benchmark，且强模型在该场景下仍不可靠。
2. BoE/FCA 2024 报告直接证明：金融机构的 AI 采用已较广泛，但 fully autonomous use cases 极少，治理与第三方依赖是核心约束。
3. ERC-4337 直接提供了 agent wallet / programmable account 的底层标准框架。
4. Coinbase AgentKit 直接证明：主流开发平台已开始把 AI agent -> 钱包 -> 链上动作 做成开发者工具链。

## support_vs_contradiction
### support
- AI Finance：workflow / risk / governance 是现实主线
- AI Web3：execution layer / wallet layer 已有清晰标准和 SDK 化入口
- 两者可以在“受约束执行”这一层发生强耦合

### contradiction
- FinanceBench 表明即便是强模型，在金融基础问答上仍远未可靠
- BoE/FCA 表明 fully autonomous 在真实金融场景仍非常少
- 这意味着“自治交易 agent 快速落地”的叙事证据仍弱

## new_angles
1. 把 AI Web3 作为 AI Finance 的“执行基础设施扩展”来看，而不是平行赛道
2. 把 account abstraction / modular accounts / agent toolkits 放进“金融 agent 执行层”章节
3. 用 BoE/FCA 的 semi-autonomous vs fully autonomous 分层，约束对 AI Web3 autopilot 的表述

## merge_ready_sections
- AI Finance 主稿可新增：workflow benchmark / governance assurance 小节
- 可新开 AI Web3 专题稿的首章：agentic wallet / execution layer
- 可新开交叉章节：research-to-execution stack

## keep_as_exploratory
- tokenized asset / tokenized securities agentic workflow
- trusted execution / provenance 是否升为主线
- crypto-native benchmark / replay / simulation evaluation

## route_family_summary
当前最清晰的两条路线族：
1. AI Finance：grounded workflow -> governance -> semi-autonomous deployment
2. AI Web3：account abstraction -> modular wallet -> agent toolkit -> callable market/payment actions

## catalog_sync_notes
下一轮应补以下条目后，再决定是否更新正式主稿：
- BIS / IMF / ECB
- Moody’s / FactSet / S&P Global
- Safe / Oasis / Phala

## recommendation
下一步最值得做的，不是直接改旧主稿，而是：
1. 再补 4~6 条一手来源
2. 形成一版 `report_ai_web3_directions_v0.1.md`
3. 然后决定哪些段落并回 `agentic-finance-research-v0.1.md`
