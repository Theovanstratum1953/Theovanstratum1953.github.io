---
title: "What Is Probabilistic Delivery?"
subtitle: "A New Operating System for Software Governance"
date: 2026-01-15
draft: false
categories: ["governance"]
tags: ["Probabilistic Delivery", "Monte Carlo", "P85", "Agile", "Software Governance", "Actuarial"]
summary: "Why dashboards lie, story points fail, and actuarial science is the only honest alternative to the comfortable fiction of sprint velocity."
---

Look around the room at your next sprint review.

There is a dashboard on the screen. It has a burn-down chart, a velocity metric, a projected completion date. The numbers are tidy. The trend lines are reassuring. Someone in senior leadership is nodding.

Nobody in that room believes the projected completion date.

The engineers don't believe it. The project manager doesn't believe it. The Scrum Master has a private mental correction factor — take whatever the dashboard says and add eight weeks — that they have never written down because writing it down would be impolite. The VP of Engineering has been watching this particular date drift for six months, two weeks at a time, with the slow horror of someone watching a ship run aground in slow motion and having no way to stop it.

This is not a failure of execution. It is a failure of measurement. And it is costing organisations hundreds of billions of dollars every year.

## The Lie the Dashboard Tells

The sprint velocity dashboard presents a deeply uncertain, non-linear, profoundly human process as though it were a smooth, predictable machine. Story points accumulate. Burn-down lines descend. Confidence is performed professionally, by people who have learned that expressing doubt is socially and professionally dangerous.

The dashboard is not measuring delivery. It is measuring the performance of delivery. These are not the same thing.

A burn-down chart that shows 60% completion at the midpoint of a project tells you almost nothing about when the project will end. It tells you what percentage of the originally estimated work has been marked done — a number distorted by estimation error, scope change, technical discovery, and the human tendency to call things done before they are done. The remaining 40% will take however long it takes, governed by the actual statistical properties of your team's work, not by the symmetry of the chart.

## What Actuaries Know That You Don't

The insurance industry solved this problem two centuries ago. Not perfectly — nothing in a stochastic system is solved perfectly — but well enough to underwrite trillions of dollars of risk annually with a level of accuracy that would be unrecognisable to most software organisations.

Actuaries do not predict the future. They model it. They collect historical data on outcomes — how long claims take to settle, how often policies lapse, what the distribution of losses looks like in different risk categories — and they use that data to build probability distributions. From those distributions they derive confidence intervals. From those confidence intervals they make commitments.

They never make a commitment without a probability attached to it. A delivery date with no confidence level is, to an actuary, not a delivery date. It is a wish.

## The P85 Standard

The central commitment in Probabilistic Delivery is the P85 date: the date at which 85% of simulated outcomes, drawn from your historical delivery data, complete successfully.

Why 85%? Because it mirrors the threshold used in actuarial science for insurable commitments — the confidence level at which a risk can be underwritten without being considered reckless. Below P85, you are not making a commitment. You are making a bet, with your stakeholders' time, money, and trust as the stake, without telling them they are gambling.

The P50 date — the date by which half of simulated outcomes complete — is useful for internal planning. It is the date a reasonable optimist would give you if they had looked at the data honestly. It should never leave the building. The P85 date is the only number you should ever give to a stakeholder.

Most organisations, without knowing it, are currently giving their stakeholders something between P30 and P50. They are making commitments that have a roughly one-in-two chance of being met and presenting them as plans. The gap between that and P85 is not pessimism. It is honesty.

## Inside the Monte Carlo Engine

The mechanism that produces P85 dates is the Monte Carlo simulation — a technique borrowed directly from actuarial and financial risk modelling.

The process is straightforward. You collect your historical cycle time data: the actual elapsed time for every work item your team has completed, over as long a period as you have honest records. You do not use story points. You do not use estimates. You use the real numbers, including the outliers, including the catastrophic items, including everything the dashboard was designed to smooth away.

From that data you build a distribution. Not a single average — a distribution, with its variance, its skew, its tail. That tail is where the truth lives. Most delivery disasters are tail events. The Monte Carlo simulation runs that distribution ten thousand times, each run drawing randomly from the historical data, each run producing a completion date. The spread of those ten thousand dates is your forecast. The date at which 85% of them complete is your P85 commitment.

This is not a complicated idea. It is simply an honest one.

## The Binary Gate Protocol

Probabilistic Delivery is not only a forecasting tool. It is a governance framework, and one of its most important elements is the Binary Gate Protocol: a unit of work is either done or it is not. There is no 80% complete. There is no "in review." There is no "basically finished." There is done, and there is not done.

This sounds obvious. It is, in practice, one of the most disruptive ideas in software governance.

Most organisations have elaborate taxonomies of partial completion — states like "in development," "in testing," "in review," "awaiting deployment" — that create the appearance of progress while concealing the actual state of affairs. Work that is 80% complete contributes nothing to the delivery. It consumes resources, occupies capacity, and sits in the queue generating risk. The Binary Gate Protocol forces that truth into the open.

When every work item is either done or not done, the burn-down chart stops being a comfort blanket and starts being a measurement instrument. When the Monte Carlo engine is seeded from binary completion data, the forecasts become trustworthy. When the P85 date is derived from that trustworthy forecast, the commitment is real.

## The Organisational Objection

At this point, most organisations raise the same objection. The P85 date is too late. The market will not accept it. The CEO has already committed to a date. The competitor ships faster.

These objections are understandable. They are also a description of an organisation choosing comfortable dishonesty over uncomfortable truth, and paying for that choice in the only currency that matters: repeated, predictable, expensive delivery failure.

The P85 date does not create the uncertainty. It reveals it. The risk was always there, accumulating in the tail of the distribution, invisible on the dashboard, unacknowledged in the standup. The date that feels too late is simply the honest answer to the question that was always being asked.

Organisations that have made the transition — and the empirical data from over 200 project teams supports this — achieve on-time delivery rates at P85 that are more than double the industry average. Not because they became more talented or more disciplined. Because they started measuring the right thing and committing to what the measurement actually said.

The dashboard will still be green. The Scrum Master will still be nodding. But the date on the slide will be one that someone in the room actually believes.

---

*This post is adapted from* Probabilistic Delivery: The Actuarial Science of Software Governance *(2026).*
