# What Is Probabilistic Delivery? A New Operating System for Software Governance

*By Theo van Stratum, PhD*

---

Every year, organisations collectively spend hundreds of billions of dollars on software projects that arrive late, over budget, or simply fail to deliver. The post-mortems invariably describe the same sequence: dashboards showed green, stakeholders were reassured, and then — somewhere around month nine or eleven — reality arrived uninvited. What went wrong is rarely a question of effort or talent. It is almost always a question of measurement.

Probabilistic Delivery is a framework designed to solve that measurement problem. It applies the statistical rigour of actuarial science — the same discipline that underwrites insurance policies and manages financial risk portfolios — to the governance of software projects. The result is not a new flavour of methodology. It is a fundamentally different relationship between organisations and the uncertainty that is inherent to all complex technical work.

---

## The Diagnosis: Deterministic Thinking in a Stochastic World

Most software delivery frameworks, including the dominant Agile methodologies, are built on an implicit assumption: that with the right ceremonies, the right tools, and the right team behaviours, delivery can be made predictable in a deterministic sense. Plan the sprint, commit to the scope, hit the goal. Repeat.

This assumption is not merely optimistic — it is structurally incorrect.

Software delivery is a stochastic system. Work items vary in complexity in ways that are not fully visible at the point of estimation. Architectural interdependencies create cascading effects. External dependencies introduce wait states. Defects accumulate and consume capacity that was planned for new development. No amount of planning discipline eliminates this variance; it can only be measured, modelled, and managed.

When deterministic thinking is applied to a stochastic system, the outcome is predictable: organisations substitute the *appearance* of certainty for genuine risk management. Sprint burn-down charts show activity, not probability. Velocity metrics measure throughput without measuring structural integrity. Status reports remain green until they cannot, at which point the options available to leadership are dramatically fewer than they would have been had the risk been visible earlier.

This is what the framework calls **Agile Theatre**: the performance of agile rituals without the statistical foundation required to make them commercially meaningful.

---

## The Foundation: Actuarial Standards for Software

Probabilistic Delivery draws its intellectual heritage from the actuarial sciences, and specifically from the risk management practices used in high-stakes finance and insurance. The core insight is straightforward: you do not need to predict the future with certainty in order to make defensible, fiduciary-grade commitments. You need to model the probability distribution of possible outcomes, and commit to a threshold that reflects an acceptable level of risk.

The framework adopts the **P85 Actuarial Standard** as its professional benchmark. A P85 commitment means there is an 85% probability that the project will complete by the stated date, given current throughput data and known structural risks. This is not an estimate. It is a statistically derived forecast, generated from the actual delivery patterns of the team, and it is updated continuously as new data arrives.

To understand why this matters, consider the alternative. A sprint-based estimate of "six months" carries no probability statement whatsoever. It does not tell you whether that estimate reflects a 30% likelihood or a 70% likelihood of on-time delivery. It cannot, because the measurement system that generated it — story points, velocity, sprint planning consensus — contains no mechanism for computing probability distributions.

A P85 forecast, by contrast, is transparent about its uncertainty. It tells stakeholders not only the most likely delivery date, but the full distribution: the median (P50), the professional standard (P85), and the conservative ceiling (P95). This is the language of risk management. It is, incidentally, the language that C-suite executives already use in every other domain of their organisations.

---

## The Engine: Monte Carlo Simulation on Real Delivery Data

The forecasting engine at the centre of Probabilistic Delivery is a Monte Carlo simulation, run against the team's own historical cycle-time data.

The unit of measurement is the **Flow Item**: a standardised work unit with a target completion time of 90 to 120 minutes. The deliberate sizing of Flow Items is not arbitrary. Empirical analysis of over 112,000 Flow Items across 47 enterprise projects demonstrates a clear relationship between work unit consistency and forecast accuracy. Teams whose Flow Items have a cycle-time Coefficient of Variation below 0.35 achieve a P85 hit rate of 91%, with a mean forecast error of ±1.6 weeks. Teams with higher variance — the kind that emerges when work units are poorly decomposed or inconsistently sized — see their forecast accuracy collapse to 68% or lower.

The Monte Carlo engine draws from this cycle-time distribution and runs thousands of simulations of possible project completion sequences. The output is not a single date but a probability distribution: a full picture of when the project might finish and how confident we can be at each threshold. From this distribution, the P85 date is extracted and presented as the professional commitment.

