# EvaLine Network

Interactive **Tetraktys Topology** visualizing the **10 business agents** of the **EvaLine EVA foam manufacturer** — mapping the real company functions (from raw EVA sheets to finished goods) onto a 1-2-3-4 pyramid network. Deployed to **https://evaline.network/**.

Built from the `evaline-com-ua` business archive research.

## Features

- **10 connected business agents** in a 1-2-3-4 pyramid (square tetraktys) — all squares identical size
- **Live dataflow simulation**: animated SVG edges, message passing between nodes
- **Real interaction**: click any node → detail panel (Ping / Pulse / Toggle online)
- **Status indicators**: ONLINE / PROCESSING / OFFLINE on every node + NET health bar
- **Multi-language**: EN 🇬🇧 / UK 🇺🇦 / RU 🇷🇺
- **Dark / Light theme** toggle
- Pure HTML/CSS/JS (no framework), Roboto Mono

## The 10 Business Agents

| # | Key | Agent | Line |
|---|-----|-------|------|
| 01 | HQ | Brand HQ | Headquarters / Orchestrator |
| 02 | PROD | Production | EVA sheets & figure cutting |
| 03 | SUPPLY | Supply & Compliance | Procurement / Certifications |
| 04 | B2B | B2B Sales | Wholesale / Production orders |
| 05 | B2C | B2C Retail | Online shop / Consumer |
| 06 | SPORT | Sports Line | Tatami & sports mats |
| 07 | AUTO | Auto Line | Car mats & EVA sheets |
| 08 | AGRO | Agro Line | Livestock mats "Buryonka" |
| 09 | SHOE | Shoe Line | Soles & insoles |
| 10 | SRVC | Client Service | Support / Private Label |

## Deploy

Site is served from `/var/www/evaline.network/` on the GCloud VM `evaline-micro-vm`.

```bash
scp index.html evaline-micro-vm.us-central1-a.evabot-agent-server:/tmp/evaline-new.html
ssh evaline-micro-vm.us-central1-a.evabot-agent-server "sudo cp /tmp/evaline-new.html /var/www/evaline.network/index.html"
```
