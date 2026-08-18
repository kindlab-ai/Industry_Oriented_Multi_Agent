# Industry-Oriented Multi-Agent: the paper collection

Screened candidate pool for the survey **Self-Evolving Context Engineering for LLM-Based Multi-Agent Systems**.

This repository is not a reading list. It is the *released set of papers* that the survey's empirical section is a census of. The survey does not claim a reproducible database query -- no Boolean string regenerates this pool -- so it publishes the pool instead, and every proportion reported in the paper is a proportion over the papers indexed here, not an estimate of a rate over all published multi-agent work.

## The numbers, and where to check them

| | count |
|---|---|
| PDF paths in the library across the nine folders | 137 |
| Distinct documents, after removing byte-identical duplicates by content hash | **125** |
| Retained for the audit (proposes or evaluates an LLM-based multi-agent system **and** reports a quantitative main result) | **38** |
| Not retained, each with a recorded reason | **87** |

12 papers are cross-filed under two topical folders with identical bytes, which is why the two counts differ. This repository stores each document once, under the folder the audit refers to it by; the *also filed under* column of `index/papers.csv` records the other location. The distinction matters when reading proportions: a rate over 125 documents is not a rate over 137 filings.

The per-system coding behind the audit is released with the paper's supplement as `e1_audit.csv` (38 rows), `e2_audit.csv` (760 cells) and `excluded.csv` (the exclusion ledger). `index/papers.csv` in this repository is the same index as the tables below, machine-readable.

## Folders

| Folder | Topic | Papers | Retained |
|---|---|---:|---:|
| `Papers/01_overview_surveys/` | Overview surveys | 7 | 0 |
| `Papers/02_multi_agent_frameworks/` | Multi-agent frameworks | 14 | 11 |
| `Papers/03_self_evolution/` | Self-evolution | 18 | 10 |
| `Papers/04_context_engineering_icl_memory/` | Context engineering, ICL, and memory | 20 | 0 |
| `Papers/05_industry_applications/` | Industry applications | 15 | 10 |
| `Papers/06_evaluation_benchmarks_safety/` | Evaluation, benchmarks, and safety | 20 | 5 |
| `Papers/07_frontier_2025_2026/` | Frontier 2025–2026 | 1 | 0 |
| `Papers/08_demo_selection_icl_sota/` | Demonstration selection | 18 | 2 |
| `Papers/09_coverage_budget_conformal/` | Coverage and budget methods | 12 | 0 |

Folders 08 and 09 were assembled for a separate line of work on demonstration selection and were screened by the same criterion as the rest; two of their papers (ConsensAgent, M2CL) are multi-agent systems and were retained. They are part of the pool and are published here for that reason.

## The audit corpus (38 retained systems)

These are the systems every quantitative claim in the survey's empirical section is computed over. Γ is the resource-equivalent collaboration gain; `cost` is what the paper reports about its own token or call cost.

