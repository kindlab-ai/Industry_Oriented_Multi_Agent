摘要

交代行业任务对 agent 的需求：复杂流程、知识密集、长链路决策、高可靠性；

说明单 agent 的局限：上下文容量、错误累积、角色单一、缺乏持续改进；

提出综述视角：从 ICL/context engineering 出发，看多智能体如何实现 context construction, coordination, reflection, and evolution；

总结贡献：taxonomy、应用域梳理、benchmark/evaluation、开放问题。

1. Introduction

为什么行业任务需要多智能体

为什么只讲 agent 不够，必须讲“上下文技术”

为什么“自进化”会成为下一阶段重点

本综述的范围、定义和贡献

2. Background

2.1 LLM agents
2.2 Multi-agent collaboration
2.3 In-context learning and prompt-based adaptation
2.4 Context engineering
2.5 Self-improvement / self-evolution in agent systems


3. Problem Formulation

定义“面向行业的多智能体自进化上下文技术”：

输入：任务、知识源、历史交互、工具反馈、行业规则

中间：多 agent 上下文构建/交换/裁剪/评估/更新

输出：任务决策、可解释过程、经验积累

目标：性能、鲁棒性、成本、合规、安全

4. Taxonomy of Context in Multi-Agent Systems

4.1 Context sources
4.2 Context representations
4.3 Context operations
4.4 Context flow across agents
4.5 Context failure modes

lost in the middle

context conflict

hallucinated feedback

memory drift

context collapse

5. Multi-Agent Mechanisms for Context Construction and Coordination

5.1 Role-based collaboration（CAMEL, MetaGPT, ChatDev）
5.2 Conversation-based coordination（AutoGen）
5.3 Topology/graph-based coordination（MacNet, GoA）
5.4 Aggregation/ensemble-based collaboration（MoA）
5.5 Evaluation-oriented multi-agent frameworks（MAgIC, MultiAgentBench）

6. Self-Evolving Context Techniques


6.1 Reflection-driven evolution
6.2 Experience accumulation and memory reuse
6.3 Judge-based and reward-based evolution
6.4 Prompt/context optimization by planning or evolution
6.5 Co-evolution among multiple agents
6.6 From static prompts to evolving playbooks

重点：360°REA、SiriuS、MAE、CoMAS、PromptAgent、EvoPrompt、ACE/SCOPE。

7. Industry Applications

7.1 Software engineering
7.2 Healthcare and medical decision support
7.3 Finance and investment analysis
7.4 Autonomous driving and embodied decision-making
7.5 Scientific discovery and drug discovery

每个小节统一写法：

task definition

why single-agent is insufficient

multi-agent context design

self-evolution signal

evaluation metric

deployment constraints

8. Evaluation Protocols and Benchmarks

8.1 General multi-agent benchmarks
8.2 Long-context and memory evaluation
8.3 Domain-specific evaluation
8.4 Cost-latency-reliability tradeoff
8.5 Human evaluation and expert-in-the-loop

9. Open Challenges

可以重点写这几个：

上下文进化缺乏统一定义

经验积累容易污染，产生错误迁移

多 agent 协作的收益与成本不成比例

行业场景里缺少统一、可信、可复现 benchmark

长上下文、记忆、检索、工具反馈还没形成统一理论

安全、隐私、合规与可解释性仍是部署瓶颈

10. Future Directions



context as a first-class optimization object

self-evolving agent memory

multi-agent context marketplaces / routing

domain-specialized evaluators and judges

adaptive orchestration under budget constraints

compliant and auditable agent systems for industry

integration of long-context, retrieval, memory, and evolution