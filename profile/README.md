<div align="center">

# ClusterCode

### Hand off a ticket. Get back a PR.

**Self-hosted AI coding orchestration — your machines, your code, your cluster.**

[Website](https://clustercode.io) · [Docs](https://docs.clustercode.io) · [Console](https://console.clustercode.io) · [Discord](https://discord.gg/theclustercode) · [X](https://x.com/theclustercode)

</div>

---

## What we build

ClusterCode is a **self-hosted platform** for orchestrating agentic development across machines you already own. Register a spare laptop, a home server, or a $6 VPS as a worker, point it at your ticket board, and get back draft PRs — with the code never leaving your infrastructure.

```
🎫 Ticket  →  📦 DevBox spins up  →  🤖 Agent does the work  →  🔀 Draft PR
```

A centralized dashboard launches, monitors, and steers AI coding agents running inside isolated **DevBoxes** on your workers — on demand, on a schedule, or by chatting with an in-app assistant.

---

## The cluster

| Concept | What it is |
|---------|------------|
| **Workers** | Your machines (running Podman) — or managed Cloud workers when you'd rather not host |
| **DevBoxes** | Isolated dev environments where agents work: repo, toolchain, and agent, ready in seconds |
| **Projects** | One workspace per effort — the DevBoxes, runs, schedules, and env vars behind it |
| **Runs** | On-demand and interactive: watch the timeline, steer mid-flight, answer its questions |
| **Schedules** | Recurring autonomous cron jobs — wake up to draft PRs, flaky-test sweeps, dependency audits |
| **Engines** | Claude Code, Codex, and Copilot do the in-DevBox coding |
| **Nova** | The coordinator that orchestrates engines across a run |
| **Nucleus** | The in-app assistant — launch DevBoxes, start runs, and create schedules from a conversation |
| **Observatory** | Your whole fleet as a navigable galaxy: workers as suns, DevBoxes as planets, schedules as orbits |

---

## Why ClusterCode

🖥️ **Bring Your Own Machine** — register any machine with Podman and it's part of your cluster. No per-seat cloud sandbox pricing.

🔌 **Engine-agnostic** — Claude Code, Codex, Copilot. Mix them in a single run with real handoffs, each keeping its own session.

🎫 **Ticket-to-PR** — paste a GitHub issue or Azure DevOps work item; a DevBox spins up with the full context ready to go.

🔒 **Outbound-only** — workers connect to the orchestrator over an authenticated outbound WebSocket. Behind NAT and firewalls, zero port forwarding.

🔭 **Fully observable** — live web terminal into any DevBox, per-DevBox CPU/memory/disk, and the Observatory over the whole fleet.

---

## Getting started

```bash
npm install -g @clustercode/cli   # requires Node.js 22+
clustercode onboard               # guided login, tenant selection, runtime checks
```

Then paste a ticket link into the dashboard and pick a worker. Full walkthrough in the [Quickstart](https://docs.clustercode.io/getting-started/quickstart).

---

## Repositories

| Repo | What it does |
|------|--------------|
| **[cli](https://github.com/clustercodehq/cli)** | The `clustercode` CLI — log in, register workers, run the worker agent. Apache-2.0. |
| **[vscode-extension](https://github.com/clustercodehq/vscode-extension)** | Tend your DevBoxes without leaving the editor. Apache-2.0. |
| **[docs](https://github.com/clustercodehq/docs)** | Source for [docs.clustercode.io](https://docs.clustercode.io). |
| **[dist](https://github.com/clustercodehq/dist)** | Public distribution host for ClusterCode binaries, published as GitHub Releases. |
| **[support](https://github.com/clustercodehq/support)** | Bug reports and feature requests — [open an issue](https://github.com/clustercodehq/support/issues). |

The software that runs on *your* hardware should be open for inspection: the CLI and the VS Code extension are Apache-2.0. The orchestrator is proprietary.

---

<div align="center">

**[Get started →](https://clustercode.io/register)**

© 2026 ClusterCode LLC

</div>
