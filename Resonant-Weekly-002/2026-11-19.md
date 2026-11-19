# Resonant Weekly 002

**19 November 2026 | Community discussions from 12–18 November**

**What happens when we give AI systems more autonomy?** Discussions this week touched on security, memory, local control, collaboration and community governance.

## In this issue

1. [Agent Security and Guardrails](#agent-security-and-guardrails)
2. [Why We Ask for Divergence](#why-we-ask-for-divergence)
3. [The ResonantDAO Contribution Economy](#the-resonantdao-contribution-economy)
4. [Local AI Hardware: What Do You Actually Need?](#local-ai-hardware-what-do-you-actually-need)
5. [Local Agents, Privacy and Independence](#local-agents-privacy-and-independence)
6. [Agent Memory, Compaction and Skills](#agent-memory-compaction-and-skills)
7. [NVIDIA and AI Infrastructure](#nvidia-and-ai-infrastructure)
8. [Agents Working Together](#agents-working-together)
9. [Experiments, Projects and Evaluation](#experiments-projects-and-evaluation)
10. [Recordings and Short Edits](#recordings-and-short-edits)
11. [Key Terms](#key-terms)

---

## Agent Security and Guardrails

In `#ai-models` on 18 November, members discussed checking agents' outbound requests with smaller security models, including **IBM Granite Guardian** and **NVIDIA NeMo Guardrails**. Questions included model updates, what a guardrail can detect, and latency when a larger checking model runs on a CPU. No configuration was reported as tested.

**Discord:** [Original discussion](https://discord.com/channels/1423225702135894111/1491424406595964958/1572641112751997019) · [NeMo updates](https://discord.com/channels/1423225702135894111/1491424406595964958/1572642879271080008) · [CPU and model-size trade-offs](https://discord.com/channels/1423225702135894111/1491424406595964958/1572648516684357847)  
**Project:** [NVIDIA NeMo Guardrails](https://github.com/NVIDIA-NeMo/Guardrails)

## Why We Ask for Divergence

The **17 November Academy** call discussed why divergent thinkers and people from different backgrounds matter to the community, alongside the limitations of rigid agent rules. Much of the session moved into practical issues: persistent memory, context windows, agent skills, local models and learning to build with AI.

**Watch:** [Full Academy call](https://youtu.be/HtjWrisDcSg) · [Short edit](https://youtu.be/quvhbZhNces) · [Divergent thinking, 24:05](https://youtu.be/HtjWrisDcSg?t=1445)

## The ResonantDAO Contribution Economy

At the **16 November ResonantDAO call**, Victor demonstrated how a contributor can submit evidence, select peer verifiers and receive a settlement decision. The session reported **11 of 22 planned workflow dimensions** built in the prototype. Members questioned what counts as value, how evidence should be assessed and how governance tokens would differ from transferable economic tokens. The full contribution economy has not launched.

**Watch:** [Full recording](https://youtu.be/uvatiLPDFKI) · [Contribution submission, 10:20](https://youtu.be/uvatiLPDFKI?t=620) · [Peer verification, 12:50](https://youtu.be/uvatiLPDFKI?t=770)  
**Projects:** [Interactive contribution prototype](https://vijayee.github.io/resonantdao-example/contribution-economy/) · [ResonantDAO](https://resonantdao.com/)

## Local AI Hardware: What Do You Actually Need?

A **£5,000 hardware question** in `#local-hardware-lab` led to comparisons of GPUs, high-memory systems and smaller starting setups. The **18 November AI Stack chat** added discussions of RTX 5080/5090 builds, DGX Spark, power draw, cooling and second-GPU bottlenecks. Members' suggestions depended on workload, budget and location; there was no single agreed build.

**Discord:** [The £5,000 question](https://discord.com/channels/1423225702135894111/1517639386215350424/1572250717144616982) · [Workload and location](https://discord.com/channels/1423225702135894111/1517639386215350424/1572251321304744098) · [Trying a smaller local model](https://discord.com/channels/1423225702135894111/1491424406595964958/1572623933142999272)  
**Shared resources:** [Second-GPU bottlenecks (video)](https://youtu.be/nU7hEHanTPk) · [WiCi local AI research](https://wici.ai/)

## Local Agents, Privacy and Independence

A member wanted to move personal AI characters away from a hosted platform. The replies distinguished **running your own agent** from **running the model locally**: some recommended beginning with a local agent and hosted inference, then switching providers or moving inference in-house. Others cautioned that locally running software can still send data outward through harnesses and connected tools.

**Discord:** [Start with a local agent](https://discord.com/channels/1423225702135894111/1491424406595964958/1572608804204318882) · [Local does not automatically mean private](https://discord.com/channels/1423225702135894111/1491424406595964958/1572619850080059473) · [Getting started with local models](https://discord.com/channels/1423225702135894111/1491424406595964958/1572623933142999272)

## Agent Memory, Compaction and Skills

The **17 November Academy** covered how context compaction can lose the narrative behind decisions, and how accumulated auto-generated Hermes skills can become noise. Practical suggestions included auditing `SKILL.md` files, checking third-party skills for prompt injection, keeping project decisions outside chat and taking Git snapshots before changes.

**Watch:** [Context and compaction, 10:15](https://youtu.be/HtjWrisDcSg?t=615) · [Hermes skills, 37:07](https://youtu.be/HtjWrisDcSg?t=2227) · [Modular workflows, 51:56](https://youtu.be/HtjWrisDcSg?t=3116)

## NVIDIA and AI Infrastructure

The **12 November Augmented Minds** call discussed NVIDIA's leadership change and market reaction, alongside compute demand, data-centre power requirements and the future cost of AI infrastructure. Financial interpretations expressed in the call were participants' views, not established investment conclusions.

**Watch:** [Augmented Minds: The Corrections](https://youtu.be/kvWPV9_ypT0) · [Infrastructure and power, 54:04](https://youtu.be/kvWPV9_ypT0?t=3244)  
**Reference:** [NVIDIA CEO transition announcement](https://nvidianews.nvidia.com/news/nvidia-announces-ceo-transition)

## Agents Working Together

Members compared orchestration approaches, specialist agents and personal **AI Superteams**. In `#harnesscraft`, one member described building a **provider-lane scheduler** to queue concurrent local agents and preserve KV caches across three runners, rather than letting sessions compete for the same resources. The discussions did not describe one unified community system.

**Discord:** [Orchestrators and specialists](https://discord.com/channels/1423225702135894111/1517639386215350424/1572227874130366516) · [Personal AI Superteams](https://discord.com/channels/1423225702135894111/1517639386215350424/1572252082684170321) · [Local agent scheduling and KV caches](https://discord.com/channels/1423225702135894111/1546522589852340280/1572692468527276083)

The Augmented Minds call also touched on **A2A communication and agent payments**, including x402-related approaches.

**Watch:** [Agent payments, 1:12:45](https://youtu.be/kvWPV9_ypT0?t=4365)  
**Projects:** [A2A specification](https://github.com/a2aproject/a2a) · [Google's A2A introduction](https://developers.googleblog.com/en/a2a-a-new-era-of-agent-interoperability/) · [x402 and AP2 background](https://www.coinbase.com/en-gb/developer-platform/discover/launches/google_x402)

## Experiments, Projects and Evaluation

**Sketches for AI image generation.** A member shared rough drawings alongside finished thumbnails, showing how sketches can convey composition, negative space and lighting choices that are difficult to describe in prompts. The post prompted further discussion of visual control and model behaviour.

**Discord:** [Sketch-to-image examples and discussion](https://discord.com/channels/1423225702135894111/1544435111934566460/1571516616242634782)

**Replacing characters in existing video.** Another member experimented with placing friends into existing footage. After weeks of tests, they reported one successful scene, character sheets and many unexpected outcomes, along with a warning about the time required even for a short video.

**Discord:** [Character-replacement experiment](https://discord.com/channels/1423225702135894111/1544435111934566460/1572648172403036161)

**What counts as a useful AI evaluation?** In `#harnesscraft`, members discussed applying scientific methods when comparing models and agent harnesses, including the difference between a reproducible experiment and a tool that merely preserves an audit trail. CyberAlchemy Lab was shared and challenged as part of that discussion; no consensus was established.

**Discord:** [Scientific testing of agents](https://discord.com/channels/1423225702135894111/1546522589852340280/1571796805585477655) · [A/B testing and evidence](https://discord.com/channels/1423225702135894111/1546522589852340280/1572263764827447328)  
**Project:** [CyberAlchemy Lab](https://github.com/cyberAlchemyAI/CyberAlchemy-lab)

**Other shared experiments:** [Seedance 2 tests](https://discord.com/channels/1423225702135894111/1544435111934566460/1572660346039181394) · [Skaldsong discussion](https://discord.com/channels/1423225702135894111/1491424406595964958/1572650758686638102) · [Skaldsong project](https://store.steampowered.com/app/3808550/Skaldsong/)

## Recordings and Short Edits

- **Academy, 17 November:** [Divergence (full recording)](https://youtu.be/HtjWrisDcSg) · [Short edit](https://youtu.be/quvhbZhNces)
- **ResonantDAO, 16 November:** [Exploration and Community](https://youtu.be/uvatiLPDFKI) · Contribution Economy demo
- **Augmented Minds, 12 November:** [The Corrections](https://youtu.be/kvWPV9_ypT0) · Markets, AI infrastructure and agent payments
- **AI Stack, 18 November:** No recording; coverage is based on the separately supplied chat.

## Key Terms

- **Agent harness:** Software that connects an AI model to tools and a working session.
- **Guardrail:** A check or restriction intended to reduce unwanted agent behaviour.
- **Context window:** Information available to a model during an interaction.
- **Compaction:** Shortening earlier context to make room for new information.
- **VRAM:** Graphics-card memory; often a constraint when running models locally.
- **KV cache:** Reusable attention data from earlier tokens. Losing it can increase compute and latency.
- **Orchestrator:** An agent or process coordinating specialist agents.
- **Contribution token:** In ResonantDAO's proposed design, a non-transferable record of verified contribution linked to governance.
- **A2A:** Agent2Agent, a protocol for communication between agent applications.

---

**About this issue:** A selection of community discussions, experiments and shared resources, not a transcript or statement of consensus. Reporting window: **12–18 November 2026**. The AI Stack material comes from chat, not a recording.

**Previous issue:** [Resonant Weekly 001](https://github.com/ximonomix/resonant-weekly/blob/main/Resonant-Weekly-001-2026-11-12.md)
