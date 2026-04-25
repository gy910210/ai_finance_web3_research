# Agentic Finance Research — 项目索引

最后更新：2026-04-24  
项目状态：🟢 活跃（v0.2 主稿完成，v0.3 待补证据）

---

## 快速阅读路径

### 如果你只想用 10 分钟把握全局
1. `onepager-agentic-finance-ai-web3-v0.2.md`
2. `executive-summary-agentic-finance-v0.2.md`
3. `agentic-finance-research-v0.2.md` 的 `§1`、`§6.2`、`§6.3`、`§8.3`
4. `report_ai_web3_directions_v0.1.md`
5. 如需交易专项，再看 `ai-trader-deep-dive.md`

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

---

## 主稿 & 专题稿

| 文件 | 版本 | 角色 | 状态 |
|------|------|------|------|
| [onepager-agentic-finance-ai-web3-v0.2.md](onepager-agentic-finance-ai-web3-v0.2.md) | v0.2 | 一页版分享摘要·Agentic Finance × AI Web3 One-pager | ✅ 完成 |
| [executive-summary-agentic-finance-v0.2.md](executive-summary-agentic-finance-v0.2.md) | v0.2 | 对外分享摘要·Agentic Finance × AI Web3 Executive Summary | ✅ 完成 |
| [agentic-finance-research-v0.2.md](agentic-finance-research-v0.2.md) | v0.2 | 主稿·增量主稿（并回 workflow / assurance / execution layer） | ✅ 完成 |
| [agentic-finance-research-v0.1.md](agentic-finance-research-v0.1.md) | v0.1.1 | 旧版主稿·增量探索稿（含 GitHub 热门项目 §10） | ✅ 保留 |
| [ai-trader-deep-dive.md](ai-trader-deep-dive.md) | v1.0 | 专题稿·AI-Trader 深度调研 | ✅ 完成 |
| [report_ai_web3_directions_v0.1.md](report_ai_web3_directions_v0.1.md) | v0.1 | 专题稿·AI Web3 方向图谱 | ✅ 完成 |

---

## 中间产物（.meta/）

| 文件 | 角色 | 状态 | 下次更新建议 |
|------|------|------|-------------|
| [.meta/context_brief.md](.meta/context_brief.md) | 研究边界定义·种子术语·开放问题 | ✅ v0.1 | v0.2 前更新未解问题清单 |
| [.meta/evidence_map.md](.meta/evidence_map.md) | 文献证据地图（28篇，6方向） | ✅ v0.1 | 补充 FinCon/AlphaAgents/TradeTrap 精读后更新 |
| [.meta/paper_notes.md](.meta/paper_notes.md) | 核心论文精读（TradingAgents/FinAgent/Survey） | ✅ v0.1 | v0.2 补充 FinCon、AlphaAgents、TradeTrap |
| [.meta/evidence_audit.md](.meta/evidence_audit.md) | 批判性审查·改写建议·方法论缺陷 | ✅ v0.1 | 随精读扩展同步更新 |

---

## 版本链

```
v0.1 — 2026-04-17
  全新项目启动，零现有材料
  覆盖论文：28篇（精读3篇）
  主要方向：Agentic金融研究系统 + 交易Agent + Benchmark + 风险治理 + 产业信号
  核心来源：KDD 2024 / NeurIPS 2024 / EMNLP 2025 / ACM ICAIF 2025 / arXiv 2024-2026

v0.2 — 2026-04-24
  并回 workflow / assurance / execution layer
  新增主线：grounded workflow、semi-autonomous deployment、AI Web3 执行基础设施
  新增工件：AI Web3 专题稿 + 新版主稿

```

---

## v0.3 待补充项（优先级排序）

| 优先级 | 任务 | 涉及文件 |
|--------|------|----------|
| 🔴 P1 | 精读 FinCon (2407.06567) NeurIPS 正式版，补充性能数据与消融细节 | paper_notes / 主稿 §3.1 |
| 🔴 P1 | 精读 TradeTrap (2512.02261)，补充攻击实验完整数值 | paper_notes / 主稿 §5 |
| 🟠 P2 | 精读 AlphaAgents (2508.11152)，补充辩论机制与风险偏好建模细节 | paper_notes / 主稿 §3.3 |
| 🟠 P2 | 检索 MarketSenseAI 2.0 一手 arXiv 来源，替换二次引用 | evidence_map |
| 🟠 P2 | 补充 FinMem 直接文献来源（目前为二次引用） | evidence_map |
| 🟡 P3 | 检索 A股/中文市场专项 Agent 研究 | evidence_map / 主稿 §8 |
| 🟡 P3 | 补充 QuantAgent / AlphaGPT 的 Alpha Miner 路线细节 | 主稿 §3.1 |
| 🟡 P3 | 全文精读 AI Agents in Financial Markets (arXiv 2603.13942) | paper_notes / 主稿 §5 |
| 🟡 P3 | 关注 FinBen 在 COLING 2025 共享任务的最新结果 | 主稿 §4 |

---

## 一致性检查记录

| 检查项 | 状态 | 备注 |
|--------|------|------|
| 断链扫描 | ✅ 通过 | 所有 arXiv 链接格式一致 |
| 版本口径 | ✅ 一致 | 全稿统一 v0.1 标注 |
| 证据等级标注 | ✅ 一致 | 主稿内 `[直接]`/`[邻近]`/`[综合判断]`/`[待验证]` 标注完整 |
| Benchmark 元数据 | ⚠️ 部分缺失 | FinAgentBench / FinMaster 的 release 状态标注为 `[待确认]` |
| MarketSenseAI 2.0 来源 | ⚠️ 待补 | 目前为二次引用，无直接 arXiv 链接 |
| FinMem 来源 | ⚠️ 待补 | 目前为二次引用 |
