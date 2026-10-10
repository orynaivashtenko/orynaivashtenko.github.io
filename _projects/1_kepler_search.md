---
layout: page
title: Small long-period planets in Kepler data
description: An independent search for planets near the detection limit, with a calibrated false-alarm probability for every candidate.
importance: 1
related_publications: true
---

The photometric precision of Kepler is, in principle, sufficient to find Earth-sized planets on long orbits. In practice, these are the signals with the lowest signal-to-noise ratio in the data, and separating them from false alarms produced by correlated, non-Gaussian stellar and instrumental noise is what limits both the reliability of the catalog and the precision of occurrence-rate estimates for small long-period planets.

With Barak Zackay I built an independent search pipeline for small (Kepler multiple-event statistic MES ≲ 12), long-period (50–500 days) planets. The detection statistic accounts for the non-Gaussianity of the noise and includes physical priors. For every threshold-crossing event we run permutation and injection procedures that yield the probability that the event is caused by a real planet rather than by noise. The resulting background distribution has no heavy tail, with about one false alarm per search at MES ∼ 7.8, and the detection efficiency improves for MES of 7.5–9 and more than four transits. The pipeline recovers most of the faint confirmed Kepler planets and, applied to the entire Kepler data set, finds ∼50 candidate events with a high probability of being real planets {% cite Ivashtenko2025pipeline %}.

The catalog of these candidates and the occurrence rate derived from it, propagating each candidate's reality probability and radius posterior into the population inference, are the subject of the next papers in the series.