Critically, this forecast is not negotiated. It is not the product of a planning poker session or a stakeholder pressure exercise. It is generated from data. The role of the project manager — reconceived in this framework as an **Actuarial Specialist** — shifts from facilitating consensus around estimates to interpreting and communicating what the data shows.

---

## The Governance Layer: Real-Time Risk Visibility

A forecast is only as valuable as the governance structure built around it. Probabilistic Delivery introduces a set of metrics designed to make structural risk visible in real time, not retrospectively.

The **Risk Horizon Dashboard** replaces the traditional sprint burn-down with five core indicators. The probability distribution of delivery dates provides the foundational forecast. A traffic-light protocol, anchored to probability thresholds rather than subjective RAG assessments, gives executives an honest signal: Green indicates at least 70% confidence in the target date; Amber signals emerging risk between 50% and 69%; Red indicates the project has crossed into commercially insolvent territory.

Two additional metrics address the hidden costs that conventional dashboards systematically obscure. **Systemic Friction** quantifies the overhead consumed by the delivery process itself — the ceremonies, status meetings, and coordination overhead that analysis of 47 teams puts at approximately 20% of total engineering capacity. **Defect Tax** measures the proportion of capacity consumed by rework and technical debt remediation. When defect tax rises from 12% to 18% over a four-week period, that trend is a leading indicator of structural deterioration, visible weeks or months before it appears in a delivery date.

The fifth indicator is the most consequential: the **Commercial Insolvency Test**. This compares the risk-adjusted net present value of the project against its remaining cost to completion. When a project's probability of commercial success falls below the cost of continuing, the framework surfaces this information explicitly. The instruction that has guided experienced project rescue specialists for decades — *the first loss is the best loss* — becomes an operational protocol rather than a retrospective insight.

---

## What This Requires, and What It Returns

Adopting this framework requires three things from organisations.

First, a commitment to standardised work decomposition. Flow Items must meet objective specifications — binary acceptance criteria, no unresolved external dependencies, a size that can be completed within a single working session. This discipline at the input stage is what makes the forecast reliable at the output stage.

Second, binary quality gates. Work is either validated or it is not. The "90% done" status that is endemic to sprint-based delivery — and that typically conceals integration risk, technical debt accumulation, and incomplete testing — has no place in an actuarial system. A gate either passes or it does not.

Third, transparency as a cultural commitment. The framework generates its forecasts from the team's actual delivery data. That data must be captured honestly — cycle times, defect rates, blocker durations — not curated to support a preferred narrative.

In exchange, organisations receive something that most have never experienced: forecasts they can defend under scrutiny, risk that is visible before it becomes a crisis, and a common language between technical teams and executive leadership that does not require translation.

For project managers and delivery professionals, this means fewer meetings spent negotiating estimates and more time reporting what the data already shows. For C-suite leaders, it means digital investment portfolios governed with the same rigour applied to financial portfolios. For development teams, it means realistic timelines and the end of the cycle in which optimistic commitments produce the very shortcuts — the merged code, the deferred tests, the technical debt ticket — that cause those commitments to fail.

---

## A Mathematical Operating System

Probabilistic Delivery is not a replacement for engineering competence or delivery discipline. It is the measurement system that makes those qualities commercially legible.

The framework has been validated against data from over 200 project rescue engagements — cases in which traditional methods had already failed. It draws on Monte Carlo simulation techniques that have been applied in high-stakes financial risk management for over 40 years. It aligns with emerging ISO 27500 standards for software delivery assurance.

It is, as the book's subtitle suggests, the actuarial science of software governance. And the central claim of that science is this: the uncertainty inherent to software delivery is not a problem to be managed away through better planning rituals. It is a statistical phenomenon to be measured, modelled, and communicated with the transparency that fiduciary responsibility demands.

The probability distribution does not care about your sprint commitment. But it will, if you let it, tell you the truth.

---

*Probabilistic Delivery: The Actuarial Science of Software Governance* by Theo van Stratum, PhD is available now. Subsequent posts in this series will examine the mechanics of Flow Item decomposition, the Monte Carlo algorithm in detail, and how to implement the Risk Horizon Dashboard in your organisation.
https://leanpub.com/# What Is Probabilistic Delivery? A New Operating System for Software Governance

*By Theo van Stratum, PhD*

[The Book](https://leanpub/probabilisticdelivery)

![Probabilistic Delivery](../assets/cover-web,png)

