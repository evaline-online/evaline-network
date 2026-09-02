# Nova Line Network

Interactive **Tetraktys Topology** visualizing a network of **10 LLM agents** (Monad → Architect → Synthesizer → ... → Client Synergy). Deployed to **https://evaline.network/**.

## Features

- **10 connected agents** in a 1-2-3-4 pyramid (square tetraktys)
- **Live dataflow simulation**: animated SVG edges, message passing between nodes
- **Real interaction**: click any node → detail panel (Ping / Pulse / Toggle online)
- **Status indicators**: ONLINE / PROCESSING / OFFLINE on every node + NET health bar
- **Multi-language**: EN 🇬🇧 / UK 🇺🇦 / RU 🇷🇺
- **Dark / Light theme** toggle
- Pure HTML/CSS/JS (no framework), Roboto Mono

## The 10 Agents

| # | Key | Agent | Role |
|---|-----|-------|------|
| 01 | MONAD | Monad Prime | Orchestrator |
| 02 | ARCH | Strategic Architect | Strategy / Blueprint |
| 03 | SYNTH | Analytical Synthesizer | Analytics / Data Feeds |
| 04 | EXEC | Executive Decision | Decision / Consensus |
| 05 | RISK | Risk & Compliance | Audit & Safety |
| 06 | QUAL | Quality & Validation | Verification |
| 07 | MKT | Market Intel | Prediction |
| 08 | OPS | Operational Ops | Pipelines |
| 09 | FIN | Financial Model | Yield & Fiscal |
| 10 | SYNERGY | Client Synergy | User Interface |

## Deploy

Site is served from `/var/www/evaline.network/` on the GCloud VM `evaline-micro-vm`.

```bash
scp index.html evaline-micro-vm.us-central1-a.evabot-agent-server:/tmp/evaline-new.html
ssh evaline-micro-vm.us-central1-a.evabot-agent-server "sudo cp /tmp/evaline-new.html /var/www/evaline.network/index.html"
```
