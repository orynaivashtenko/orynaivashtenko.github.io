---
layout: page
title: Gravitational-wave precessing search
description: Detecting precessing compact binary coalescences in LIGO data, getting their parameter posteriors, and computing the evidence — very quickly.
importance: 3
related_publications: true
---

The same questions that drive my exoplanet work, how to detect a weak signal reliably and how to compute a posterior quickly enough to use it at scale, appear in gravitational-wave astronomy, and are even more complex there. I have been a part of a group working on detecting and characterizing compact binary mergers in LIGO data, showing signatures of spin-orbital precession. The detection project was led by Zihan Zhou, and the parameter estimation project by Jonathan Mushkin.

In {% cite Mushkin2025dotPE %} a method was developed to compute the posterior distribution of a compact binary coalescence without a stochastic sampler. The full parameter estimation in the 15-dimensional parameter space of a compact binary merger is very computationally expensive and is one of the major bottlenecks in gravitational-wave inference. Jonathan split the parameters into two sets, intrinsic and extrinsic, and found a way to evaluate the likelihood for all their combinations with dot products. Full parameter estimation then takes minutes on a single CPU. This speed enables the use of the full evidence integral for detection, rather than a simplified detection statistic.

The work {% cite Zhou2026precessing %} builds a search pipeline for binary black holes whose spins are misaligned with the orbital angular momentum, a feature that almost all previous LIGO–Virgo–KAGRA searches have neglected. Using the precession harmonic decomposition, the search applies matched filtering to each harmonic separately and computes the final detection score by marginalizing over the harmonic signal-to-noise ratios.

I collaborated on this project in 2023, working with my supervisor Barak Zackay, and with Matias Zaldarriaga.
