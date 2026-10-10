---
layout: page
title: fBLS, a fast-folding transit search
description: A fast-folding BLS algorithm designed for ultra-short-period planets whose parameter space is too large to search in the classical way.
importance: 4
related_publications: true
---

fBLS is a fast-folding technique for transit searches, built on the fast-folding algorithm, a dynamic-programming method that is widely used in pulsar astronomy. For a light curve with N points, it produces the binned phase-folded light curves for an array of N<sub>p</sub> trial periods, and then computes the standard BLS periodogram and statistics for each. The cost is O(N<sub>p</sub> log N<sub>p</sub>) operations instead of the O(N<sub>p</sub> N) of a regular BLS, which matters most for planets with periods shorter than a day, where the period grid is dense.

A preliminary fBLS search for ultra-short-period planets in the Kepler main-sequence light curves, followed by a simple signal-validation scheme, recovered all known ultra-short-period candidates and found three new ones {% cite Shahaf2022fBLS %}. This work, led by Sahar Shahaf with Barak Zackay, Tsevi Mazeh, and Simchon Faigler, dates from my M.Sc. years at Weizmann.
