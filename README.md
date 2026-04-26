# Industry_Oriented_Multi_Agent
Research and Applications of Industry-Oriented Multi-Agent Self-Evolving Context Technology



## 初筛论文列表

### A. 领域总览与奠基框架：必须先读

1. **Large Language Model based Multi-Agents: A Survey of Progress and Challenges**
    多智能体 LLM 的总综述，适合用来搭综述的“背景—分类—挑战”总框架。 
2. **Large Language Model Agent: A Survey on Methodology, Applications and Challenges**
    虽然范围比“纯多智能体”更大，但它把 agent 的构造、协作、演化和应用域都纳入了，能帮你把“上下文技术”嵌进 agent 框架。 
3. **CAMEL: Communicative Agents for “Mind” Exploration of Large Language Model Society**
    2023 年非常关键的早期工作，提出 role-playing 多 agent 协作，是后续“角色分工+对话协作”路线的重要起点。 
4. **AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversations**
    Microsoft 的代表性框架，把复杂 LLM 应用统一成多 agent 对话编排，是“工程化多智能体系统”的标志性工作。 
5. **MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework**
    将 SOP（标准流程）引入多智能体协作，特别适合你“面向行业”这个角度，因为行业场景天然依赖规范流程。 
6. **AgentVerse: Facilitating Multi-Agent Collaboration and Exploring Emergent Behaviors**
    更强调多 agent 协作与涌现行为，适合写“多智能体系统形态”这一节。 
7. **ChatDev: Communicative Agents for Software Development**（ACL 2024）
    顶会论文，而且是“行业应用=软件工程”的典型案例，适合做应用章节里的重点案例。 
8. **Mixture-of-Agents Enhances Large Language Model Capabilities**
    这篇不是传统 workflow 型 MAS，但它代表了“多 agent 聚合提升能力”的另一条路线，适合放在协作范式比较里。 

------

### B. 多智能体“自进化/自改进”方向：你题目里的核心创新轴

1. **360°REA: Towards A Reusable Experience Accumulation with 360° Assessment for Multi-Agent System**（Findings of ACL 2024）
    这篇非常贴你的题：多 agent、评估反馈、经验池、可复用经验积累，已经明显触到“自进化上下文”的雏形。 
2. **SiriuS: Self-improving Multi-agent Systems via Bootstrapped Reasoning**（NeurIPS 2025）
    重点是 experience library 和 bootstrapped reasoning，适合写“从反思到经验库”的自进化路线。 
3. **Multi-Agent Evolve (MAE): LLM Self-Improve through Multi-Agent Co-evolution**
    提出 Proposer–Solver–Judge 三角色闭环，用 RL 做共同进化，是“co-evolution”关键词的代表作。 
4. **CoMAS: Co-Evolving Multi-Agent Systems via Interaction Rewards**
    亮点是不用外部监督，而从 agent 交互中构造 intrinsic rewards，代表更强的“自主进化”取向。 
5. **EvolveR: Self-Evolving LLM Agents through an Experience Lifecycle**
    更偏 agent 自我改进闭环，适合放到“经验驱动的进化机制”小节。 
6. **MorphAgent: Empowering Agents through Self-Evolving Profiles**
    关注 agent profile/role 的动态演化，适合和 CAMEL、MetaGPT 这种静态角色设计形成对照。 
7. **Multi-Agent Collaboration via Evolving Orchestration**
    从 orchestrator 角度做动态调度，不是直接优化 agent 能力，而是优化组织方式，很适合你写“系统级自进化”。 
8. **ACC-Collab: An Actor-Critic Approach to Multi-Agent LLM Collaboration**
    用 actor-critic 学协作，说明多智能体不是只能靠 prompt 设计，也能走学习型协作优化。 

------

### C. “上下文技术”主线：从 ICL 到 context engineering，再到 context evolution

1. **Language Models are Few-Shot Learners**（NeurIPS 2020）
    ICL 的奠基论文，综述里一定要交代，因为你导师已经点名“上下文包含之前的 in-context learning 等内容”。 
