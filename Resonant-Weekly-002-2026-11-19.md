# Resonant Weekly 002

**19 November 2026 | Community discussions from 12–18 November**

Weekly update on what's happening in the Augmentatist community. This issue looks at safeguards for increasingly autonomous agents, the value of divergent thinking, progress on ResonantDAO's contribution economy, and the practical choices involved in running AI locally. It also covers memory, agent collaboration, AI infrastructure and creative experiments.

The connecting question this week is **what happens when we give AI systems more autonomy?** The discussions do not all answer it in the same way. Some focus on giving agents room to act; others focus on context, security, hardware and human oversight.

## In this issue

1. [Who Watches the Agents?](#who-watches-the-agents)
2. [Why We Ask for Divergence](#why-we-ask-for-divergence)
3. [The ResonantDAO Contribution Economy](#the-resonantdao-contribution-economy)
4. [The AI Hardware Dilemma: Buy, Build or Wait?](#the-ai-hardware-dilemma-buy-build-or-wait)
5. [When an AI Remembers Too Much or Too Little](#when-an-ai-remembers-too-much-or-too-little)
6. [NVIDIA, Market Corrections and the Cost of AI Infrastructure](#nvidia-market-corrections-and-the-cost-of-ai-infrastructure)
7. [Agents Working Together](#agents-working-together)
8. [Experiments, Projects and Exploration](#experiments-projects-and-exploration)
9. [Recordings and short edits](#recordings-and-short-edits)
10. [Key terms](#key-terms)

---

## Who Watches the Agents?

As agents gain permission to browse, use tools, call services and handle information, it becomes more important to examine **what they are about to do**, not just whether their text looks convincing.

A discussion in `#ai-models` on 18 November explored putting a smaller guardrail model in the path of potentially risky agent actions, particularly before outbound network requests or the disclosure of data. Members considered whether cheap CPU capacity could be used for such checks rather than reserving expensive GPU resources for every task.

IBM's Granite Guardian family came up as one possible approach, alongside [NVIDIA NeMo Guardrails](https://github.com/NVIDIA-NeMo/Guardrails). The discussion also exposed a real trade-off: a lightweight guardrail may miss important threats, whereas a more capable model running on a CPU may add noticeable delay. Members questioned how quickly protection mechanisms are updated as attacks change.

No tested configuration or definitive recommendation emerged. The useful principle is to design **checks at the boundary between an agent's reasoning and its ability to act**, and to measure the cost and effectiveness of those checks in real workflows. A guardrail model should complement, not replace, limited permissions, review steps and other security controls.

**From the discussion:** [Proposed checks on outbound requests](https://discord.com/channels/1423225702135894111/1491424406595964958/1572641112751997019) · [NeMo Guardrails and the update question](https://discord.com/channels/1423225702135894111/1491424406595964958/1572642879271080008) · [Small model versus CPU latency](https://discord.com/channels/1423225702135894111/1491424406595964958/1572648516684357847)

**Practical question:** What actions should an agent be allowed to perform automatically, and which should require checking or explicit approval?

## Why We Ask for Divergence

The [Academy session on 17 November](https://youtu.be/HtjWrisDcSg) examined the tension between systems built from fixed rules and the varied ways that people actually think and create.

A recurring problem described in the call is that, after making a mistake, an agent may suggest adding another rigid instruction to prevent it happening again. Some rules are essential, especially for safety. But accumulating them can make a creative or complex workflow less adaptable. The group considered how to maintain the context and relationships that make an agent a useful partner without reducing every situation to an ever-growing checklist.

The discussion broadened into the value of **divergent thinkers and unconventional experiments**. Members argued that formal technical expertise should not become a barrier to participation: people with different backgrounds may notice assumptions, try unexpected approaches and uncover possibilities that established workflows miss. This is an invitation to include a wider range of perspectives, not a claim that every unconventional idea will succeed.

The conversation linked this philosophy back to very practical matters: persistent memory, agent skills, context windows, local models and how people learn to work with AI. Rather than report those subjects here a second time, the memory and workflow lessons are collected in the sections below.

**Watch:** [Full Academy session](https://youtu.be/HtjWrisDcSg) · [Short edit](https://youtu.be/quvhbZhNces) · [Divergent thinking, 24:05](https://youtu.be/HtjWrisDcSg?t=1445)

## The ResonantDAO Contribution Economy

The [ResonantDAO Exploration and Community call on 16 November](https://youtu.be/uvatiLPDFKI) moved from the project's vision to a demonstration of its emerging **Contribution Economy** workflow.

The premise is that meaningful work in a community does not always resemble a centrally assigned task. A person may build software, document an experiment, mentor a newcomer, test a tool or help others move a project forward. The proposed system aims to recognise value that members can **describe, evidence and have verified by peers**.

Victor demonstrated a prototype in which a contributor enters a description and evidence, selects verifiers, and follows a review and settlement process. The session notes report that **11 of the planned 22 workflow dimensions** were implemented in the demonstration at that point. The next proposed steps include completing the remaining dimensions, opening a test environment and improving the user experience. This is progress on a working prototype, not a claim that the full economy has launched.

A substantial part of the Q&A explored what the *dimensions* mean. They are intended to describe different beneficial outcomes, rather than a fixed list of jobs that leaders assign from the top down. The chat also raised a useful evidence question: how should the system judge whether proof is valid, authentic, current, reliable and sufficient? Those criteria were suggested for consideration, not formally adopted in the call.

The proposed token model separates **non-transferable contribution-based governance power** from a **transferable economic token**. The purpose is to stop financial wealth from automatically purchasing community decision-making power while providing a possible mechanism for funding activity. The effectiveness of that design still needs to be tested through implementation and governance.

**Explore:** [Full recording](https://youtu.be/uvatiLPDFKI) · [Contribution workflow demonstration, 10:20](https://youtu.be/uvatiLPDFKI?t=620) · [Prototype](https://vijayee.github.io/resonantdao-example/contribution-economy/) · [ResonantDAO](https://resonantdao.com/)

**Question to carry forward:** How can peer verification recognise less visible contributions without becoming so complicated that people stop participating?

## The AI Hardware Dilemma: Buy, Build or Wait?

The same purchasing problem appeared in `#local-hardware-lab` and the **18 November AI Stack chat**: what machine should someone buy for their own agents, and is buying hardware even the best first step?

Members compared full-size GPUs, prebuilt machines, high-memory systems and devices such as the DGX Spark. One member described a budget around **£5,000** and asked for guidance; others emphasised that model choice, intended workloads, location, availability, memory requirements and the possibility of waiting all change the answer. Real-world experiences with RTX 3090 and 5090 systems, storage, cooling, noise and power consumption added further context.

There was also a counterargument to beginning with a shopping list. A hosted model or inexpensive subscription can help someone discover what an agent harness does and what kinds of work they actually want to run. Members recommended experimenting with smaller local models and manageable tools before committing to a large build.

Two constraints were particularly clear: **VRAM is not the same as system RAM**, and more graphics cards are not automatically better if the system cannot move data between them efficiently. Hardware advice in these conversations reflects individual setups and budgets; it should not be taken as a universal buying recommendation.

**From Discord:** [A £5,000 hardware question](https://discord.com/channels/1423225702135894111/1517639386215350424/1572250717144616982) · [Why workload and location matter](https://discord.com/channels/1423225702135894111/1517639386215350424/1572251321304744098) · [Starting with a small local model](https://discord.com/channels/1423225702135894111/1491424406595964958/1572623933142999272)

**From AI Stack chat:** [Second-GPU bottlenecks, video](https://youtu.be/nU7hEHanTPk) · [WiCi local AI research](https://wici.ai/)

## When an AI Remembers Too Much or Too Little

The 17 November Academy conversation returned to a problem familiar to anyone working with agents over long periods: a system may remember large quantities of text yet lose the **narrative behind important decisions**.

When a context window fills, an agent harness may compact earlier exchanges into a shorter summary. This can keep a session going, but some reasoning, history and nuance are lost. On the other hand, loading too many instructions or automatically generated skills can crowd the working context and make the agent less responsive to the current task.

Hermes provided a concrete example. Members discussed auto-generated `SKILL.md` files that may work well with one model but become unnecessary or restrictive after an upgrade. They also discussed checking third-party skills for prompt-injection risks and keeping Git snapshots so that broken changes can be rolled back.

**Practical takeaways from the session:**

- Review automatically created skills instead of accumulating them indefinitely.
- Keep important project definitions and decisions in a clear external reference document.
- Break large coding projects into smaller components that can be inspected and changed independently.
- Keep verbose logs in files, with concise summaries in the conversation.
- Use fresh sessions or branches when exploratory work begins to overwhelm the main thread.

These are approaches members recommended or reported using, not a single agreed standard for every agent system.

**Watch:** [Academy discussion of memory and compaction, 10:15](https://youtu.be/HtjWrisDcSg?t=615) · [Managing Hermes skills, 37:07](https://youtu.be/HtjWrisDcSg?t=2227) · [Beginner workflow advice, 51:56](https://youtu.be/HtjWrisDcSg?t=3116)

## NVIDIA, Market Corrections and the Cost of AI Infrastructure

The [Augmented Minds call on 12 November](https://youtu.be/kvWPV9_ypT0) examined the shock around **Jensen Huang's departure from NVIDIA**, the stock-market response and what the episode might mean for an AI industry heavily dependent on a small number of infrastructure suppliers.

NVIDIA [announced the CEO transition on 12 November](https://nvidianews.nvidia.com/news/nvidia-announces-ceo-transition), naming Colette Kress interim CEO. The call considered how investors respond to executive uncertainty, whether market price movements reflect long-term fundamentals, and how the fortunes of NVIDIA, AMD and Intel are connected to demand for compute. Participants expressed different views about short-term trading and long-term investment; these are perspectives, not investment recommendations.

The most durable questions extend beyond the day's market movement. How quickly can data-centre capacity expand? Where will the electricity come from? What happens when AI infrastructure depends on specific hardware, energy supplies or leadership teams?

The discussion also moved to **agent-to-agent communication and payments**, including Google's A2A protocol and x402-related approaches. These developments suggest a future in which agents may transact with services and one another, making security, permissioning and oversight even more important.

We have not reproduced unverified allegations about individuals from the live chat. They are not necessary to understand the technical and economic discussion.

**Watch and read:** [Augmented Minds recording](https://youtu.be/kvWPV9_ypT0) · [Infrastructure and energy, 54:04](https://youtu.be/kvWPV9_ypT0?t=3244) · [Agent payments, 1:12:45](https://youtu.be/kvWPV9_ypT0?t=4365) · [NVIDIA's official transition announcement](https://nvidianews.nvidia.com/news/nvidia-announces-ceo-transition)

## Agents Working Together

Several conversations considered how a collection of agents might divide up work, instead of expecting one model to handle everything inside a single expanding context window.

In `#local-hardware-lab`, members discussed using a **larger-context orchestrator** to coordinate narrower specialist agents. Others explored personal AI personalities or 'AI Superteams' that could eventually be moved from hosted services to their own machines. Those are experiments and plans at different stages, not a single deployed community architecture.

The AI Stack chat also raised a practical question from a Hermes user: **should different bots use different models?** A model suited to writing, routing or summarisation may not be the best model for coding or reviewing a risky action. The sensible starting point is to define the job, test the candidate models on that job, and consider cost and latency alongside quality.

The broader interoperability question came up in Augmented Minds through [Agent2Agent (A2A)](https://github.com/a2aproject/a2a) and [Google's introduction to A2A](https://developers.googleblog.com/en/a2a-a-new-era-of-agent-interoperability/). Protocols offer ways for different agent applications to communicate, but communicating successfully is not the same as having trustworthy delegated authority.

**From Discord:** [Orchestrator and specialist agents](https://discord.com/channels/1423225702135894111/1517639386215350424/1572227874130366516) · [Personal AI Superteams](https://discord.com/channels/1423225702135894111/1517639386215350424/1572252082684170321)

## Experiments, Projects and Exploration

Community experiments ranged from creative video to locally generated game experiences.

In `#video-generation`, a member shared work made with **Seedance 2**, describing text-to-video experiments with character consistency, action and unusual camera perspectives. Another shared a short project created around a gaming group's final session before a friend's family commitments changed. These examples show the community using tools to make work that has a personal context, not simply to test a benchmark.

In `#ai-models`, members discussed generative role-playing games such as [Skaldsong](https://store.steampowered.com/app/3808550/Skaldsong/). The reported experience was mixed: locally generated scenarios can be enjoyable, but longer play sessions may drift or become inconsistent. Some participants still preferred older, more deterministic methods for non-player-character behaviour.

These experiments complement the technical conversations. They give people concrete reasons to care about better memory, more reliable agents and accessible hardware.

**From Discord:** [Seedance 2 text-to-video experiment](https://discord.com/channels/1423225702135894111/1544435111934566460/1572660346039181394) · [A one-day creative video challenge](https://discord.com/channels/1423225702135894111/1544435111934566460/1572657858099810546) · [Skaldsong experience](https://discord.com/channels/1423225702135894111/1491424406595964958/1572650758686638102)

## Recordings and short edits

New recordings and edits available for this issue:

- **[Academy: Divergence, 17 November](https://youtu.be/HtjWrisDcSg)** · [Short edit](https://youtu.be/quvhbZhNces)
- **[ResonantDAO Exploration and Community, 16 November](https://youtu.be/uvatiLPDFKI)** · Contribution Economy prototype demonstration
- **[Augmented Minds: The Corrections, 12 November](https://youtu.be/kvWPV9_ypT0)** · Market, infrastructure and agent payment discussions
- **AI Stack, 18 November:** No meeting recording is available. This issue draws on the chat supplied separately; it does not reconstruct what was said on the call.

The two edits from the **10 November Academy** were already featured in RW 001 and are intentionally not repeated here.

## Key terms

- **Agent harness:** The software environment that lets a model maintain a working session and use tools or other services.
- **Guardrail:** A check or restriction intended to reduce unsafe or unwanted model or agent behaviour.
- **Context window:** The information available to a model during a particular interaction, subject to a token limit.
- **Compaction:** Summarising older context to make room for new information; some detail may be lost.
- **VRAM:** Memory on a graphics processor, often a major constraint when running local AI models.
- **Orchestrator:** An agent or process that coordinates work delegated to other agents or tools.
- **Contribution token:** In the proposed ResonantDAO model, a non-transferable record of verified contribution linked to governance participation.
- **A2A:** Agent2Agent, a protocol for communication between agent applications.

---

### About this issue

Resonant Weekly is a curated account of discussions, experiments and developments from the Augmentatist community. It is not a full transcript or a statement of consensus. Individual experiences and opinions are described as such, and technical claims may require independent testing.

**Sources:** Selected Discord channels and public threads exported on 19 November 2026 (839 messages, including early messages from 19 November); meeting notes and recording links supplied by the community; AI Stack chat from 18 November; and an independent NVIDIA announcement. The editorial reporting window is **12–18 November 2026**. Original raw Discord exports are retained separately in the restricted source archive.

**Previous issue:** [Resonant Weekly 001](https://github.com/ximonomix/resonant-weekly/blob/main/Resonant-Weekly-001-2026-11-12.md)
