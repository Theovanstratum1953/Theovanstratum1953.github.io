---
title: "The P85 Standard"
subtitle: "Why 85% Confidence Is the Only Honest Commitment"
date: 2026-02-10
draft: false
categories: ["probability"]
tags: ["P85", "Probability", "Actuarial", "Forecasting", "Commitments"]
summary: "What actuaries have known for a century that software organisations are only now beginning to discover — and why anything below P85 is an unhedged gamble."
---

Every commitment you have ever made about a software delivery date has been a number without a probability attached to it.

"We will ship by March 14th." Full stop. No confidence level. No distribution. No acknowledgment that March 14th is one point on a range of outcomes, some earlier, most later, a few catastrophically so.

This is not how professionals who take risk seriously communicate. It is not how actuaries work, or insurers, or anyone whose career depends on the accuracy of their forecasts rather than the confidence of their presentation.

It is, however, how almost every software organisation in the world makes its commitments. And it is why those commitments are wrong so consistently that experienced practitioners have developed a private mental correction factor — take whatever the project manager says and add eight weeks.

## What P85 Means

P85 is the date at which, given your historical delivery data and a Monte Carlo simulation of your system, 85% of modelled outcomes complete successfully.

It is not a guarantee. Nothing in a stochastic system is a guarantee. It is a defensible probability, derived from evidence, communicated honestly.

The choice of 85% is not arbitrary. It mirrors the standard used in actuarial science for insurable commitments — the threshold at which a risk can be underwritten without being considered reckless. Below P85, you are not making a commitment. You are making a bet, and asking your stakeholders to absorb the downside without knowing they have accepted it.

## The Commitment You Are Actually Making

When a project manager presents a delivery date with no confidence level attached, they are implicitly presenting their P50 — the date by which roughly half of plausible outcomes complete.

Think about that. The standard practice in software governance is to make commitments that have approximately a fifty percent chance of being met. This is not a cynical observation. It is a mathematical description of what a point estimate without a probability distribution actually means.

A P50 commitment is a coin flip dressed in a Gantt chart.

The reason organisations use P50 without knowing it is not malice. It is that estimators anchor on the most likely scenario — the one where everything goes approximately to plan — and then present that scenario as the plan. The tail of the distribution, where the interesting and painful things live, is edited out of the presentation before it reaches the stakeholder.

The stakeholder, reasonably, assumes they have been given a realistic date. They plan around it. They make their own commitments based on it. When the tail arrives — as tails do, reliably, in roughly half of all projects — the consequences cascade.

## What Changes When You Use P85

The first thing that changes is the date. A P85 commitment is almost always later than a P50 commitment. Sometimes by days. Often by weeks. Occasionally by months, particularly in high-variance systems.

This is uncomfortable. Leadership does not want a later date. The market does not want a later date. The sales team has already told the customer a date that was optimistic even at the time.

The discomfort is the point. The P85 standard does not create the uncertainty — it reveals it. The risk was always there, accumulating in the tail of the distribution, invisible in the dashboard, unacknowledged in the standup. P85 makes the honesty explicit.

The second thing that changes is accountability. When you commit to a P85 date and miss it, you have encountered a genuine one-in-seven event. You can analyse it, learn from it, and update your model. When you commit to a P50 date and miss it, you have encountered Tuesday. There is nothing to learn. The failure was priced in.

## The Organisation That Cannot Handle Truth

Some organisations, when presented with P85 dates, reject them. The dates are too conservative. The market will not accept them. The CEO has already promised the board a date and that date is not changing.

This is a governance failure, not a statistical one. The probability does not negotiate. The distribution does not adjust itself to meet the board's expectations. The tail will arrive on its own schedule, indifferent to the commitments that were made in its absence.

The choice is not between a comfortable date and an uncomfortable date. The choice is between an honest date and a dishonest one. The consequences arrive either way. Only one approach gives you the chance to prepare for them.

---

*This post draws on research from* Probabilistic Delivery: The Actuarial Science of Software Governance *(2026).*
