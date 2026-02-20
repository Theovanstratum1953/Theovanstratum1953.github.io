---
title: "An Introduction to Bayesian Updating"
subtitle: "For People Who Have Been Wrong Before"
date: 2026-02-20
draft: false
categories: ["probability"]
tags: ["Bayesian", "Probability", "Python", "Decision-making", "Statistics"]
summary: "A practical introduction to revising beliefs in the face of evidence — with real examples and none of the condescension of most statistics writing."
---

At some point in the last year, you updated a belief.

Maybe you started a project assuming it would take three months, saw the first month's actual progress, and quietly revised your estimate upward. Maybe you hired someone who interviewed brilliantly and spent the first six weeks wondering whether you had been wrong. Maybe you trusted a delivery date and then, after two missed milestones, stopped trusting it.

In each case, you did something statistically sophisticated: you started with a prior belief, received new evidence, and produced a revised belief that incorporated both. You did Bayesian updating, informally, without calling it that.

Bayesian statistics is simply the formalisation of this process — the machinery that lets you do it rigorously, consistently, and without the cognitive biases that make informal belief revision so unreliable.

## The Problem with How We Were Taught

Most people who learned statistics learned the frequentist version. Hypothesis testing, p-values, confidence intervals, null hypotheses. This framework has its uses. It also has a fundamental limitation: it cannot easily incorporate what you already know.

A frequentist analysis treats each dataset as if it arrived from nowhere, uncontaminated by prior knowledge. You run the test. You get a p-value. You accept or reject the null hypothesis. What you believed before you collected the data is, formally, irrelevant.

This is fine in a laboratory where you are testing a genuinely new phenomenon with no prior knowledge. It is deeply unhelpful in the messy, experience-laden, prior-knowledge-saturated world of software governance, project management, or academic research, where you almost always know something before you see the data.

You know, from thirty years of experience, that software projects have fat-tailed completion distributions. You know that teams which missed the first milestone almost always miss the second. You know that requirements described as "simple" by stakeholders are rarely simple. You know these things. Frequentist statistics gives you no formal way to use them.

Bayesian statistics does.

## Prior, Likelihood, Posterior

The Bayesian framework has three components.

The **prior** is what you believe before seeing the data. It does not have to be precise — it can be broad and uncertain, reflecting genuine ignorance — but it has to be honest. If you have experience that says software project durations follow a certain distribution, your prior should reflect that.

The **likelihood** is the probability of seeing the data you actually observed, given different possible states of the world. This is where the evidence speaks.

The **posterior** is the result of combining the two. It is your updated belief, after the evidence has been incorporated. It is more informed than the prior, but it carries the prior's influence — particularly when the data is sparse.

This matters enormously in practice. When you have very little data, your prior dominates the posterior, which is correct: limited evidence should not dramatically overturn prior knowledge. As data accumulates, the posterior converges toward what the data shows, regardless of the prior. Experience gives way to evidence, at the rate the evidence deserves.

## Why It Changes How You Think About Estimates

Consider a project that has just completed its first sprint. You have one data point. A frequentist analysis of one data point is almost meaningless — the confidence interval is enormous, the statistical power is negligible, the result is essentially noise.

A Bayesian analysis can incorporate what you knew before the sprint started: the historical distribution of your team's cycle times, the reference class of similar projects, the known risk factors for this type of work. The single data point updates that prior — modestly, appropriately, without pretending it carries more information than it does.

This is what Probabilistic Delivery does in practice. The Monte Carlo engine is seeded from a prior distribution — the historical record of what work actually took — and updated as new evidence arrives. The result is not a point estimate. It is a probability distribution, and it improves continuously as the project progresses.

## The Uncomfortable Implication

Bayesian reasoning has an implication that organisations find genuinely uncomfortable: **you are required to state your prior beliefs explicitly, before you see the data.**

This is not optional. A Bayesian analysis without an explicit prior is not Bayesian — it is frequentist with decorative notation. The prior must be stated, defended, and exposed to scrutiny.

For most organisations, this is the hard part. Stating your prior beliefs explicitly means committing to them. It means being wrong in a way that is documented and attributable. It means being unable, later, to claim that the outcome was unforeseeable when you had, in fact, published a prior that assigned it a non-trivial probability.

This accountability is not a flaw in the Bayesian framework. It is the point.

---

*Probabilistic Python: Bayesian Reasoning and Uncertainty Quantification for Academic Research is currently under proposal with an academic publisher.*
