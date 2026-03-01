---
title: "Probabilistic Python"
subtitle: "Bayesian Reasoning and Uncertainty Quantification for Academic Research"
status: "proposal"
expected: "Q3 2026"
cover: "/images/python.png"
chapters: "12 + 4 Appendices"
pages_est: "380–430"
topics: ["PyMC", "ArviZ", "Bambi", "Bayesian Inference", "MCMC", "Prior Selection", "Model Criticism"]
weight: 5
summary: "The Python answer to McElreath's Statistical Rethinking — academically rigorous, practically oriented, written for researchers who need probabilistic methods in their own disciplines."
audience: "Researchers and PhD students in any empirical discipline who need to apply Bayesian methods and communicate uncertainty in peer-reviewed publications."
---

Richard McElreath's *Statistical Rethinking* is the best introduction to Bayesian reasoning for researchers. It uses R. This book does for Python what *Statistical Rethinking* does for R — with a unified, modern toolchain and unusually strong treatment of the parts of Bayesian workflow that textbooks typically rush past.

## The Gap This Book Fills

Python has become the dominant language for scientific computing. PyMC, ArviZ, and Bambi together form one of the most powerful Bayesian modelling ecosystems available. But the resources for learning these tools are fragmented: PyMC documentation written for engineers, ArviZ tutorials that assume you already understand MCMC, Bambi examples oriented toward machine learning rather than scientific inference.

There is no single resource that takes a researcher from "I want to use Bayesian methods" to "I can build, criticise, and communicate probabilistic models in peer-reviewed work." This book is that resource.

## The Unified Workflow

The book teaches Bayesian modelling as a coherent workflow, not a collection of techniques:

**Specifying priors** with scientific justification — not as a mathematical formality but as a discipline of making assumptions explicit and defensible.

**Building models** in PyMC with a focus on interpretability and the correspondence between statistical model and scientific question.

**Running inference** with an understanding of what MCMC is doing, how to diagnose problems, and when to trust results.

**Criticising models** using posterior predictive checks, leave-one-out cross-validation, and the ArviZ toolkit — the phase of Bayesian workflow most often skipped in introductory treatments.

**Communicating uncertainty** in the language of peer-reviewed publication — credible intervals, probability statements, and visualisations that convey what the model actually says.

## What Makes This Academically Oriented

This is not a book about applying machine learning models to prediction problems. It is a book about using probabilistic models to answer scientific questions and report findings with appropriate uncertainty.

The examples are drawn from social science, epidemiology, economics, psychology, and natural science. The focus throughout is on the correspondence between the statistical model and the scientific question it is meant to answer — the connection that too many Bayesian resources treat as obvious when it is anything but.

## The Toolchain

**PyMC** for model specification and inference — the most mature and actively developed Bayesian modelling library in Python.

**ArviZ** for diagnostics, model comparison, and visualisation — the standard library for Bayesian workflow in Python.

**Bambi** for formula-based model specification — for researchers coming from R's `lme4` or Stata, Bambi provides a familiar interface to PyMC's capabilities.

The three tools are taught as an integrated workflow, not separately.

## Chapter Overview

**Part I — Foundations**
1. Why Bayes? Probability as a Language for Science
2. Setting Up the Bayesian Workflow Environment
3. Probability Distributions for Researchers
4. Your First Bayesian Model in PyMC

**Part II — Core Modelling Techniques**
5. Prior Selection — the discipline of making assumptions explicit
6. Linear Models — the Bayesian way
7. Generalised Linear Models for Research Questions
8. Hierarchical Models — partial pooling and the researcher's friend

**Part III — Advanced Models**
9. Model Criticism and Posterior Predictive Checks
10. Model Comparison with ArviZ
11. Time Series and Longitudinal Data
12. Latent Variable Models

**Part IV — Communicating Results**  
*Chapter on reporting Bayesian results for peer review, credible interval interpretation, and visualisation standards*

*Appendix A: PyMC Quick Reference*  
*Appendix B: ArviZ Diagnostics Guide*  
*Appendix C: Prior Selection Reference*  
*Appendix D: Bayesian Reporting Checklist for Peer Review*
---
