# Michael Anderson

I build runtimes for AI agents — and the orchestration harnesses that coordinate them. The layer between the model and the work, and the layer between agents and each other.

Currently shipping [**Mnemara**](https://github.com/mekickdemons-creator/mnemara): an open-source Python conversation runtime where the role doc is re-read on every API call and pinned as the system prompt. Rules apply on turn 20, not just turn 1. MIT, on PyPI, growing daily.

The thesis: **context management is the next big leap in intelligence.** Bigger models, longer context windows, and better reasoning all hit diminishing returns when an agent's context is cluttered with stale tool output and irrelevant turns. The ceiling on agent quality isn't model capability — it's whether the right facts are in the right place at the right moment.

## What I work on

- **Agent runtimes** — context management, role-doc-driven behavior, tool-use orchestration
- **Agentic harnesses** — multi-agent dispatch, persistent panels, cross-agent message routing, work-tracking primitives
- **Local-first AI** — running Gemma 4 26B and similar models via Ollama, no API costs, full privacy
- **Self-monitoring agents** — runtime guards that halt on no-progress, polling, drift, sycophancy

## How I work

I co-author with Anthropic's Claude openly. Every Mnemara commit substantially shaped by AI gets a `Co-Authored-By:` trailer. See [CONTRIBUTORS.md](https://github.com/mekickdemons-creator/mnemara/blob/main/CONTRIBUTORS.md) — hiding AI co-authorship in a project about working with LLMs would be incoherent.

## Availability

Open to **part-time consulting / contracts (~20 hours/week)** in the agent-runtime / LLM-tooling space. Especially interested in problems where the rolling-window or self-monitoring patterns from Mnemara apply directly. Reach me through GitHub issues on Mnemara, or by email. (mekickdemons@gmail.com)

---

[Mnemara](https://github.com/mekickdemons-creator/mnemara) · [PyPI](https://pypi.org/project/mnemara/)
