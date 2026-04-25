# AI Finance × AI Web3 Research

中文研究仓库，聚焦两条正在收敛的主线：
- AI Finance：agentic 金融研究系统、交易 agent、benchmark、workflow、governance、assurance
- AI Web3：agentic wallet、execution layer、payment / settlement、callable market interfaces、trusted execution

一句话概括：
AI Finance 决定 agent 知道什么、如何判断；AI Web3 决定 agent 如何在规则内行动。

## 这个仓库里有什么

这个仓库不是代码库，而是一个持续迭代的研究文档库，当前包含三层内容：

1. 对外分享层
- `onepager-agentic-finance-ai-web3-v0.2.md` — 一页版分享摘要
- `executive-summary-agentic-finance-v0.2.md` — 对外分享摘要

2. 主稿 / 专题稿层
- `agentic-finance-research-v0.2.md` — 当前主稿
- `report_ai_web3_directions_v0.1.md` — AI Web3 专题稿
- `ai-trader-deep-dive.md` — AI-Trader 专题稿

3. 研究工件层
- `INDEX.md` — 项目导航
- `.meta/INDEX.md` — 工件导航
- `.meta/` 下的 evidence map、paper notes、reading queue、synthesis packet

## 推荐阅读顺序

### 如果你只想用 5–10 分钟把握全局
1. `onepager-agentic-finance-ai-web3-v0.2.md`
2. `executive-summary-agentic-finance-v0.2.md`
3. `agentic-finance-research-v0.2.md` 的 `§1`、`§6.2`、`§6.3`、`§8.3`

### 如果你更关心 AI Finance 主线
1. `agentic-finance-research-v0.2.md`
2. `.meta/paper_notes_financebench.md`
3. `.meta/paper_notes_boe_fca_ai_finance_2024.md`
4. `.meta/evidence_map_ai_finance_web3_verified_v0.2.md`

### 如果你更关心 AI Web3 执行层
1. `report_ai_web3_directions_v0.1.md`
2. `.meta/paper_notes_eip4337.md`
3. `.meta/paper_notes_coinbase_agentkit.md`
4. `agentic-finance-research-v0.2.md` 的 `§6.3` 与 `§8.3`

## 当前最重要的结论

1. AI Finance 的现实主线，正在从“自治交易 agent”转向 grounded workflow、governance 与 semi-autonomous deployment。
2. AI Web3 最有价值的位置，不是泛“AI+链”叙事，而是账户、执行、支付/结算与审计基础设施。
3. 更完整的下一代金融 agent，应被理解为一个闭环：
   Research → Decision → Execution → Settlement / Payment → Audit / Governance

## 仓库结构

```text
.
├── README.md
├── INDEX.md
├── onepager-agentic-finance-ai-web3-v0.2.md
├── executive-summary-agentic-finance-v0.2.md
├── agentic-finance-research-v0.2.md
├── report_ai_web3_directions_v0.1.md
├── ai-trader-deep-dive.md
└── .meta/
    ├── INDEX.md
    ├── evidence_map_ai_finance_web3_verified_v0.2.md
    ├── paper_notes_financebench.md
    ├── paper_notes_boe_fca_ai_finance_2024.md
    ├── paper_notes_eip4337.md
    ├── paper_notes_coinbase_agentkit.md
    └── ...
```

## 如何使用这个仓库

如果你是：

- 研究者：先看主稿，再下钻 `.meta/` 中的 paper notes 和 evidence map
- 投资人 / 产品人：先看 one-pager 和 executive summary
- 想关注 AI Web3：先看专题稿，再回看主稿中 execution layer 与统一框架部分
- 想跟踪后续更新：从 `INDEX.md` 和 `.meta/INDEX.md` 开始

## 当前证据边界

这个仓库强调区分三类内容：
- 直接证据：论文、官方文档、官方产品页、官方报告直接支持
- 综合判断：跨来源归纳的研究判断
- 待验证假设：目前还不能写成成熟结论的方向

因此：
- 对外引用时，优先使用主稿、摘要、专题稿
- `.meta/` 更适合作为研究过程工件与证据台账，而不是最终成文

## 后续待补方向

- BIS / IMF / ECB / S&P Global 的一手来源
- Phala 或同类 trusted execution / privacy compute 来源
- tokenized asset / tokenized securities workflow
- crypto-native benchmark / replay / simulation evaluation

## 入口文件

- 项目总导航：`INDEX.md`
- 工件总导航：`.meta/INDEX.md`
- 当前主稿：`agentic-finance-research-v0.2.md`

## License

当前仓库尚未单独补 License 文件；如需对外长期开放，建议下一步补充。