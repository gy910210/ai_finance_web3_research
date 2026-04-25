# Paper Notes — Artificial intelligence in UK financial services - 2024

source_type: official report
title: Artificial intelligence in UK financial services - 2024
publication_time: 21 November 2024
venue_or_source: Bank of England / Financial Conduct Authority
institution_or_company: Bank of England; FCA
url: https://www.bankofengland.co.uk/report/2024/artificial-intelligence-in-uk-financial-services-2024

## problem_statement
这份报告的核心问题不是“某个模型是否 SOTA”，而是：AI 在英国金融服务行业到底使用到什么程度、主要用在哪里、风险与治理问题是什么、生成式 AI 带来了哪些新增变化。

## task_type
- official survey / market adoption report
- governance / risk / regulation
- financial services AI adoption mapping

## method_or_system
- BoE 与 FCA 联合开展 2024 年 AI / ML survey
- 目标是延续 2019、2022 调查，持续掌握 UK financial services 中 AI 的开发、部署与使用情况
- 在 2024 版中，明确纳入了 generative AI / foundation models 相关问题
- 调查共收到 118 家机构回复

## datasets_and_benchmarks
这不是 benchmark 论文，而是监管/官方调查报告。当前可直接提取的数据点包括：
- survey responses: 118 firms
- 75% 的受访机构已使用 AI
- 另有 10% 计划在未来三年使用 AI
- foundation models 占全部 AI use cases 的 17%

## explicit_claims
1. 75% 的受访机构已经使用 AI，另有 10% 计划在未来三年使用 AI。
2. foundation models 占所有 AI use cases 的 17%，表明这类模型正在快速进入金融机构场景。
3. 三分之一的 AI use cases 属于 third-party implementations，且高于 2022 年调查结果。
4. top three 第三方提供商占 cloud / model / data providers 的 73% / 44% / 33%，说明集中度与依赖风险上升。
5. 55% 的 AI 用例具有某种程度的 automated decision-making，其中 24% 属于 semi-autonomous；fully autonomous 仅 2%。
6. 最高的当前感知收益来自 data and analytical insights、AML / fraud、cybersecurity。
7. 未来三年预计增长最大的收益来自 operational efficiency、productivity、cost base。
8. 当前最重要风险中，前五项里有四项与数据有关：privacy / protection、quality、security、bias / representativeness。
9. 未来三年预计增幅最大的风险包括 third-party dependencies、model complexity、hidden / embedded models。
10. 84% 的机构报告称其 AI framework 有 accountable person；72% 表示 executive leadership 对 AI use cases 负责。
11. 46% 的机构仅对其所使用 AI 技术具有 partial understanding，34% 报告具有 complete understanding；原因之一是第三方模型使用增加。

## results
- 118 firms responded
- 75% already using AI
- 10% planning to use AI in next three years
- foundation models = 17% of all use cases
- one third of AI use cases are third-party implementations
- 55% of AI use cases have some degree of automated decision-making
- fully autonomous decision-making only 2%
- 84% have an accountable person for AI framework
- 46% report only partial understanding of the AI technologies they use

## limitations_or_undisclosed_items
- 这是英国监管/行业调查，不能直接外推为全球金融机构整体状态。
- 报告反映的是机构自报（self-reported）情况，不等于外部审计后的真实成熟度评估。
- 该报告更适合作为“采用现状 + 风险治理”证据，而不是某类具体模型性能证据。

## reusable_for_sections
- AI Finance：risk / compliance / model governance / assurance
- AI Finance：产业采用现状
- AI Finance：human-in-the-loop / semi-autonomous vs fully autonomous 边界
- 交叉框架：为什么真实金融部署更偏向受控自动化而不是完全自治

## citation_clues
- 页面标题：Artificial intelligence in UK financial services - 2024
- 页面日期：Published on 21 November 2024
- 页面正文可直接引用的数据句：
  - "75% of firms are already using artificial intelligence (AI)..."
  - "Foundation models form 17% of all AI use cases"
  - "Only 2% of use cases have fully autonomous decision-making"
  - "84% of firms reported having an accountable person for their AI framework"

## assessment
这份报告是你当前项目里非常关键的一手治理材料。

它直接支持两个判断：
1. 金融行业对 AI 的真实落地，首先集中在运营、分析、AML/欺诈、客户支持、风险治理，而不是“完全自治交易代理”。
2. 即便采用在上升，第三方依赖、可理解性不足、模型复杂性和治理责任依然是核心约束。

因此，它非常适合把你原来的 AI Finance 主稿从“交易 agent”扩展到“workflow + assurance + governance”。