| System | Paper | Venue / year | Mechanism | Γ | Cost |
|---|---|---|---|---|---|
| 360°REA | [360°REA: Towards A Reusable Experience Accumulation with 360° Assessment for Multi-Agent System](https://aclanthology.org/2024.findings-acl.778/) | Findings-ACL 2024 | evolution | no | N |
| ACE | [Agentic Context Engineering: Evolving Contexts for Self-Improving Language Models](https://openreview.net/forum?id=eC4ygDs02R) | ICLR 2026 | evolution | no | full |
| AgentDropout | [AgentDropout: Dynamic Agent Elimination for Token-Efficient and High-Performance LLM-Based Multi-Agent Collaboration](https://aclanthology.org/2025.acl-long.1170/) | ACL 2025 | topology | yes | full |
| Agents Under Siege | [Agents Under Siege: Breaking Pragmatic Multi-Agent LLM Systems with Optimized Prompt Attacks](https://aclanthology.org/2025.acl-long.476/) | ACL 2025 | other | no | N |
| AgentVerse | [AgentVerse: Facilitating Multi-Agent Collaboration and Exploring Emergent Behaviors](https://openreview.net/forum?id=EHg5GDnyq1) | ICLR 2024 | role-play | no | N |
| AI Hospital | [AI Hospital: Benchmarking Large Language Models in a Multi-agent Medical Interaction Simulator](https://aclanthology.org/2025.coling-main.680/) | COLING 2025 | role-play | no | N |
| AutoGen | [AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversations](https://openreview.net/forum?id=BAakY1hNKS) | COLM 2024 | workflow | no | N |
| Benchmark Self-Evolving | [Benchmark Self-Evolving: A Multi-Agent Framework for Dynamic LLM Evaluation](https://aclanthology.org/2025.coling-main.223/) | COLING 2025 | evolution | no | N |
| Beyond Frameworks | [Beyond Frameworks: Unpacking Collaboration Strategies in Multi-Agent Systems](https://aclanthology.org/2025.acl-long.1037/) | ACL 2025 | other | no | partial |
| CAMEL | [CAMEL: Communicative Agents for Mind Exploration of Large Language Model Society](https://doi.org/10.52202/075280-2264) | NeurIPS 2023 | role-play | no | N |
| ChatDev | [ChatDev: Communicative Agents for Software Development](https://aclanthology.org/2024.acl-long.810/) | ACL 2024 | workflow | no | full |
| CoMAS | [CoMAS: Co-Evolving Multi-Agent Systems via Interaction Rewards](https://openreview.net/forum?id=ihwAzktmWc) | ICLR 2026 | evolution | yes | N |
| CONSENSAGENT | ConsensAgent: Towards Efficient and Effective Consensus in Multi-Agent LLM Interactions through Sycophancy Mitigation | ACL 2025 | debate | yes | partial |
| Coscientist | [Autonomous Chemical Research with Large Language Models](https://doi.org/10.1038/s41586-023-06792-0) | Nature 2023 | workflow | no | N |
| DatawiseAgent | [DatawiseAgent: A Notebook-Centric LLM Agent Framework for Adaptive and Robust Data Science Automation](https://aclanthology.org/2025.emnlp-main.58/) | EMNLP 2025 | workflow | no | N |
| DriveAgent | [DriveAgent: Multi-Agent Structured Reasoning With LLM and Multimodal Sensor Fusion for Autonomous Driving](https://doi.org/10.1109/LRA.2025.3619807) | preprint 2025 | workflow | no | N |
| DrugAgent | [DrugAgent: Automating AI-aided Drug Discovery Programming through LLM Multi-Agent Collaboration](https://arxiv.org/abs/2411.15692) | preprint 2024 | workflow | no | N |
| Earnings-Call Agents | [From Earnings Calls to Investment Reports: Evaluating Role-based Multi-Agent LLM Systems](https://aclanthology.org/2025.finnlp-2.19/) | preprint 2025 | role-play | no | N |
| EvolveR | [EvolveR: Self-Evolving LLM Agents through an Experience-Driven Lifecycle](https://arxiv.org/abs/2510.16079) | preprint 2026 | evolution | no | N |
| Failure Attribution | [Which Agent Causes Task Failures and When? On Automated Failure Attribution of LLM Multi-Agent Systems](https://arxiv.org/pdf/2505.00212) | ICML 2025 | other | no | N |
| Generative Agents | [Generative Agents: Interactive Simulacra of Human Behavior](https://doi.org/10.1145/3586183.3606763) | UIST 2023 | role-play | no | N |
| GenPilot | [GenPilot: A Multi-Agent System for Test-Time Prompt Optimization in Image Generation](https://aclanthology.org/2025.findings-emnlp.49/) | EMNLP 2025 | evolution | no | N |
| Loosely-Structured SW | [Loosely-Structured Software: Engineering Context, Structure, and Evolution Entropy in Runtime-Rewired Multi-Agent Systems](https://arxiv.org/abs/2603.15690) | preprint 2026 | topology | no | partial |
| M2CL | [Context Learning for Multi-Agent Discussion](https://arxiv.org/abs/2602.02350) | ICLR 2026 | debate | no | N |
| MacNet | [Scaling Large Language Model-based Multi-Agent Collaboration](https://openreview.net/forum?id=K3n5jPkrU6) | ICLR 2025 | topology | no | N |
| MegaAgent | [MegaAgent: A Large-Scale Autonomous LLM-based Multi-Agent System Without Predefined SOPs](https://aclanthology.org/2025.findings-acl.259/) | Findings-ACL 2025 | hierarchy | no | partial |
| MetaGPT | [MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework](https://openreview.net/forum?id=VtmBAGCN7o) | ICLR 2024 | workflow | no | partial |
| Mixture-of-Agents | [Mixture-of-Agents Enhances Large Language Model Capabilities](https://openreview.net/forum?id=h0ZfDIrj7T) | ICLR 2025 | aggregation | yes | partial |
| MorphAgent | [MorphAgent: Empowering Agents through Self-Evolving Profiles and Decentralized Collaboration](https://arxiv.org/abs/2410.15048) | preprint 2024 | evolution | no | N |
| Multi-Agent Evolve | [Multi-Agent Evolve: LLM Self-Improve through Co-evolution](https://arxiv.org/abs/2510.23595) | ICLR 2026 (under review) | evolution | no | N |
| Multiagent Finetuning | [Multiagent Finetuning: Self Improvement with Diverse Reasoning Chains](https://openreview.net/forum?id=JtGPIZpOrz) | ICLR 2025 | evolution | no | N |
| MultiAgentESC | [MultiAgentESC: A LLM-based Multi-Agent Collaboration Framework for Emotional Support Conversation](https://aclanthology.org/2025.emnlp-main.232/) | EMNLP 2025 | debate | yes | N |
| QuantAgents | [QuantAgents: Towards Multi-agent Financial System via Simulated Trading](https://aclanthology.org/2025.findings-emnlp.945/) | preprint 2025 | role-play | no | N |
| Resilience w/ Faulty Agents | [On the Resilience of LLM-Based Multi-Agent Collaboration with Faulty Agents](https://proceedings.mlr.press/v267/huang25ay.html) | ICML 2025 | other | no | N |
| Sci. Discovery Agents | [Autonomous Agents for Scientific Discovery: Orchestrating Scientists, Language, Code, and Physics](https://arxiv.org/abs/2510.09901) | preprint 2025 | workflow | no | N |
| SiriuS | [SiriuS: Self-improving Multi-agent Systems via Bootstrapped Reasoning](https://openreview.net/forum?id=IDSTtDw4Cs) | ICLR 2025 WS | evolution | no | N |
| TriageAgent | [TriageAgent: Towards Better Multi-Agents Collaborations for Large Language Model-Based Clinical Triage](https://aclanthology.org/2024.findings-emnlp.329/) | Findings-EMNLP 2024 | debate | yes | full |
| When Allies Turn Foes | [When Allies Turn Foes: Exploring Group Characteristics of LLM-Based Multi-Agent Collaborative Systems Under Adversarial Attacks](https://aclanthology.org/2025.findings-emnlp.333/) | preprint 2025 | other | no | N |

## The full pool

`retained` marks the 38 systems above. Every other row carries the reason it was screened out; those reasons are the exclusion ledger of the paper's appendix, reproduced here per paper rather than in bulk. *Cited* records whether the survey cites the work somewhere in its body -- being outside the audit corpus is a statement about what can be counted, not about relevance, and many excluded papers are cited.

### `01_overview_surveys` --- Overview surveys

| # | Paper | Venue / year | Status | Cited |
|---:|---|---|---|:-:|
| 1 | [A Comprehensive Survey of Self-Evolving AI Agents: A New Paradigm Bridging Foundation Models and Lifelong Agentic Systems](https://arxiv.org/abs/2508.07407) | arXiv preprint 2025 | not retained --- survey | ✓ |
| 2 | [A Survey of Context Engineering for Large Language Models](https://arxiv.org/abs/2507.13334) | arXiv preprint 2025 | not retained --- survey | ✓ |
| 3 | [A Survey of Self-Evolving Agents: What, When, How, and Where to Evolve on the Path to Artificial Super Intelligence](https://openreview.net/forum?id=CTr3bovS5F) | Trans. Mach. Learn. Res. 2026 | not retained --- survey | ✓ |
| 4 | [A Survey on In-context Learning](https://aclanthology.org/2024.emnlp-main.64/) | Proc. Conf. Empirical Methods Natural Lang. Process. 2024 | not retained --- survey | ✓ |
| 5 | [Creativity in LLM-based Multi-Agent Systems: A Survey](https://aclanthology.org/2025.emnlp-main.1403/) | Proc. Conf. Empirical Methods Natural Lang. Process. 2025 | not retained --- survey | ✓ |
| 6 | [Large Language Model Based Multi-Agents: A Survey of Progress and Challenges](https://www.ijcai.org/proceedings/2024/890) | Proc. 33rd Int. Joint Conf. Artif. Intell. 2024 | not retained --- survey | ✓ |
| 7 | [Multi-Agent Autonomous Driving Systems with Large Language Models: A Survey of Recent Advances, Resources, and Future Directions](https://aclanthology.org/2025.findings-emnlp.683/) | Findings Assoc. Comput. Linguistics: EMNLP 2025 | not retained --- survey | ✓ |

### `02_multi_agent_frameworks` --- Multi-agent frameworks

| # | Paper | Venue / year | Status | Cited |
|---:|---|---|---|:-:|
| 1 | [AgentDropout: Dynamic Agent Elimination for Token-Efficient and High-Performance LLM-Based Multi-Agent Collaboration](https://aclanthology.org/2025.acl-long.1170/) | ACL 2025 | **retained** | ✓ |
| 2 | [AgentVerse: Facilitating Multi-Agent Collaboration and Exploring Emergent Behaviors](https://openreview.net/forum?id=EHg5GDnyq1) | ICLR 2024 | **retained** | ✓ |
| 3 | [AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversations](https://openreview.net/forum?id=BAakY1hNKS) | COLM 2024 | **retained** | ✓ |
| 4 | [Beyond Frameworks: Unpacking Collaboration Strategies in Multi-Agent Systems](https://aclanthology.org/2025.acl-long.1037/) | ACL 2025 | **retained** | ✓ |
| 5 | [CAMEL: Communicative Agents for Mind Exploration of Large Language Model Society](https://doi.org/10.52202/075280-2264) | NeurIPS 2023 | **retained** | ✓ |
| 6 | [ChatDev: Communicative Agents for Software Development](https://aclanthology.org/2024.acl-long.810/) | ACL 2024 | **retained** | ✓ |
| 7 | [Loosely-Structured Software: Engineering Context, Structure, and Evolution Entropy in Runtime-Rewired Multi-Agent Systems](https://arxiv.org/abs/2603.15690) | preprint 2026 | **retained** | ✓ |
| 8 | [MAgIC: Investigation of Large Language Model Powered Multi-Agent in Cognition, Adaptability, Rationality and Collaboration](https://aclanthology.org/2024.emnlp-main.416/) | Proc. Conf. Empirical Methods Natural Lang. Process. 2024 | not retained --- benchmark of MAS, proposes no MAS method | ✓ |
| 9 | [MegaAgent: A Large-Scale Autonomous LLM-based Multi-Agent System Without Predefined SOPs](https://aclanthology.org/2025.findings-acl.259/) | Findings-ACL 2025 | **retained** | ✓ |
| 10 | [MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework](https://openreview.net/forum?id=VtmBAGCN7o) | ICLR 2024 | **retained** | ✓ |
| 11 | [Mixture-of-Agents Enhances Large Language Model Capabilities](https://openreview.net/forum?id=h0ZfDIrj7T) | ICLR 2025 | **retained** | ✓ |
| 12 | [MultiAgentBench: Evaluating the Collaboration and Competition of LLM agents](https://aclanthology.org/2025.acl-long.421/) | Proc. 63rd Annu. Meeting Assoc. Comput. Linguistics 2025 | not retained --- benchmark | ✓ |
| 13 | [Scaling Large Language Model-based Multi-Agent Collaboration](https://openreview.net/forum?id=K3n5jPkrU6) | ICLR 2025 | **retained** | ✓ |
| 14 | [Towards a Science of Collective AI: LLM-based Multi-Agent Systems Need a Transition from Blind Trial-and-Error to Rigorous Science](https://arxiv.org/abs/2602.05289) | arXiv preprint 2026 | not retained --- position paper |  |

### `03_self_evolution` --- Self-evolution

| # | Paper | Venue / year | Status | Cited |
|---:|---|---|---|:-:|
| 1 | [360°REA: Towards A Reusable Experience Accumulation with 360° Assessment for Multi-Agent System](https://aclanthology.org/2024.findings-acl.778/) | Findings-ACL 2024 | **retained** | ✓ |
| 2 | [Agentic Context Engineering: Evolving Contexts for Self-Improving Language Models](https://openreview.net/forum?id=eC4ygDs02R) | ICLR 2026 | **retained** | ✓ |
| 3 | [CoMAS: Co-Evolving Multi-Agent Systems via Interaction Rewards](https://openreview.net/forum?id=ihwAzktmWc) | ICLR 2026 | **retained** | ✓ |
| 4 | [EvoPrompt: Connecting LLMs with Evolutionary Algorithms Yields Powerful Prompt Optimizers](https://openreview.net/forum?id=zg3PuXyH2X) † | Proc. Int. Conf. Learn. Represent. 2024 | not retained --- single agent | ✓ |
| 5 | [EvoPrompting: Language Models for Code-Level Neural Architecture Search](https://arxiv.org/abs/2302.14838) | NeurIPS 2023 | not retained --- single agent (NAS) |  |
| 6 | [EvolveR: Self-Evolving LLM Agents through an Experience-Driven Lifecycle](https://arxiv.org/abs/2510.16079) | preprint 2026 | **retained** | ✓ |
| 7 | [GenPilot: A Multi-Agent System for Test-Time Prompt Optimization in Image Generation](https://aclanthology.org/2025.findings-emnlp.49/) | EMNLP 2025 | **retained** | ✓ |
| 8 | [Generative Agents: Interactive Simulacra of Human Behavior](https://doi.org/10.1145/3586183.3606763) | UIST 2023 | **retained** | ✓ |
| 9 | [Gödel Agent: A Self-Referential Agent Framework for Recursively Self-Improvement](https://aclanthology.org/2025.acl-long.1354/) | Proc. 63rd Annu. Meeting Assoc. Comput. Linguistics 2025 | not retained --- single agent | ✓ |
| 10 | [MorphAgent: Empowering Agents through Self-Evolving Profiles and Decentralized Collaboration](https://arxiv.org/abs/2410.15048) | preprint 2024 | **retained** | ✓ |
| 11 | [Multi-Agent Evolve: LLM Self-Improve through Co-evolution](https://arxiv.org/abs/2510.23595) | ICLR 2026 (under review) | **retained** | ✓ |
| 12 | [Multiagent Finetuning: Self Improvement with Diverse Reasoning Chains](https://openreview.net/forum?id=JtGPIZpOrz) | ICLR 2025 | **retained** | ✓ |
| 13 | [PromptAgent: Strategic Planning with Large Language Models Enables Expert-Level Prompt Optimization](https://openreview.net/forum?id=22pyNMuIoa) | Proc. Int. Conf. Learn. Represent. 2024 | not retained --- single agent | ✓ |
| 14 | [Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/abs/2303.11366) | Proc. Adv. Neural Inf. Process. Syst. 2023 | not retained --- single agent | ✓ |
| 15 | [Self-Refine: Iterative Refinement with Self-Feedback](https://arxiv.org/abs/2303.17651) | Proc. Adv. Neural Inf. Process. Syst. 2023 | not retained --- single agent | ✓ |
| 16 | [SiriuS: Self-improving Multi-agent Systems via Bootstrapped Reasoning](https://openreview.net/forum?id=IDSTtDw4Cs) | ICLR 2025 WS | **retained** | ✓ |
| 17 | [Optimizing generative AI by backpropagating language model feedback](https://doi.org/10.1038/s41586-025-08661-4) | Nature 2025 | not retained --- single agent | ✓ |
| 18 | [Voyager: An Open-Ended Embodied Agent with Large Language Models](https://openreview.net/forum?id=ehfRiF0R3a) | Trans. Mach. Learn. Res. 2024 | not retained --- single agent | ✓ |

### `04_context_engineering_icl_memory` --- Context engineering, ICL, and memory

| # | Paper | Venue / year | Status | Cited |
|---:|---|---|---|:-:|
| 1 | [Compressing Context to Enhance Inference Efficiency of Large Language Models](https://aclanthology.org/2023.emnlp-main.391/) † | EMNLP 2023 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 2 | [Enabling Large Language Models to Generate Text with Citations](https://aclanthology.org/2023.emnlp-main.398/) | EMNLP 2023 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 3 | [FreshLLMs: Refreshing Large Language Models with Search Engine Augmentation](https://aclanthology.org/2024.findings-acl.813/) | Findings Assoc. Comput. Linguistics: ACL 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 4 | [LLMLingua: Compressing Prompts for Accelerated Inference of Large Language Models](https://doi.org/10.18653/v1/2023.emnlp-main.825) | Proc. Conf. Empirical Methods Natural Lang. Process. 2023 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 5 | [Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165) | Proc. Adv. Neural Inf. Process. Syst. 2020 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 6 | [LongBench: A Bilingual, Multitask Benchmark for Long Context Understanding](https://aclanthology.org/2024.acl-long.172/) | Proc. 62nd Annu. Meeting Assoc. Comput. Linguistics 2024 | not retained --- benchmark | ✓ |
| 7 | [LongLLMLingua: Accelerating and Enhancing LLMs in Long Context Scenarios via Prompt Compression](https://doi.org/10.18653/v1/2024.acl-long.91) | Proc. 62nd Annu. Meeting Assoc. Comput. Linguistics 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 8 | [LongLeader: A Comprehensive Leaderboard for Large Language Models in Long-context Scenarios](https://aclanthology.org/2025.naacl-long.439/) | Proc. Conf. Nations Americas Chapter Assoc. Comput. Linguistics: Human Lang. Technol. 2025 | not retained --- benchmark | ✓ |
| 9 | [Lost in the Middle: How Language Models Use Long Contexts](https://aclanthology.org/2024.tacl-1.9/) | Trans. Assoc. Comput. Linguistics 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 10 | [Measuring Attribution in Natural Language Generation Models](https://arxiv.org/abs/2112.12870) | Computational Linguistics 2023 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 11 | [MemBench: Towards More Comprehensive Evaluation on the Memory of LLM-based Agents](https://aclanthology.org/2025.findings-acl.989/) | Findings Assoc. Comput. Linguistics: ACL 2025 | not retained --- benchmark | ✓ |
| 12 | [MemGPT: Towards LLMs as Operating Systems](https://arxiv.org/abs/2310.08560) | arXiv preprint 2023 | not retained --- single agent | ✓ |
| 13 | [RECOMP: Improving Retrieval-Augmented LMs with Compression and Selective Augmentation](https://arxiv.org/abs/2310.04408) | ICLR 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 14 | [ReAct: Synergizing Reasoning and Acting in Language Models](https://openreview.net/forum?id=WE_vluYUL-X) | Proc. Int. Conf. Learn. Represent. 2023 | not retained --- single agent | ✓ |
| 15 | [Rethinking the Role of Demonstrations: What Makes In-Context Learning Work?](https://aclanthology.org/2022.emnlp-main.759/) | Proc. Conf. Empirical Methods Natural Lang. Process. 2022 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 16 | [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401) | Proc. Adv. Neural Inf. Process. Syst. 2020 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 17 | [The Mystery of In-Context Learning: A Comprehensive Survey on Interpretation and Analysis](https://aclanthology.org/2024.emnlp-main.795/) | Proc. Conf. Empirical Methods Natural Lang. Process. 2024 | not retained --- survey | ✓ |
| 18 | [Toolformer: Language Models Can Teach Themselves to Use Tools](https://openreview.net/forum?id=Yacmpz84TH) | Proc. Adv. Neural Inf. Process. Syst. 2023 | not retained --- single agent | ✓ |
| 19 | [Tree of Agents: Improving Long-Context Capabilities of Large Language Models through Multi-Perspective Reasoning](https://aclanthology.org/2025.findings-emnlp.246/) | Findings Assoc. Comput. Linguistics: EMNLP 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 20 | What Makes Good In-Context Examples for GPT-3? | Proc. 3rd Workshop Knowl. Extraction Integr. Deep Learn. Architectures (DeeLIO) 2022 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |

### `05_industry_applications` --- Industry applications

| # | Paper | Venue / year | Status | Cited |
|---:|---|---|---|:-:|
| 1 | [AI Hospital: Benchmarking Large Language Models in a Multi-agent Medical Interaction Simulator](https://aclanthology.org/2025.coling-main.680/) † | COLING 2025 | **retained** | ✓ |
| 2 | [AI Hospital: Benchmarking Large Language Models in a Multi-agent Medical Interaction Simulator](https://aclanthology.org/2025.coling-main.680/) | Proc. 31st Int. Conf. Comput. Linguistics 2025 | not retained --- screened, criterion not met | ✓ |
| 3 | [Autonomous Agents for Scientific Discovery: Orchestrating Scientists, Language, Code, and Physics](https://arxiv.org/abs/2510.09901) | preprint 2025 | **retained** | ✓ |
| 4 | [Autonomous Chemical Research with Large Language Models](https://doi.org/10.1038/s41586-023-06792-0) | Nature 2023 | **retained** | ✓ |
| 5 | [DatawiseAgent: A Notebook-Centric LLM Agent Framework for Adaptive and Robust Data Science Automation](https://aclanthology.org/2025.emnlp-main.58/) | EMNLP 2025 | **retained** | ✓ |
| 6 | [DriveAgent: Multi-Agent Structured Reasoning With LLM and Multimodal Sensor Fusion for Autonomous Driving](https://doi.org/10.1109/LRA.2025.3619807) | preprint 2025 | **retained** | ✓ |
| 7 | [DrugAgent: Automating AI-aided Drug Discovery Programming through LLM Multi-Agent Collaboration](https://arxiv.org/abs/2411.15692) | preprint 2024 | **retained** | ✓ |
| 8 | [From Earnings Calls to Investment Reports: Evaluating Role-based Multi-Agent LLM Systems](https://aclanthology.org/2025.finnlp-2.19/) | preprint 2025 | **retained** | ✓ |
| 9 | [Large Language Model Agents in Finance: A Survey Bridging Research, Practice, and Real-World Deployment](https://aclanthology.org/2025.findings-emnlp.972/) | Findings Assoc. Comput. Linguistics: EMNLP 2025 | not retained --- survey | ✓ |
| 10 | [Multi-Agent Autonomous Driving Systems with Large Language Models: A Survey of Recent Advances, Resources, and Future Directions](https://aclanthology.org/2025.findings-emnlp.683/) | Findings Assoc. Comput. Linguistics: EMNLP 2025 | not retained --- survey | ✓ |
| 11 | [MultiAgentESC: A LLM-based Multi-Agent Collaboration Framework for Emotional Support Conversation](https://aclanthology.org/2025.emnlp-main.232/) | EMNLP 2025 | **retained** | ✓ |
| 12 | [QuantAgents: Towards Multi-agent Financial System via Simulated Trading](https://aclanthology.org/2025.findings-emnlp.945/) | preprint 2025 | **retained** | ✓ |
| 13 | [SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering](https://openreview.net/forum?id=mXpq6ut8J3) | Proc. Adv. Neural Inf. Process. Syst. 2024 | not retained --- single agent | ✓ |
| 14 | [SWE-bench: Can Language Models Resolve Real-World GitHub Issues?](https://arxiv.org/abs/2310.06770) | arXiv preprint 2024 | not retained --- benchmark | ✓ |
| 15 | [TriageAgent: Towards Better Multi-Agents Collaborations for Large Language Model-Based Clinical Triage](https://aclanthology.org/2024.findings-emnlp.329/) | Findings-EMNLP 2024 | **retained** | ✓ |

### `06_evaluation_benchmarks_safety` --- Evaluation, benchmarks, and safety

| # | Paper | Venue / year | Status | Cited |
|---:|---|---|---|:-:|
| 1 | [ARES: An Automated Evaluation Framework for Retrieval-Augmented Generation Systems](https://aclanthology.org/2024.naacl-long.20/) | Proc. Conf. North Amer. Chapter Assoc. Comput. Linguistics: Human Lang. Technol. 2024 | not retained --- eval framework | ✓ |
| 2 | Accelerating the Machine Learning Lifecycle with MLflow † | IEEE Data Engineering Bulletin 2018 | not retained --- screened, criterion not met |  |
| 3 | [AgentBench: Evaluating LLMs as Agents](https://openreview.net/forum?id=zAdUB0aCTQ) | Proc. Int. Conf. Learn. Represent. 2024 | not retained --- benchmark | ✓ |
| 4 | [Agents Under Siege: Breaking Pragmatic Multi-Agent LLM Systems with Optimized Prompt Attacks](https://aclanthology.org/2025.acl-long.476/) | ACL 2025 | **retained** | ✓ |
| 5 | [Benchmark Self-Evolving: A Multi-Agent Framework for Dynamic LLM Evaluation](https://aclanthology.org/2025.coling-main.223/) | COLING 2025 | **retained** | ✓ |
| 6 | [FActScore: Fine-grained Atomic Evaluation of Factual Precision in Long Form Text Generation](https://aclanthology.org/2023.emnlp-main.741/) | Proc. Conf. Empirical Methods Natural Lang. Process. 2023 | not retained --- eval metric | ✓ |
| 7 | [GAIA: A Benchmark for General AI Assistants](https://arxiv.org/abs/2311.12983) | Proc. Int. Conf. Learn. Represent. 2024 | not retained --- benchmark | ✓ |
| 8 | [IPIGuard: A Novel Tool Dependency Graph-Based Defense Against Indirect Prompt Injection in LLM Agents](https://aclanthology.org/2025.emnlp-main.53/) | Proc. Conf. Empirical Methods Natural Lang. Process. 2025 | not retained --- defense, single-agent tool use | ✓ |
| 9 | [MCIP: Protecting MCP Safety via Model Contextual Integrity Protocol](https://aclanthology.org/2025.emnlp-main.62/) | Proc. Conf. Empirical Methods Natural Lang. Process. 2025 | not retained --- safety protocol, single-agent tool use | ✓ |
| 10 | [Model Context Protocol Threat Modeling and Analysis of Vulnerabilities to Prompt Injection with Tool Poisoning](https://doi.org/10.3390/jcp6030084) † | J. Cybersecur. Privacy 2026 | not retained --- threat model, no MAS results | ✓ |
| 11 | [OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments](https://proceedings.neurips.cc/paper_files/paper/2024/hash/5d413e48f84dc61244b6be550f1cd8f5-Abstract-Datasets_and_Benchmarks_Track.html) | Proc. Adv. Neural Inf. Process. Syst. 2024 | not retained --- benchmark | ✓ |
| 12 | [OWASP Top 10 for Large Language Model Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/) | 2023 | not retained --- standards document | ✓ |
| 13 | [On the Resilience of LLM-Based Multi-Agent Collaboration with Faulty Agents](https://proceedings.mlr.press/v267/huang25ay.html) | ICML 2025 | **retained** | ✓ |
| 14 | [RAGAs: Automated Evaluation of Retrieval Augmented Generation](https://aclanthology.org/2024.eacl-demo.16/) | Proc. 18th Conf. Eur. Chapter Assoc. Comput. Linguistics: Syst. Demonstrations 2024 | not retained --- eval framework | ✓ |
| 15 | [ToolEmu: Identifying the Risks of LM Agents with an LM-Emulated Sandbox](https://arxiv.org/abs/2309.15817) | Proc. Int. Conf. Learn. Represent. 2024 | not retained --- benchmark | ✓ |
| 16 | [ToolSandbox: A Stateful, Conversational, Interactive Evaluation Benchmark for LLM Tool Use Capabilities](https://aclanthology.org/2025.findings-naacl.65/) | Findings Assoc. Comput. Linguistics: NAACL 2025 | not retained --- benchmark | ✓ |
| 17 | [WebArena: A Realistic Web Environment for Building Autonomous Agents](https://arxiv.org/abs/2307.13854) | arXiv preprint 2024 | not retained --- benchmark | ✓ |
| 18 | [When Allies Turn Foes: Exploring Group Characteristics of LLM-Based Multi-Agent Collaborative Systems Under Adversarial Attacks](https://aclanthology.org/2025.findings-emnlp.333/) | preprint 2025 | **retained** | ✓ |
| 19 | [Which Agent Causes Task Failures and When? On Automated Failure Attribution of LLM Multi-Agent Systems](https://arxiv.org/pdf/2505.00212) | ICML 2025 | **retained** | ✓ |
| 20 | [Tau-bench: A Benchmark for Tool-Agent-User Interaction in Real-World Domains](https://arxiv.org/abs/2406.12045) | arXiv preprint 2024 | not retained --- benchmark | ✓ |

### `07_frontier_2025_2026` --- Frontier 2025–2026

| # | Paper | Venue / year | Status | Cited |
|---:|---|---|---|:-:|
| 1 | [SAKI-RAG: Mitigating Context Fragmentation in Long-Document RAG via Sentence-level Attention Knowledge Integration](https://aclanthology.org/2025.emnlp-main.63/) | Proc. Conf. Empirical Methods Natural Lang. Process. 2025 | not retained --- single-agent RAG | ✓ |

### `08_demo_selection_icl_sota` --- Demonstration selection

| # | Paper | Venue / year | Status | Cited |
|---:|---|---|---|:-:|
| 1 | [Problem-Solving Logic Guided Curriculum In-Context Learning for LLMs Complex Reasoning](https://arxiv.org/abs/2502.15401) | Proc. 63rd Annu. Meeting Assoc. Comput. Linguistics 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 2 | In-Context Learning with Iterative Demonstration Selection | Findings Assoc. Comput. Linguistics: EMNLP 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 3 | [Teach Better or Show Smarter? On Instructions and Exemplars in Automatic Prompt Optimization](https://arxiv.org/abs/2406.15708) | Proc. Adv. Neural Inf. Process. Syst. 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 4 | Effective Demonstration Annotation for In-Context Learning via Language Model-Based Determinantal Point Process | Proc. Conf. Empirical Methods Natural Lang. Process. 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 5 | Reward Mixology: Crafting Hybrid Signals for Reinforcement Learning Driven In-Context Learning | Findings Assoc. Comput. Linguistics: EMNLP 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 6 | Correlation-Aware Example Selection for In-Context Learning with Nonsymmetric Determinantal Point Processes | Proc. Conf. Empirical Methods Natural Lang. Process. 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 7 | ConsensAgent: Towards Efficient and Effective Consensus in Multi-Agent LLM Interactions through Sycophancy Mitigation | ACL 2025 | **retained** |  |
| 8 | [In-Context Learning Demonstration Selection via Influence Analysis](https://arxiv.org/abs/2402.11750) | arXiv preprint 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 9 | PromptWizard: Optimizing Prompts via Task-Aware, Feedback-Driven Self-Evolution | Findings Assoc. Comput. Linguistics: ACL 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 10 | [Context Learning for Multi-Agent Discussion](https://arxiv.org/abs/2602.02350) | ICLR 2026 | **retained** |  |
| 11 | [Demonstration Selection for In-Context Learning via Reinforcement Learning](https://arxiv.org/abs/2412.03966) | Proc. 42nd Int. Conf. Mach. Learn. 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 12 | [DETAIL: Task Demonstration Attribution for Interpretable In-context Learning](https://arxiv.org/abs/2405.14899) | Proc. Adv. Neural Inf. Process. Syst. 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 13 | [Curriculum Demonstration Selection for In-Context Learning](https://arxiv.org/abs/2411.18126) | Proc. 40th ACM/SIGAPP Symp. Appl. Comput. (SAC) 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 14 | [DemoRank: Selecting Effective Demonstrations for Large Language Models in Ranking Task](https://arxiv.org/abs/2406.16332) | arXiv preprint 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 15 | [Self-Generated In-Context Examples Improve LLM Agents for Sequential Decision-Making Tasks](https://arxiv.org/abs/2505.00234) | arXiv preprint 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 16 | [Easier to Judge than to Find: Predicting In-Context Learning Success for Demonstration Selection](https://arxiv.org/abs/2605.18512) | Proc. 43rd Int. Conf. Mach. Learn. 2026 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 17 | [Rethinking Label Consistency of In-Context Learning: An Implicit Transductive Label Propagation Perspective](https://arxiv.org/abs/2512.12175) | Proc. AAAI Conf. Artif. Intell. 2026 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 18 | IclForge: Enhancing In-Context Learning with Evolutionary Algorithms under Budgeted Annotation | Proc. 34th ACM Int. Conf. Inf. Knowl. Manage. (CIKM) 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |

### `09_coverage_budget_conformal` --- Coverage and budget methods

| # | Paper | Venue / year | Status | Cited |
|---:|---|---|---|:-:|
| 1 | [From Haystack to Needle: Label Space Reduction for Zero-shot Classification](https://arxiv.org/abs/2502.08436) | arXiv 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 2 | [Efficient Text Classification with Conformal In-Context Learning](https://arxiv.org/abs/2512.05732) | arXiv preprint 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 3 | [Conformal Intent Classification and Clarification for Fast and Accurate Intent Recognition](https://arxiv.org/abs/2403.18973) | Findings of NAACL 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 4 | Many-Shot In-Context Learning | Proc. Adv. Neural Inf. Process. Syst. 2024 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 5 | [Towards Compute-Optimal Many-Shot In-Context Learning](https://arxiv.org/abs/2507.16217) | COLM 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 6 | [UCS: Estimating Unseen Coverage for Improved In-Context Learning](https://arxiv.org/abs/2604.12015) | arXiv 2026 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 7 | [Learn to Select: Exploring Label Distribution Divergence for In-Context Demonstration Selection in Text Classification](https://arxiv.org/abs/2511.10675) | arXiv 2025 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 8 | [Tail-Aware Adaptive-k: Query-Adaptive Context Selection for Retrieval-Augmented Generation](https://arxiv.org/abs/2606.11907) | arXiv 2026 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 9 | Coverage-based Example Selection for In-Context Learning | Findings Assoc. Comput. Linguistics: EMNLP 2023 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) | ✓ |
| 10 | [Know Your Limits: A Survey of Abstention in Large Language Models](https://arxiv.org/abs/2407.18418) | TACL 2025 | not retained --- survey |  |
| 11 | [ICXML: An In-Context Learning Framework for Zero-Shot Extreme Multi-Label Classification](https://arxiv.org/abs/2311.09649) | arXiv 2023 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |
| 12 | [Conformal Prediction with Large Language Models for Multi-Choice Question Answering](https://arxiv.org/abs/2305.18404) | arXiv 2023 | not retained --- single-agent ICL (folders 04/08/09 except CONSENSAGENT, M2CL) |  |

## Papers held in two versions

The pool is deduplicated by content hash, which is the rule the paper states. Two papers are present as both a preprint and a camera-ready: different bytes, different page counts, the same work. They are two documents by that rule and one paper by any other, so both copies are kept and labelled rather than one being quietly dropped.

- **Multi-Agent Autonomous Driving Systems with Large Language Models: A Survey of Recent Advances, Resources, and Future Directions**
  - `01_overview_surveys/Multi-Agent Autonomous Driving Systems with Large Language Models_ A Survey of Recent Advances, Resources, and Future Directions.pdf` --- arXiv:2502.16804v2 preprint, 18 pp.
  - `05_industry_applications/Multi-Agent Autonomous Driving Systems with Large Language Models_ A Survey of Recent Advances, Resources, and Future Directions.pdf` --- Findings of EMNLP 2025 camera-ready, pp. 12756-12773
- **AI Hospital: Benchmarking Large Language Models in a Multi-agent Medical Interaction Simulator**
  - `05_industry_applications/AI Hospital_ Benchmarking Large Language Models in a Multi-agent Medical Interaction Simulator (arXiv v4).pdf` --- arXiv:2402.09742v4 preprint, 29 pp.
  - `05_industry_applications/AI Hospital_ Benchmarking Large Language Models in a Multi-agent Medical Interaction Simulator.pdf` --- COLING 2025 camera-ready, pp. 10183-10213, 31 pp.

## † Files renamed because the name did not match the PDF

Every filename in this repository now matches the title on page 1 of the file stored under it. These are the ones that did not, and what they used to be called -- kept because a link into an old path, or an older clone, otherwise just loses the paper, and because a filename that named the wrong paper is a fact about how this collection was built rather than something to erase.

- `03_self_evolution/EvoPrompt_ Connecting LLMs with Evolutionary Algorithms Yields Powerful Prompt Optimizers.pdf`
  - was "...Yields Powerful Automatic Prompt Optimizer"
- `04_context_engineering_icl_memory/Compressing Context to Enhance Inference Efficiency of Large Language Models.pdf`
  - was "Selective Context: Efficient Inference with Content-Aware Prompt Compression", which is a different paper by the same first author
- `05_industry_applications/AI Hospital_ Benchmarking Large Language Models in a Multi-agent Medical Interaction Simulator (arXiv v4).pdf`
  - was "...in a Multi-agent Medical Scenario", an earlier title of this work; the suffix distinguishes it from the COLING camera-ready copy
- `06_evaluation_benchmarks_safety/Accelerating the Machine Learning Lifecycle with MLflow.pdf`
  - was "MLflow: A Platform for the Machine Learning Lifecycle", a different Zaharia et al. paper
- `06_evaluation_benchmarks_safety/Model Context Protocol Threat Modeling and Analyzing Vulnerabilities to Prompt Injection with Tool Poisoning.pdf`
  - was "Model Context Protocol Threat Modeling: Tool Poisoning and Client Security", a paraphrase rather than the paper's title

## `Papers/_not_in_pool/`

One file sits outside the nine folders. It was published here as *Large Language Model Agent: A Survey on Methodology, Applications and Challenges*, but the PDF stored under that name is Xi et al., *The Rise and Potential of Large Language Model Based Agents: A Survey*. The library caught the mismatch and moved the file out of the screened folders, so it is not one of the 125 pool documents and no proportion in the paper counts it. It is kept here, correctly named, because the survey does cite Xi et al.

## Provenance of this index

Generated by `scripts/gen_repo_index.py` in the paper's source tree, from `references.bib` (titles, venues and links, as verified in the paper's reference-authenticity audit), `scripts/e1e2/corpus.py` (the retained set), `e1_audit.csv` and `excluded.csv`. Where a paper has no bibliography entry, because the survey cites it nowhere, its metadata was transcribed from page 1 of the stored PDF.

**No field here comes from a filename.** An earlier version of this index did take metadata from filenames, and two of its rows described a different paper from the one stored under them.

## Limits

1. **A curated library, not a database sweep.** Papers entered it through venue browsing, citation chasing, and topical search during drafting. No query string reproduces it. Read every proportion as a census of this set.
2. **One coder.** The coding manual specifies two independent coders and a reliability statistic; one coder executed it, so no inter-rater agreement is claimed.
3. **Screen recall is below 100%.** Five false negatives were found and corrected by hand. Any undetected case of the same kind moves a computability rate up, never down, so the reported rates are lower bounds.
