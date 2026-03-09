# 🏢 Headcount Zero

**A full startup executive team with zero employees.**

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
[![Security Policy](https://img.shields.io/badge/Security-Policy-brightgreen?logo=github)](SECURITY.md)
![Version: v0.1.0](https://img.shields.io/badge/version-v0.1.0-5E5E5E.svg)
![Platform: Copilot CLI](https://img.shields.io/badge/platform-Copilot%20CLI-232F3E.svg)

Every startup needs a CEO, CTO, CFO, VP of Product, and a dozen other leaders before it ships anything. Headcount Zero deploys 15 AI agents as a complete Series A/B executive team. Give it one idea, get back a full startup operating package.

> ⚡ **Get started fast!** Say this in the Copilot CLI:
> ```
> startup
> ```

---

## 🎯 What It Does

You describe a startup idea in plain English. Headcount Zero runs it through a 5-phase pipeline where 15 specialist agents produce real artifacts — not advice, not summaries, but the actual documents a startup needs to operate.

**One prompt in. 25+ documents out.**

| What you'd normally need | What Headcount Zero gives you |
|--------------------------|-------------------------------|
| A CEO to set vision | `company-vision.md` + `investor-memo.md` |
| A CTO to design architecture | `architecture.md` + `tech-stack.md` |
| A CFO to model finances | `financial-model.md` + `unit-economics.md` |
| A VP Product to write PRDs | `prd.md` + `roadmap.md` + `user-stories.md` |
| A VP Marketing to plan GTM | `marketing-plan.md` + `brand-voice` |
| ... and 10 more department heads | Sprint plans, hiring plans, security posture, legal checklists, and more |

---

## 🚀 Quick Start

### Full Pipeline (5 phases, all 15 agents)
```
startup
```
Then describe your idea when prompted. You review output at each gate.

### Express Mode (vision + strategy only)
```
startup express
```
Runs just Phase 1 (CEO) and Phase 2 (CTO, CFO, VP Product). Good for early validation.

---

## 🏗️ How It Works

```
          Phase 1              Phase 2                Phase 3
       ┌──────────┐    ┌─────────────────┐    ┌──────────────────────┐
       │          │    │ CTO             │    │ VP Engineering       │
YOU ──▶│   CEO    │──▶ │ CFO             │──▶ │ Head of Design       │
       │          │    │ VP Product      │    │ VP Marketing         │
       └────┬─────┘    └───────┬─────────┘    │ VP Sales             │
            │                  │              │ Head of Growth       │
         [GATE]             [GATE]            │ Head of Data         │
       You review          You review         └──────────┬───────────┘
                                                         │
                                                      [GATE]
                                                    You review
                                                         │
          Phase 5              Phase 4                   │
       ┌──────────┐    ┌─────────────────┐               │
       │   CEO    │◀── │ Head of People  │◀──────────────┘
       │ (Board   │    │ Head of CS      │
       │  Review) │    │ General Counsel │
       └──────────┘    │ Head of DevOps  │
            │          │ Head of Security│
         [GATE]        └───────┬─────────┘
       You review              │
            │               [GATE]
            ▼              You review
     📦 Startup
        Package
```

**Each gate pauses for your review.** You can adjust, redirect, or skip ahead. The agents work for you, not the other way around.

---

## 👥 The Team

### Phase 1: Foundation
| Agent | Produces | Focus |
|-------|----------|-------|
| 🎯 **CEO** | `company-vision.md`, `investor-memo.md` | Mission, market, model, risks |

### Phase 2: Strategy (parallel)
| Agent | Produces | Focus |
|-------|----------|-------|
| ⚙️ **CTO** | `architecture.md`, `tech-stack.md` | System design, build vs buy |
| 💰 **CFO** | `financial-model.md`, `unit-economics.md` | Revenue, burn, runway, LTV/CAC |
| 📋 **VP Product** | `prd.md`, `roadmap.md`, `user-stories.md` | Features, personas, priorities |

### Phase 3: Execution (parallel)
| Agent | Produces | Focus |
|-------|----------|-------|
| 🔧 **VP Engineering** | `sprint-plan.md`, `team-structure.md` | Sprints, tickets, team topology |
| 🎨 **Head of Design** | `design-system.md`, `user-flows.md` | Brand, components, UX flows |
| 📣 **VP Marketing** | `marketing-plan.md` | Positioning, channels, launch plan |
| 🤝 **VP Sales** | `sales-playbook.md`, `pricing-strategy.md` | ICP, objections, pricing tiers |
| 📈 **Head of Growth** | `growth-plan.md` | Funnel, experiments, north star |
| 📊 **Head of Data** | `metrics-framework.md`, `dashboard-spec.md` | KPIs, dashboards, cadence |

### Phase 4: Operations (parallel)
| Agent | Produces | Focus |
|-------|----------|-------|
| 👤 **Head of People** | `hiring-plan.md`, `org-chart.md` | Roles, comp, interview process |
| 💬 **Head of CS** | `cs-playbook.md` | Onboarding, health scores, churn |
| ⚖️ **General Counsel** | `legal-checklist.md` | IP, compliance, terms, fundraising |
| 🖥️ **Head of DevOps** | `infra-plan.md`, `monitoring-plan.md` | Hosting, CI/CD, incident response |
| 🔒 **Head of Security** | `security-plan.md` | Threats, auth, data protection |

### Phase 5: Board Review
| Agent | Produces | Focus |
|-------|----------|-------|
| 🎯 **CEO** (again) | `executive-summary.md`, `90-day-plan.md` | Cross-department alignment, priorities |

---

## 📦 What You Get

After a full run, your `.company/` folder contains:

```
.company/
├── vision/
│   ├── company-vision.md            ← Mission, problem, solution, values
│   └── investor-memo.md             ← Market, model, risks, ask
├── product/
│   ├── prd.md                       ← Features, personas, success metrics
│   ├── roadmap.md                   ← Now / Next / Later
│   └── user-stories.md              ← 15-20 testable user stories
├── engineering/
│   ├── architecture.md              ← System design, data model, APIs
│   ├── tech-stack.md                ← Every tool with rationale
│   ├── sprint-plan.md               ← 6 sprints of tickets
│   └── team-structure.md            ← Roles, hiring sequence, culture
├── design/
│   ├── design-system.md             ← Colors, type, components, tone
│   └── user-flows.md                ← 3-5 critical flows with edge cases
├── finance/
│   ├── financial-model.md           ← Revenue, costs, runway projections
│   └── unit-economics.md            ← CAC, LTV, margins, break-even
├── gtm/
│   ├── marketing-plan.md            ← Positioning, channels, launch plan
│   ├── sales-playbook.md            ← Process, objections, demo script
│   ├── pricing-strategy.md          ← Tiers, psychology, competitor map
│   └── growth-plan.md               ← Funnel, experiments, north star
├── operations/
│   ├── hiring-plan.md               ← Roles, comp bands, interview process
│   ├── org-chart.md                 ← Current → 6mo → 12mo structure
│   ├── cs-playbook.md               ← Onboarding, health scores, churn
│   └── legal-checklist.md           ← IP, compliance, fundraising docs
├── infrastructure/
│   ├── infra-plan.md                ← Hosting, CI/CD, cost estimates
│   ├── monitoring-plan.md           ← Uptime, APM, incidents, SLOs
│   └── security-plan.md             ← Threats, auth, encryption, testing
├── data/
│   ├── metrics-framework.md         ← North star, input metrics, cadence
│   └── dashboard-spec.md            ← Exec, product, revenue, eng dashboards
└── synthesis/
    ├── executive-summary.md         ← Full company snapshot + gaps
    └── 90-day-plan.md               ← Prioritized actions with owners
```

---

## ⚙️ Configuration

All tunables live in `config.yml`:

| Key | Default | Purpose |
|-----|---------|---------|
| `company.default_mode` | `full` | `full` (5 phases) or `express` (2 phases) |
| `company.agent_timeout_sec` | `300` | Per-agent timeout |
| `company.max_agents_parallel` | `6` | Max concurrent agents per phase |
| `safety.require_gate_approval` | `true` | Never skip user review gates |
| `safety.max_artifact_lines` | `500` | Per-document line limit |
| `models.executive` | `claude-sonnet-4.6` | Model for CEO, CTO, CFO |
| `models.department` | `claude-sonnet-4.6` | Model for VP/Head agents |

---

## 🧪 Design Principles

- **Boring technology.** The CTO picks proven tools over cutting-edge ones.
- **Real numbers.** The CFO shows math, not hand-waving.
- **Ruthless prioritization.** The VP Product cuts scope, not adds it.
- **Practical security.** The Head of Security focuses on actual risk, not theater.
- **Hire for the stage.** The Head of People plans for a startup, not a Fortune 500.
- **One growth engine.** The Head of Growth picks one channel and goes deep.

---

## 📁 Project Structure

```
headcount-zero/
├── README.md                        ← 👋 You are here
├── CONTRIBUTING.md                  ← 🛠️ How to contribute
├── CODE_OF_CONDUCT.md               ← 🤝 Community standards
├── SECURITY.md                      ← 🔒 Security policy
├── CHANGELOG.md                     ← 📝 Version history
├── LICENSE                          ← 📄 MIT
├── SKILL.md                         ← 🏢 Main orchestrator
├── AGENTS.md                        ← 🤖 Agent development guide
├── config.yml                       ← ⚙️ Tunables
├── catalog.yml                      ← 📦 Skill metadata
├── .github/
│   └── copilot-instructions.md      ← 🧭 Copilot project rules
└── agents/
    ├── ceo.md                       ← 🎯 Vision & strategy
    ├── cto.md                       ← ⚙️ Architecture
    ├── cfo.md                       ← 💰 Finance
    ├── vp-product.md                ← 📋 Product
    ├── vp-engineering.md            ← 🔧 Engineering
    ├── head-of-design.md            ← 🎨 Design
    ├── vp-marketing.md              ← 📣 Marketing
    ├── vp-sales.md                  ← 🤝 Sales
    ├── head-of-growth.md            ← 📈 Growth
    ├── head-of-people.md            ← 👤 People
    ├── head-of-cs.md                ← 💬 Customer Success
    ├── general-counsel.md           ← ⚖️ Legal
    ├── head-of-data.md              ← 📊 Data
    ├── head-of-devops.md            ← 🖥️ DevOps
    └── head-of-security.md          ← 🔒 Security
```

---

## ❓ FAQ

**Can I skip phases?**
Yes. Say "express" to run only Phase 1-2. At any gate you can tell the orchestrator to skip ahead.

**Can I re-run a single agent?**
Not yet. Currently the pipeline runs phases in order. Re-running individual agents is on the roadmap.

**Does it work for non-tech startups?**
Yes. The CTO and engineering agents adapt their output to the idea. A restaurant concept gets a POS system architecture, not a Kubernetes cluster.

**How long does a full run take?**
Depends on your model. With `claude-sonnet-4.6`, expect 10-15 minutes for all 5 phases.

**Can I customize the agents?**
Absolutely. Each agent is a standalone markdown file in `agents/`. Edit the Role, Output, or Rules sections to change behavior.

---

## 🛠️ Contributing

Headcount Zero is early. Here are quick ways to help:

- 🐛 **Found a bug?** [Open an issue](https://github.com/DUBSOpenHub/headcount-zero/issues)
- 💡 **Have an idea?** Suggest a new agent role or output format
- 🎨 **Improve a prompt?** Submit a PR to any `agents/*.md` file
- 📝 **Test it out?** Run it on a wild startup idea and share the results

See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

---

## 📄 License

[MIT](LICENSE) — do whatever you want with it.

---

🐙 Created with 💜 by [@DUBSOpenHub](https://github.com/DUBSOpenHub).

Let's build! 🚀✨
