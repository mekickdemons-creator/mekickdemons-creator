Michael Anderson
Agent Runtimes & Orchestration Infrastructure
mekickdemons@gmail.com | [github.com/mekickdemons-creator](https://github.com/mekickdemons-creator)

I build the layer between the model and the work, and the layer between agents and each other.

Most developers treat agentic engineering as a prompt engineering or vector search problem. They are wrong. The bottleneck on agent performance isn't model capability—it is state degradation. When an agent's context window becomes cluttered with stale tool payloads, redundant observations, and behavioral drift, intelligence collapses.

The ceiling on agent quality isn't what the model can do; it’s whether the right facts occupy the right tokens at the exact millisecond of execution. I build runtimes that enforce strict state hygiene, dynamic context injection, and total deterministic grounding.

🎯 The Zero-Hallucination Guardrail
Models don't hallucinate out of malice; they fill vacuums left by bad architecture. I view hallucination not as an unavoidable flaw in an LLM's weights, but as a structural failure of its runtime environment.

My runtime architectures enforce absolute, deterministic boundaries between the agent and its source of truth. By controlling exactly how and when state is surfaced, hallucination is rendered structurally impossible. The model is constrained to execute solely over verifiable reality. If a fact isn't true, real, and verifiable, the runtime doesn't allow it to exist. Period.

🛠️ The Architecture I Build (Proprietary)
1. Agent Runtimes & Context Hygiene
Dynamic Role-Doc Pinning: Techniques that force model compliance across long horizons by rewriting and pinning role documents dynamically per turn, eliminating the "middle-of-the-context" attention drop.

Context Pruning & Compaction: Real-time algorithms that actively compress historical conversation turns and tool outputs into semantic summaries before hitting the context window limit, preserving high-fidelity reasoning over hundreds of turns.

State Machines over Linear Prompts: Replacing loose conversational loops with rigid, deterministic execution graphs where models act as routers rather than unconstrained drivers.

2. Multi-Agent Orchestration & Communication Layers
Message Routing Fabric: Pub/Sub architectures for agents, enabling asynchronous dispatch, parallel execution, and structured state handoffs without exploding token overhead.

Work-Tracking Primitives: Deterministic tracking systems that allow a supervisor agent to audit, pause, or roll back the state of a subordinate agent if an execution branch fails.

3. Runtime Telemetry & Guardrails (Self-Monitoring)
Anti-Looping Guards: Deterministic runtime monitors that detect and halt agents exhibiting "no-progress" behaviors, infinite polling, or repetitive tool calls.

Sycophancy & Drift Mitigation: Real-time semantic analysis of agent outputs to catch behavioral drift or echo-chamber validation before it skews the objective graph.

🚀 Public Facing Sandbox
Mnemara
An open-source Python conversation runtime alpha.

The Framework: An early, public proof-of-concept focused on micro-managing the state window by re-reading and pinning a behavioral role doc on every API call.

The Status: Archived / Core Concepts Only. Mnemara represents the baseline foundation of my early work. My current state-of-the-art orchestration layers, zero-hallucination guardrails, and multi-agent routing engines are lightyears ahead of this repository and are maintained entirely within my private, proprietary stack.

💻 How I Build (The AI Co-Authorship Thesis)
I do not hide my AI usage; I treat LLMs as high-throughput compilation targets.

I co-author openly with Anthropic’s Claude.

Every commit substantially shaped by AI receives a formal Co-Authored-By: trailer in the git log.

Hiding AI co-authorship while building infrastructure meant to coordinate AI agents is architecturally incoherent.

⚡ Availability & Consulting
Open to part-time consulting, architecture reviews, and contract engineering (~20 hours/week).

If your team is hitting a wall where your agents work beautifully for 3 turns but lose their minds by turn 15, you have a runtime problem, not a prompt problem. I fix that.

Focus Areas: Rolling-window context architectures, custom tool-orchestration layers, local-first agent deployments (Gemma 4 / Ollama stacks), and self-monitoring runtime guardrails.

Contact: Open an issue on Mnemara, or reach out directly via email at mekickdemons@gmail.com.

*Synthesized and structured by Gemini 1.5 Pro.*
