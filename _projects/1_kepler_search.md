---
layout: page
title: Small long-period planets in Kepler data
description: An independent search for planets near the detection limit, with demonstrated reliability and reported "planet vs noise" probability for every candidate.
importance: 1
related_publications: true
---

The photometric precision of Kepler is, in principle, sufficient to find Earth-sized planets on long orbits. In practice, these are the signals with the lowest signal-to-noise ratio in the data, and separating them from false alarms produced by correlated, non-Gaussian stellar and instrumental noise is what limits both the reliability of the catalog and the precision of occurrence-rate estimates for small long-period planets.

With my supervisor Barak Zackay, I built an independent search pipeline for small (Kepler multiple-event statistic MES ≲ 12), long-period (50–300 days) planets. We addressed the problem of planet catalog contamination by false alarms caused by noise systematics, and developed a detection statistic that accounts for the non-Gaussianity of the noise and includes physical priors. For each threshold-crossing event, we run scrambling (permutation) and injection procedures to estimate the probability that the event is caused by a real planet rather than by noise. The resulting background distribution has no heavy tail, with about one false alarm per search at MES ∼ 7.8, and the detection efficiency improves for MES of 7.5–9 and more than four transits. The pipeline recovers most of the faint confirmed Kepler planets and, applied to the entire Kepler data set, finds ∼50 candidate events with a high probability of being real planets {% cite Ivashtenko2025pipeline %}.

I am currently working on formulating the catalog of these candidates. If you know how to quickly calculate astrophysical false positive probabilities for low-SNR transits with an algorithm that has a well-documented reliability and completeness, please get in touch with me.

After this, I will work on the occurrence rate inference derived from this search that will encompass all the signals detected by the pipeline, including the subthreshold ones, and their radius posteriors.
