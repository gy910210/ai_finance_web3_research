# Paper Notes — FinanceBench

source_type: benchmark / arXiv paper
title: FinanceBench: A New Benchmark for Financial Question Answering
publication_time: 2023-11-20（arXiv 提交时间）
venue_or_source: arXiv
institution_or_company: 作者页未在当前精读中统一核定机构；论文作者包含 Pranab Islam、Anand Kannappan、Douwe Kiela、Rebecca Qian、Nino Scherrer、Bertie Vidgen
url: https://arxiv.org/abs/2311.11944

## problem_statement
论文试图回答一个很具体的问题：现有 LLM 在“基于公开金融文档的开放书问答（open-book financial QA）”上到底是否可靠，尤其是在企业实际会遇到的财务披露、上市公司信息与证据引用场景中是否足够可用。

## task_type
- financial question answering
- open-book QA
- benchmark / evaluation
- grounded retrieval + answer generation

## method_or_system
FinanceBench 提出一个金融问答 benchmark：
- 10,231 个关于上市公司的问题
- 带对应答案与 evidence strings
- 问题被设计为“生态有效（ecologically valid）”且尽量清晰、可核验
- 用于评估 LLM 在真实金融文档场景中的最低可用标准

## datasets_and_benchmarks
- FinanceBench：10,231 questions
- 论文还在 150 个样本案例上测试 16 种 SOTA 模型配置
- 人工审查答案 n=2,400

## explicit_claims
1. FinanceBench 是一个面向 open-book financial QA 的新 benchmark，目标是评估 LLM 在金融问答场景中的真实可用性。
2. 数据集包含 10,231 个关于上市公司的问题，并附答案和 evidence strings。
3. 作者测试了 16 个模型配置，包括 GPT-4-Turbo、Llama2、Claude2，以及向量检索和长上下文配置。
4. 现有 LLM 在金融 QA 上存在明确局限。
5. GPT-4-Turbo 在配合检索系统时，仍有 81% 的问题回答错误或拒答。
6. 更长上下文虽然能改善表现，但作者认为这对企业环境并不现实，因为会带来更高延迟，也难以支撑更大的金融文档。
7. 所有被测模型都表现出包括 hallucination 在内的弱点，限制了企业级可用性。

## results
- benchmark 规模：10,231 questions
- 被测模型配置：16
- 人工审查规模：2,400 answers
- 代表性负向结果：GPT-4-Turbo + retrieval 仍错误回答或拒答 81% 的问题

## limitations_or_undisclosed_items
- 当前精读基于 arXiv 摘要页，未进一步抽取 PDF 中表格、错误类型分布、每个模型的详细排名。
- 本轮未核对 benchmark 的许可证、发布仓库细节、样本构成比例与问题来源分层。
- “机构采用”不是这篇论文的主题，因此不能把它当作金融行业已广泛部署 workflow AI 的直接证据。

## reusable_for_sections
- AI Finance：research workflow / grounded copilot
- AI Finance：benchmark / auditability / numerical fidelity
- 风险与限制：为什么金融问答不能只看通用 LLM 能力

## citation_clues
- arXiv abs 页标题与摘要
- 提交信息：Submitted on 20 Nov 2023
- 摘要中的关键句：
  - "FinanceBench is a first-of-its-kind test suite..."
  - "It comprises 10,231 questions..."
  - "GPT-4-Turbo used with a retrieval system incorrectly answered or refused to answer 81% of questions."

## assessment
这篇论文对你的项目非常重要，但它更适合支撑这样一个判断：
“AI Finance 的关键新增方向之一是 grounded financial QA / evidence-grounded workflow，而不是只做交易 alpha 叙事。”

它不证明金融机构已经大规模依赖这类系统；它证明的是：即使是很强的模型，在金融文档问答这个基础能力层上仍不够稳。