---
layout: page
title: Gravitational-wave inference and precessing searches
description: Sampler-free parameter estimation for compact binary coalescences, and template banks for precessing binary black holes.
importance: 3
related_publications: true
---

The same questions that drive my exoplanet work, how to detect a weak signal reliably and how to compute a posterior quickly enough to use it at scale, appear in gravitational-wave astronomy, and I am part of a group working on both.

In {% cite Mushkin2025dotPE %} we present a method to compute the posterior distribution of a compact binary coalescence without a stochastic sampler. We select sets of intrinsic and extrinsic parameters that efficiently cover the relevant phase space and evaluate the likelihood for all their combinations with dot products, with a controllable integration accuracy. Full parameter estimation then takes minutes on a single CPU. The method is implemented in the dot-PE package and makes it possible to run searches that use the full evidence integral for precessing binaries with waveform banks of 10<sup>5</sup>–10<sup>6</sup> templates.

In {% cite Zhou2026precessing %} we address searches for binary black holes whose spins are misaligned with the orbital angular momentum, which almost all previous LIGO–Virgo–KAGRA searches have neglected. Using the precession harmonic decomposition, we filter each harmonic separately and marginalize over the harmonic signal-to-noise ratios in the detection statistic; marginalizing rather than maximizing increases the sensitive volume of the search by about 10%.
