# Paper outline

**Self-Evolving Context Engineering for LLM-Based Multi-Agent Systems: A Survey**

This replaces `Framwork.md`, which held the April 2026 planning outline: a
different title (*"...in Industry Applications"*), a ten-section structure, and
sections that no longer exist (*Context Evaluation*, *Context Failure Modes*,
*Creative Generation and Multimodal Applications*). The paper acquired an
empirical audit after that outline was written, and the audit is now what the
second half of the paper is organised around, so the old file described a
different document.

## Body

1. **Introduction**
2. **Preliminaries and Scope**
3. **Literature Search, Scope, and Selection Methodology** — the section this
   repository is the artifact for
4. **Positioning Against Related Surveys and Frameworks**
5. **Taxonomy** — context construction, multi-agent context coordination,
   context evolution
6. **Technical Review**
   - 6.1 Context Construction
   - 6.2 Multi-Agent Context Coordination
   - 6.3 Context Evolution
   - 6.4 Comparing the Mechanisms
   - 6.5 Worked Example: From a Failed Patch to a Reusable Playbook
7. **Empirical Study**
   - 7.1 Can collaboration gain be computed from what is published?
   - 7.2 Which lifecycle metrics can be computed at all?
   - 7.3 A governed artifact lifecycle, measured end to end
   - 7.4 Lifecycle-coded case studies
   - 7.5 Threats to the validity of this study
8. **Industry Applications and Domain Differences**
   - 8.1 From feedback properties to gate design
9. **Evaluation and Challenges**
   - 9.1 An evaluation protocol that follows the feedback
10. **Limitations of This Survey**
11. **Conclusion**

## Supplement

- **A** Notation and glossary
- **B** Timeline of representative milestones
- **C** Full taxonomy table
- **D** Artifact governance table
- **E** Related-work positioning table
- **F** Full benchmark table
- **G** Detailed domain analysis
- **H** Corpus, screening, and coding procedure — the screening flow, the
  retained-paper inventory, the exclusion ledger, and the limits of the
  procedure. **This repository is the pool that appendix screens.**
- **I** Operational metrics
- **J** Ablation protocol

## The organising claim

A validation gate can act only at the granularity at which feedback assigns
blame. Coarse credit signals therefore cannot be repaired by stricter approval
rules, and the gate a domain needs follows from the resolution and latency of
its feedback rather than from how consequential the domain is.

The empirical section is what puts that claim on measured ground rather than
argued ground, and it is why the composition of the pool in this repository is
load-bearing rather than decorative.