2. **Rethinking the Role of Demonstrations: What Makes In-Context Learning Work?**
    这篇非常关键，解释 ICL 到底依赖什么，为你后面写“context 不是简单提示词，而是可设计的信息载荷”提供理论过渡。 
3. **A Survey on In-context Learning**（EMNLP 2024）
    ICL 的系统综述，直接作为上下文技术背景综述的主参考。 
4. **The Mystery of In-Context Learning: A Comprehensive Survey on Interpretation and Analysis**（EMNLP 2024）
    更偏机制解释与分析，适合在“理论基础”里和上一篇搭配。 
5. **A Survey of Context Engineering for Large Language Models**
    这是你题目里“上下文技术”最贴近的综述，明确把 context retrieval、generation、processing、management 整体化了。 
6. **PromptAgent: Strategic Planning with Language Models Enables Expert-level Prompt Optimization**
    把 prompt/context 优化视为规划问题，是从“人工写 prompt”走向“自动进化上下文”的重要桥梁。 
7. **EvoPrompt: Connecting LLMs with Evolutionary Algorithms Yields Powerful Prompt Optimizers**
    这是“进化”与“上下文/提示优化”最直接的连接点，建议必读。 
8. **Tree of Agents: Improving Long-Context Capabilities of LLMs through Multi-Perspective Reasoning**
    这篇很好地把“多 agent”与“long-context”连接起来，非常适合你的交叉主题。 
9. **LongLeader: A Comprehensive Leaderboard for Large Language Models in Long Context**
    做上下文综述时，不能只谈方法，还要谈评测；这篇适合放在长上下文评测部分。 
10. **MemBench: Towards More Comprehensive Evaluation on the Memory of LLM Agents**
     如果你把“上下文”扩展到 memory，这篇很值得放进评测部分。 

------

### D. 行业应用：导师特别强调要看“在哪些行业用了”

#### 1）软件工程

1. **ChatDev**（ACL 2024）
    多 agent 做需求—设计—编码—测试，是最典型的软件工程应用。 
2. **MetaGPT**
    SOP 驱动的软件工程/任务分解框架，也可以放进软件工程应用节。 

#### 2）医疗健康

1. **TriageAgent: Towards Better Multi-Agents Collaborations for Large Language Model-Based Clinical Triage**（Findings of EMNLP 2024）
    临床分诊是非常实用的行业任务，这篇既有明确场景，也有多轮协作设计。 
2. **AI Hospital: Benchmarking Large Language Models in a Multi-agent Medical Scenario**
    医疗多 agent benchmark，很适合支撑“行业应用需要专门评测框架”这个观点。 
3. **MultiAgentESC: A LLM-based Multi-Agent Collaboration Framework for Emotional Support Conversation**
    偏心理健康支持，也可以作为“医疗/健康服务”子方向案例。 

#### 3）金融

1. **Large Language Model Agents in Finance: A Survey Bridging Research, Practice, and Real-World Deployment**（Findings of EMNLP 2025）
    金融场景综述，非常适合拿来梳理“行业约束、合规性、部署需求”。 
2. **QuantAgents: Towards Multi-agent Financial System via Simulated Trading**
    这是更接近实际金融工作流的多 agent 案例。 
3. **From Earnings Calls to Investment Reports: Evaluating Role-based Multi-Agent LLM Systems**
    偏投研报告生成，能体现“行业化角色分工”的实际价值。 

#### 4）自动驾驶

1. **Multi-Agent Autonomous Driving Systems with Large Language Models: A Survey of Recent Advances, Resources, and Future Directions**（Findings of EMNLP 2025）
    自动驾驶是“多主体协同+安全约束”极强的行业，非常适合你这个题。 
2. **DriveAgent: Multi-Agent Structured Reasoning with LLM and Multimodal Sensor Fusion for Autonomous Driving**
    体现了“多 agent + 多模态感知 + 决策上下文”的结合。 

