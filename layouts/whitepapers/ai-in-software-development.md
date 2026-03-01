---
title: "AI in Software Development"
subtitle: "Costs, Successes, and Failures: What the Evidence Actually Shows"
date: 2026-03-01
pdf_url: "https://drive.google.com/file/d/1kKpGEsQxmcCG4c1HjnwaUt0YjUUVsfnC/view?usp=sharing"
topics: ["AI", "Software Development", "Productivity", "Evidence-Based Research", "Technical Debt", "Security"]
type: "Research White Paper"
weight: 1
citation: "van Stratum, T. (2026). AI in Software Development: Costs, Successes, and Failures: What the Evidence Actually Shows. Research White Paper."
summary: "A rigorous synthesis of independent research on AI coding tools — finding a substantial gap between vendor marketing claims and measured outcomes, with serious structural risks that organisations are systematically underreporting."
---

The software development industry is currently experiencing one of the most significant hype cycles in its history. LinkedIn, conference talks, and vendor marketing are saturated with stories of AI coding tools delivering 50%+ productivity gains, teams shipping in days what used to take months, and companies achieving transformative ROI.

The evidence tells a more complicated story.

## Research Note

This paper synthesises findings from peer-reviewed studies, independent research organisations, and large-scale industry surveys. It deliberately prioritises evidence that contradicts the dominant narrative of AI as an unqualified productivity revolution. The goal is not pessimism, but accuracy. Organisations making multi-million dollar decisions deserve an honest picture.

## Key Findings

**The productivity evidence is far weaker than reported.** The most rigorous independent study (METR, 2025) found that experienced developers took 19% *longer* to complete tasks with AI — while simultaneously believing AI had made them 20% faster. BlueOptima's independent study of 218,000 developers found productivity gains of approximately 4%, against vendor claims of 20–55%.

**Organisational delivery performance degrades with AI adoption.** Google's DORA report (2024, 39,000+ respondents) found that every 25% increase in AI adoption correlated with a 7.2% decrease in software delivery stability and a 1.5% decrease in throughput.

**The failure rate is unprecedented.** 42% of companies abandoned the majority of their AI initiatives in 2025, up from 17% in 2024. MIT's analysis of 300+ AI initiatives found 95% delivered zero measurable return on investment.

**Security and technical debt costs are systematically underreported.** Security vulnerabilities in AI-generated code increased by 10x in Fortune 50 enterprises over six months. Veracode's study of 100+ LLMs found 45% of coding tasks introduced critical security flaws. The true total cost of ownership is 3–5x the license fee in year one.

**The skills pipeline is being disrupted.** Developers using AI scored 17 percentage points lower on skill comprehension tests (Anthropic, 2026). Junior developer employment for ages 22–25 has fallen nearly 20% since 2022. The pipeline problem will compound: the AI-generated code accumulating today will require expert remediation from a shrinking pool of developers capable of providing it.

## Where AI Genuinely Succeeds

The evidence is not uniformly negative. Consistent productivity benefits appear in specific contexts: less experienced developers on unfamiliar codebases, boilerplate-heavy tasks (unit test generation, documentation, CRUD scaffolding), greenfield projects without accumulated legacy context, and onboarding to unfamiliar technology.

The consistent pattern across credible research: AI helps where developers lack knowledge, and adds friction where developers are experts. This is the inverse of how most organisations are deploying it.

## Recommendations

For organisations evaluating AI tools: run controlled internal pilots before committing to organisation-wide rollout, budget the full total cost of ownership (not the license fee), and define measurable business outcomes — not activity metrics — before deployment.

For teams already using AI: distinguish tasks where AI is genuinely faster from tasks where it creates overhead, invest in the skill of evaluating AI output (not just generating it), and maintain deliberate practice of coding without AI assistance.

For the research community: demand independent replication of vendor-funded productivity studies and invest in longitudinal research tracking technical debt, security incidents, and team capability changes over 2–5 year horizons.

## Primary Sources

- METR (2025). *Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity.* arXiv:2507.09089
- Google / DORA (2024). *2024 Accelerate State of DevOps Report.* N=39,000+
- Anthropic (2026). *How AI Assistance Impacts the Formation of Coding Skills.*
- BlueOptima (2024). *Debunking GitHub's Claims: A Data-Driven Critique of Their Copilot Study.* N=218,000 developers
- GitClear (2024–2025). *AI Copilot Code Quality Report.* N=211M+ changed lines of code
- S&P Global (2025). *Enterprise AI Initiative Survey.* N=1,000+ enterprises
- MIT NANDA (2025). *The GenAI Divide: State of AI in Business 2025.* N=300+ initiatives
- Veracode (2025). *GenAI Code Security Report.* N=100+ LLMs, 80 coding tasks
- Apiiro (2025). *4x Velocity, 10x Vulnerabilities: AI Coding Assistants Are Shipping More Risks.*
---
