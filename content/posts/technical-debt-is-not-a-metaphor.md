---
title: "Technical Debt Is Not a Metaphor"
subtitle: "It Is a Measurable, Compounding Financial Risk"
date: 2026-02-15
draft: false
categories: ["governance"]
tags: ["Technical Debt", "Software Governance", "Risk", "Fiduciary", "Measurement"]
summary: "The case for treating deferred quality decisions with the same fiduciary seriousness as any other form of organisational liability."
---

Ward Cunningham introduced the term "technical debt" in 1992 as a metaphor — a way of explaining to non-technical stakeholders why cutting corners today creates extra work tomorrow. It was a good metaphor. It was clear, intuitive, and memorable.

It has also allowed organisations to treat a quantifiable financial liability as a vague feeling.

"We have a lot of technical debt" has become the software equivalent of "we should really tidy the garage." Everyone agrees it is true. Everyone agrees it is a problem. Nobody measures it, prices it, or treats it with the seriousness that any other liability of comparable magnitude would demand.

## Debt That Does Not Appear on the Balance Sheet

Consider what technical debt actually represents. It is the accumulated cost of decisions made to deliver faster at the expense of quality — shortcuts in architecture, deferred refactoring, tests not written, documentation not maintained. Each of those decisions transferred a future cost from the present to some unspecified later date, in exchange for delivery speed today.

This is a financial transaction. It has a principal — the cost of the work deferred. It has interest — the compounding cost of working around the deferred work, the increased time to make changes, the higher probability of production incidents. It has a maturity risk — the possibility that the debt becomes unserviceable, that the system becomes too entangled to modify without catastrophic risk.

None of this appears on any balance sheet. None of it is reported to boards or auditors. None of it is factored into the valuations that underpin investment decisions, acquisition pricing, or strategic planning.

An organisation that borrowed fifty million dollars would have that liability disclosed, monitored, and managed. An organisation that has accumulated the equivalent in deferred engineering quality almost certainly does not know it has done so, let alone what it owes.

## The Compounding Problem

Financial debt compounds because interest accrues on the outstanding principal. Technical debt compounds for a different reason: the more of it you have, the slower every subsequent piece of work becomes.

A codebase with significant technical debt is not simply a codebase where some things need to be cleaned up. It is a codebase where every new feature takes longer, every bug fix carries higher risk of introducing new bugs, every deployment requires more manual intervention, and every engineer who joins takes longer to become productive because the system they are learning is harder to understand.

The interest rate on technical debt is not fixed. It increases as the debt grows. A team with moderate debt might work at 80% of their potential speed. A team with severe debt might work at 40%. The compounding is non-linear, and by the time it becomes visible in delivery metrics, it has typically been accumulating for years.

## Measurement Is Not Optional

The standard objection to measuring technical debt is that it is too complex to quantify. The codebase is too large. The interactions are too subtle. The future costs are too uncertain to price.

This argument would be immediately rejected in any other domain of risk management. Insurance companies price far more complex and uncertain risks every day. The uncertainty does not make measurement impossible — it makes measurement probabilistic. You do not need to know exactly what the debt will cost. You need to know its distribution.

The tools exist. Cycle time data — the actual elapsed time for work items — captures the debt's effect even when its cause is opaque. If your cycle times are increasing quarter over quarter without a corresponding increase in work complexity, the technical debt is compounding. That is a measurable signal. It has a dollar value attached to it: the difference between what your team could deliver in a debt-free system and what they are actually delivering.

## The Fiduciary Question

Here is the question that organisations consistently avoid: if the board of a company knew that a liability of this magnitude existed on the engineering balance sheet, and that it was compounding at this rate, and that it was not being managed or even disclosed — what would they say?

Technical debt is not a development team problem. It is a governance problem. The decisions that created it were often made at the request of leadership, under pressure to ship faster, in the name of business priorities that seemed urgent at the time. The responsibility for managing it belongs at the same level.

Treating technical debt as a vague feeling, a developer complaint, a thing to be addressed "when we have time" — which means never — is a fiduciary failure. It is the acceptance of a compounding liability without disclosure, measurement, or a plan for repayment.

The garage is not going to tidy itself. And unlike the garage, it is getting messier every week you leave it.

---

*This post draws on ongoing research for* The Technical Debt Paradox *(forthcoming).*