#### 5）科学发现 / 生物医药

1. **DrugAgent: Automating AI-aided Drug Discovery Programming through LLM Multi-Agent Collaboration**
    很适合作为“科研/医药工业场景”的代表。 
2. **Autonomous Agents for Scientific Discovery: Orchestrating Scientists and Robots through LLM-based Agents**
    更偏前沿科研自动化，适合放到“未来高价值行业场景”。 

------

### E. 评测与基准：EMNLP 风格综述一定要单列

1. **MAgIC: Investigation of LLM Powered Multi-Agent in Cognition, Adaptability, Rationality and Collaboration**（EMNLP 2024）
    多智能体评测的代表作之一，建议放在“评测维度与benchmark”部分。 
2. **MultiAgentBench: Evaluating the Collaboration and Competition of LLM Agents**（ACL 2025）
    强调 collaboration 和 competition 的综合评测，很适合综述里做 benchmark 表。 
3. **Benchmark Self-Evolving: A Multi-Agent Framework for Dynamic LLM Evaluation**
    这篇适合你“自进化”主题，因为它连评测集合本身都在动态演化。 
4. **Scaling Large Language Model-based Multi-Agent Collaboration**（ICLR 2025）
    讨论多 agent 数量、拓扑结构、协作扩展性，属于很关键的“系统规律”论文





## Master table

