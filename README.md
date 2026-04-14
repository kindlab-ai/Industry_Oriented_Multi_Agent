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