| Category                        | Paper                                                        | Venue/Year                    | Problem                                  | Method                                                       | Context Contribution                                         | Relevance                                                    | URL                                                          |
| ------------------------------- | ------------------------------------------------------------ | ----------------------------- | ---------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 综述与总览                      | Large Language Model based Multi-Agents: A Survey of Progress and Challenges | Survey / 2024                 | LLM-MAS overview                         | Systematically surveys LLM-based multi-agent systems, progress and challenges. | Provides taxonomy across agent roles, communication, cooperation, planning, and evaluation. | Backbone survey for defining MAS scope and challenges.       | https://arxiv.org/abs/2402.01680                             |
| 综述与总览                      | Large Language Model Agent: A Survey on Methodology, Applications and Challenges | Survey / 2023-2025            | LLM agent methodology                    | Surveys agent architecture, planning, memory, tool use, applications, and challenges. | Connects context, memory and tool feedback to agent operation. | Background chapter for agent components beyond multi-agent systems. | https://arxiv.org/abs/2309.07864                             |
| 综述与总览                      | A Survey of Self-Evolving Agents: On Path to Artificial Super Intelligence | arXiv / 2025                  | Self-evolving agents                     | Reviews agents that adapt through data, interaction, feedback and experience. | Formalizes what/when/how to evolve, including memory, tools, architecture and multi-agent systems. | Key 2025 survey for the self-evolution axis.                 | https://arxiv.org/abs/2507.21046                             |
| 综述与总览                      | A Comprehensive Survey of Self-Evolving AI Agents: A New Paradigm Bridging Foundation Models and Lifelong Agentic Systems | arXiv / 2025                  | Self-evolving agentic systems            | Unifies feedback loops underlying self-evolving agents.      | Frames evolution as iterative feedback, refinement and lifelong adaptation. | Useful for defining self-evolution beyond prompt tweaking.   | https://huggingface.co/papers/2508.07407                     |
| 综述与总览                      | A Survey of Context Engineering for Large Language Models    | arXiv / 2025                  | Context engineering                      | Surveys context retrieval, generation, processing and management. | Defines context as an optimizable information payload rather than a static prompt. | Core survey for the context-engineering framing.             | https://arxiv.org/abs/2507.13334                             |
| 综述与总览                      | Creativity in LLM-based Multi-Agent Systems: A Survey        | EMNLP / 2025                  | Creativity in MAS                        | Surveys creativity generation, evaluation, personas and workflow coordination in MAS. | Highlights how creative contexts and agent personas are designed and evaluated. | Good 2025 frontier example of domain-specific MAS survey.    | https://aclanthology.org/2025.emnlp-main.1403/               |
| 多智能体框架与协作机制          | CAMEL: Communicative Agents for Mind Exploration of Large Language Model Society | NeurIPS workshop/arXiv / 2023 | Role-playing communication               | Introduces role-playing communicative agents for task solving and agent society exploration. | Shows how role prompts and conversation history become shared task context. | Foundational role-based multi-agent framework.               | https://arxiv.org/abs/2303.17760                             |
| 多智能体框架与协作机制          | AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversations | arXiv / 2023                  | Multi-agent application framework        | Provides a programmable framework for multi-agent conversation and orchestration. | Treats messages, tool outputs, human feedback and histories as operational context. | Canonical engineering framework for MAS applications.        | https://arxiv.org/abs/2308.08155                             |
| 多智能体框架与协作机制          | MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework | ICLR / 2024                   | SOP-driven collaboration                 | Encodes software-company SOPs into multi-agent roles and workflows. | Turns process documents and role responsibilities into structured context. | Important for industry-oriented process-driven agents.       | https://arxiv.org/abs/2308.00352                             |
| 多智能体框架与协作机制          | AgentVerse: Facilitating Multi-Agent Collaboration and Exploring Emergent Behaviors | ICLR / 2024                   | Collaboration and emergence              | Framework for multi-agent collaboration, simulation and emergent behavior study. | Uses role, memory, environment and inter-agent messages as context channels. | Useful for taxonomy of agent societies and coordination.     | https://arxiv.org/abs/2308.10848                             |
| 多智能体框架与协作机制          | ChatDev: Communicative Agents for Software Development       | ACL / 2024                    | Software development via agents          | Models software development as multi-agent chat among CEO, CTO, programmers, testers, etc. | Transforms software requirements, design reviews and tests into evolving collaborative context. | Key industry application and MAS framework case.             | https://aclanthology.org/2024.acl-long.810/                  |
| 多智能体框架与协作机制          | Mixture-of-Agents Enhances Large Language Model Capabilities | arXiv / 2024                  | Agent/model aggregation                  | Aggregates outputs from multiple LLM agents/models to improve answer quality. | Shows context aggregation and response refinement through multiple agents. | Represents ensemble/aggregation route distinct from workflow MAS. | https://arxiv.org/abs/2406.04692                             |
| 多智能体框架与协作机制          | Scaling Large Language Model-based Multi-Agent Collaboration | ICLR / 2025                   | Scaling MAS collaboration                | Studies effects of number of agents, communication structures and collaboration scaling. | Analyzes how topology and history management affect context flow. | Important for system-level limits and scaling laws.          | https://openreview.net/                                      |
| 多智能体框架与协作机制          | Beyond Frameworks: Unpacking Collaboration Strategies in Multi-Agent LLM Systems | ACL / 2025                    | Collaboration strategies                 | Studies governance, participation control, interaction dynamics and dialogue history management. | Directly analyzes dialogue history management as a context variable. | Strong 2025 paper for mechanism-level taxonomy.              | https://aclanthology.org/2025.acl-long.1037/                 |
| 多智能体框架与协作机制          | MegaAgent: A Large-Scale Autonomous LLM-based Multi-Agent System | Findings ACL / 2025           | Large-scale autonomous MAS               | Generates agents based on task complexity with dynamic decomposition and monitoring. | Uses dynamic decomposition, communication and monitoring contexts to coordinate many agents. | New 2025 framework for scalable autonomous MAS.              | https://aclanthology.org/2025.findings-acl.259/              |
| 自进化/自改进机制               | 360°REA: Towards A Reusable Experience Accumulation with 360° Assessment for Multi-Agent System | Findings ACL / 2024           | Reusable experience accumulation         | Builds assessment and experience accumulation mechanisms for MAS. | Turns assessment results into reusable experience context.   | Highly aligned with self-evolving context in MAS.            | https://aclanthology.org/2024.findings-acl.***/              |
| 自进化/自改进机制               | SiriuS: Self-improving Multi-agent Systems via Bootstrapped Reasoning | OpenReview / 2025             | Self-improving MAS                       | Constructs an experience library of high-quality reasoning trajectories for optimization. | Experience library becomes persistent context for later agents. | Core paper for experience-driven self-evolution.             | https://openreview.net/forum?id=sLBSJr3hH5                   |
| 自进化/自改进机制               | Multi-Agent Evolve: LLM Self-Improve through Multi-Agent Co-evolution | OpenReview / 2025             | Multi-agent co-evolution                 | Uses Proposer-Solver-Judge roles and reinforcement learning for self-improvement. | Judge feedback and generated tasks form evolving training/context signals. | Core co-evolution paper for the topic.                       | https://openreview.net/forum?id=sknMpr8NWU                   |
| 自进化/自改进机制               | CoMAS: Co-Evolving Multi-Agent Systems via Interaction Rewards | arXiv/OpenReview / 2025       | Interaction-reward evolution             | Learns from intrinsic rewards derived from agent interactions rather than external labels. | Uses inter-agent interaction traces as evolution signals.    | Useful for autonomous evolution without human supervision.   | https://openreview.net/                                      |
| 自进化/自改进机制               | EvolveR: Self-Evolving LLM Agents through an Experience Lifecycle | arXiv / 2025                  | Experience lifecycle                     | Defines lifecycle for collecting, validating, storing and reusing experiences. | Explicitly models experience as evolving memory/context.     | Good for memory-to-evolution mechanism section.              | https://arxiv.org/                                           |
| 自进化/自改进机制               | MorphAgent: Empowering Agents through Self-Evolving Profiles | arXiv / 2025                  | Self-evolving profiles                   | Allows agent profiles/personas to evolve with task feedback. | Agent profile is treated as mutable context.                 | Useful contrast with static role prompts in CAMEL/MetaGPT.   | https://arxiv.org/                                           |
| 自进化/自改进机制               | Gödel Agent: A Self-Referential Agent Framework for Recursive Self-Improvement | ACL / 2025                    | Recursive self-improvement               | Explores self-referential agent improvement loops.           | Agent instructions and self-model are subject to recursive revision. | Important frontier paper for self-improvement discussion.    | https://aclanthology.org/                                    |
| 自进化/自改进机制               | Agentic Context Engineering: Evolving Contexts for Self-Improving Language Models | ICLR / 2026                   | Evolving contexts                        | Studies context adaptation through instructions, strategies and evidence rather than weight updates. | Directly treats context as the evolving object for self-improving LLMs. | Probably the closest 2026 paper to your exact title.         | https://openreview.net/forum?id=eC4ygDs02R                   |
| 自进化/自改进机制               | Multiagent Finetuning: Self Improvement with Diverse Reasoning Chains | OpenReview / 2025             | Self-improvement via debate data         | Fine-tunes generator/critic agents using diverse reasoning chains from multi-agent debate. | Debate trajectories become training/contextual supervision.  | Supports bridge between MAS and model-level self-improvement. | https://openreview.net/forum?id=JtGPIZpOrz                   |
| 上下文工程、ICL、记忆与长上下文 | Language Models are Few-Shot Learners                        | NeurIPS / 2020                | Few-shot prompting and ICL               | Introduces GPT-3 and demonstrates in-context few-shot learning. | Establishes examples/instructions in prompt as adaptation context. | Historical foundation for context technologies.              | https://proceedings.neurips.cc/paper/2020/hash/1457c0d6bfcb4967418bfb8ac142f64a-Abstract.html |
| 上下文工程、ICL、记忆与长上下文 | Rethinking the Role of Demonstrations: What Makes In-Context Learning Work? | EMNLP / 2022                  | ICL mechanism                            | Analyzes which aspects of demonstrations matter for ICL.     | Shows context labels/examples affect model behavior in non-trivial ways. | Theoretical bridge from ICL to engineered context.           | https://aclanthology.org/2022.emnlp-main.759/                |
| 上下文工程、ICL、记忆与长上下文 | A Survey on In-context Learning                              | EMNLP / 2024                  | ICL survey                               | Systematically surveys ICL definitions, methods and evaluations. | Organizes demonstration selection, ordering and formatting as context design. | Main background survey for ICL section.                      | https://aclanthology.org/2024.emnlp-main.64/                 |
| 上下文工程、ICL、记忆与长上下文 | The Mystery of In-Context Learning: A Comprehensive Survey on Interpretation and Analysis | EMNLP / 2024                  | ICL interpretation                       | Surveys mechanisms and interpretation of ICL.                | Helps explain why context can induce task behavior without weight updates. | Useful for theory subsection.                                | https://aclanthology.org/2024.emnlp-main.*/                  |
| 上下文工程、ICL、记忆与长上下文 | PromptAgent: Strategic Planning with Language Models Enables Expert-level Prompt Optimization | ICLR / 2024                   | Prompt optimization                      | Uses strategic planning to optimize prompts.                 | Turns prompt/context optimization into search/planning.      | Bridge from manual prompt engineering to self-evolving context. | https://openreview.net/forum?id=22pyNMuIoa                   |
| 上下文工程、ICL、记忆与长上下文 | EvoPrompt: Connecting LLMs with Evolutionary Algorithms Yields Powerful Prompt Optimizers | ICLR / 2024                   | Evolutionary prompt optimization         | Combines LLMs and evolutionary algorithms to optimize prompts. | Directly connects evolutionary search with context/prompt improvement. | Must-read for evolution + context optimization.              | https://openreview.net/forum?id=zg3PuXyH2X                   |
| 上下文工程、ICL、记忆与长上下文 | Tree of Agents: Improving Long-Context Capabilities of LLMs through Multi-Perspective Reasoning | arXiv / 2024-2025             | Long-context reasoning                   | Uses multiple agents/perspectives to process long contexts.  | Splits and integrates long context through agent tree reasoning. | Cross-over paper connecting MAS and long-context.            | https://arxiv.org/                                           |
| 上下文工程、ICL、记忆与长上下文 | LongLeader: A Comprehensive Leaderboard for Large Language Models in Long Context | arXiv / 2024-2025             | Long-context benchmark                   | Benchmarks LLMs on long-context capabilities.                | Provides evaluation angle for context length, robustness and retrieval. | Useful for benchmark section.                                | https://arxiv.org/                                           |
| 上下文工程、ICL、记忆与长上下文 | MemBench: Towards More Comprehensive Evaluation on the Memory of LLM Agents | arXiv / 2024-2025             | Agent memory evaluation                  | Evaluates memory of LLM agents more comprehensively.         | Frames memory as persistent context subject to retention and retrieval errors. | Useful for memory/evaluation section.                        | https://arxiv.org/                                           |
| 行业应用                        | TriageAgent: Towards Better Multi-Agents Collaborations for Large Language Model-Based Clinical Triage | Findings EMNLP / 2024         | Clinical triage                          | Applies multi-agent collaboration to clinical triage tasks.  | Role-specific medical context and discussion improve decision support. | Healthcare case for industry applications.                   | https://aclanthology.org/2024.findings-emnlp.***/            |
| 行业应用                        | AI Hospital: Benchmarking Large Language Models in a Multi-agent Medical Scenario | arXiv / 2024-2025             | Medical MAS benchmark                    | Simulates hospital-like multi-agent medical scenarios.       | Medical workflow and patient histories form structured context. | Good domain-specific benchmark example.                      | https://arxiv.org/                                           |
| 行业应用                        | MultiAgentESC: A LLM-based Multi-Agent Collaboration Framework for Emotional Support Conversation | EMNLP / 2025                  | Emotional support conversation           | Applies multi-agent collaboration to mental-health support conversations. | Uses roles and interaction history to structure supportive response generation. | 2025 healthcare/mental-health application.                   | https://aclanthology.org/2025.emnlp-main.232/                |
| 行业应用                        | Large Language Model Agents in Finance: A Survey Bridging Research, Practice, and Real-World Deployment | Findings EMNLP / 2025         | Finance agents survey                    | Surveys finance LLM agents from research and deployment perspectives. | Highlights institutional context, compliance, transparency and domain constraints. | Best 2025 finance survey for industry chapter.               | https://aclanthology.org/2025.findings-emnlp.972/            |
| 行业应用                        | QuantAgents: Towards Multi-agent Financial System via Simulated Trading | arXiv / 2024-2025             | Financial trading MAS                    | Builds multi-agent financial system for simulated trading.   | Market data, roles and trading history become evolving context. | Concrete finance application case.                           | https://arxiv.org/                                           |
| 行业应用                        | From Earnings Calls to Investment Reports: Evaluating Role-based Multi-Agent LLM Systems | arXiv / 2024-2025             | Investment report generation             | Evaluates role-based agents for turning earnings calls into investment reports. | Domain documents and role assignments provide industry-specific context. | Good for finance/report generation example.                  | https://arxiv.org/                                           |
| 行业应用                        | Multi-Agent Autonomous Driving Systems with Large Language Models: A Survey of Recent Advances, Resources, and Future Directions | Findings EMNLP / 2025         | Autonomous driving MAS survey            | Surveys LLM-based multi-agent autonomous driving systems.    | Links perception, communication, planning and human interaction contexts. | Strong 2025 industry survey for autonomous driving.          | https://aclanthology.org/2025.findings-emnlp.683/            |
| 行业应用                        | DriveAgent: Multi-Agent Structured Reasoning with LLM and Multimodal Sensor Fusion for Autonomous Driving | arXiv / 2024-2025             | Autonomous driving reasoning             | Uses multi-agent structured reasoning plus multimodal sensor fusion. | Sensor context and agent reasoning contexts are fused for driving decisions. | Concrete autonomous-driving method paper.                    | https://arxiv.org/                                           |
| 行业应用                        | DrugAgent: Automating AI-aided Drug Discovery Programming through LLM Multi-Agent Collaboration | arXiv / 2024-2025             | Drug discovery programming               | Uses LLM multi-agent collaboration for AI-aided drug discovery programming. | Scientific code, experiment feedback and domain knowledge form task context. | Scientific discovery / pharma industry example.              | https://arxiv.org/                                           |
| 行业应用                        | Autonomous Agents for Scientific Discovery: Orchestrating Scientists and Robots through LLM-based Agents | arXiv / 2024-2025             | Scientific discovery agents              | Orchestrates scientist and robot agents for autonomous discovery workflows. | Lab protocols, observations and robot feedback become evolving context. | High-value future industry/science direction.                | https://arxiv.org/                                           |
| 评测、基准与安全                | MAgIC: Investigation of LLM Powered Multi-Agent in Cognition, Adaptability, Rationality and Collaboration | EMNLP / 2024                  | MAS evaluation                           | Evaluates multi-agent systems across cognition, adaptability, rationality and collaboration. | Provides dimensions for context use and collaboration quality. | Key benchmark for evaluation chapter.                        | https://aclanthology.org/2024.emnlp-main.***/                |
| 评测、基准与安全                | MultiAgentBench: Evaluating the Collaboration and Competition of LLM Agents | ACL / 2025                    | MAS benchmark                            | Benchmarks collaboration and competition across interactive scenarios. | Evaluates coordination protocols and dialogue/context strategies. | Very important 2025 benchmark for MAS evaluation.            | https://aclanthology.org/2025.acl-long.421/                  |
| 评测、基准与安全                | Benchmark Self-Evolving: A Multi-Agent Framework for Dynamic LLM Evaluation | arXiv / 2025                  | Dynamic evaluation                       | Uses multi-agent framework to evolve benchmarks dynamically. | Treats evaluation context and test cases as evolving artifacts. | Useful for self-evolving evaluation subsection.              | https://arxiv.org/                                           |
| 评测、基准与安全                | Agents Under Siege: Breaking Pragmatic Multi-Agent LLM Systems | ACL / 2025                    | MAS security                             | Studies attacks that propagate through inter-agent communication. | Shows shared context and messages can become attack vectors. | Important safety warning for industry deployment.            | https://aclanthology.org/2025.acl-long.476/                  |
| 评测、基准与安全                | When Allies Turn Foes: Exploring Group Characteristics of LLM-Based Multi-Agent Collaborative Systems Under Adversarial Attacks | Findings EMNLP / 2025         | Adversarial MAS                          | Studies group characteristics of MAS under attacks.          | Analyzes how malicious context spreads in collaboration.     | 2025 safety paper for open challenges.                       | https://2025.emnlp.org/program/find_papers/                  |
| 评测、基准与安全                | AgentDropout: Dynamic Agent Elimination for Token-Efficient and High-Performance LLM-Based Multi-Agent Collaboration | ACL / 2025                    | Token-efficient MAS                      | Eliminates less useful agents dynamically to reduce cost.    | Optimizes context budget and communication load.             | Useful for cost/context-efficiency discussion.               | https://aclanthology.org/                                    |
| 评测、基准与安全                | On the Resilience of LLM-Based Multi-Agent Collaboration with Faulty Agents | ICML / 2025                   | Fault-tolerant MAS                       | Studies resilience of multi-agent collaboration when agents are faulty. | Faulty messages and histories affect group context quality.  | Important for reliability in industry settings.              | https://openreview.net/                                      |
| 评测、基准与安全                | Which Agent Causes Task Failures and When? On Automated Failure Attribution of LLM Multi-Agent Systems | ICML / 2025                   | Failure attribution                      | Attributes failures to specific agents or moments in MAS workflows. | Analyzes dialogue traces/context histories for debugging.    | Useful for observability and auditability in deployment.     | https://openreview.net/                                      |
| 2025/2026 前沿补充              | DatawiseAgent: A Notebook-Centric LLM Agent Framework for Adaptive and Robust Data Science Automation | EMNLP / 2025                  | Data science automation                  | Builds adaptive notebook-centric agents for data science tasks. | Notebook state, code, outputs and feedback become executable context. | Industry data-analysis application and agent context case.   | https://2025.emnlp.org/program/main_papers/                  |
| 2025/2026 前沿补充              | GenPilot: A Multi-Agent System for Test-Time Prompt Optimization in Image Generation | Findings EMNLP / 2025         | Prompt optimization for image generation | Uses multi-agent system to optimize prompts at test time.    | Directly evolves prompt/context during generation.           | Good 2025 cross-modal context-evolution paper.               | https://2025.emnlp.org/program/find_papers/                  |
| 2025/2026 前沿补充              | IPIGuard: A Novel Tool Dependency Graph-Based Defense Against Indirect Prompt Injection in LLM Agents | EMNLP / 2025                  | Prompt-injection defense                 | Uses tool dependency graph to defend LLM agents from indirect prompt injection. | Models tool outputs and dependencies as security-sensitive context. | Important for safe industry deployment of context-heavy agents. | https://2025.emnlp.org/program/main_papers/                  |
| 2025/2026 前沿补充              | MCIP: Protecting MCP Safety via Model Contextual Integrity Protocol | EMNLP / 2025                  | MCP/context safety                       | Proposes contextual integrity protocol for MCP-style agent systems. | Formalizes context boundaries and integrity constraints.     | Relevant to secure context engineering in agent systems.     | https://2025.emnlp.org/program/main_papers/                  |
| 2025/2026 前沿补充              | SAKI-RAG: Mitigating Context Fragmentation in Long-Document RAG via Sentence-level Attention Knowledge Integration | EMNLP / 2025                  | Long-document RAG                        | Mitigates context fragmentation in long-document RAG.        | Improves retrieval/integration context for long documents.   | Useful for context-processing subsection.                    | https://2025.emnlp.org/program/main_papers/                  |
