---
layout: page
title: Radius posteriors for low-SNR transiting planets
description: Marginalized planet-to-star radius ratio posteriors accounting for correlated noise, non-circular orbit, and stellar parameter priors, in hours instead of days.
importance: 2
related_publications: true
---

Occurrence rates of small long-period planets depend on the radii of transit candidates detected at low signal-to-noise ratio, and these radii should enter the population inference as full posteriors rather than point estimates. A proper posterior has to carry the uncertainty of all the latent parameters of the transit model and account for correlated noise in the light curve. A full Markov chain Monte Carlo fit with a Gaussian-process noise model does this, but takes too long and spends a lot of effort on nuisance parameters that are marginalized over anyway.

We developed a dimensionality-reduction method that computes the marginalized posterior of the planet-to-star radius ratio while sampling only a lower-dimensional effective parameter space. The 11-dimensional transit problem reduces to a 4-dimensional one, while the posterior still contains the uncertainty budget of the nuisance parameters, including eccentric orbits, stellar parameters, and limb darkening. The method operates on whitened light curves, which mitigates biases from correlated noise. We showed that the posterior distributions are calibrated: on simulated systems, the true radii have uniformly distributed p-values, and the posterior widths agree with a theoretical estimate. Applied to 419 faint long-period Kepler Objects of Interest, the radius ratios are broadly consistent with the KOI table, although the differences exceed what the reported uncertainties would predict {% cite Ivashtenko2026radius %}. The method is sketched in Fig. 1.

<div class="row justify-content-center">
    <div class="col-sm-12 mt-3 mb-2">
        {% include figure.liquid loading="eager" path="assets/img/projects/radii_method_scheme.png" class="img-fluid rounded z-depth-1" zoomable=true alt="Scheme of the dimensionality-reduction method" %}
    </div>
</div>
<div class="caption">
    Fig. 1. Method scheme. All the considered parameters, along with their priors, are shown on the left. We compress them into a 4-dimensional template bank, parametrized by limb-darkening coefficients, effective transit duration, and effective impact parameter. These are enough to cover the possible transit shapes, and the remaining information is stored in their priors. The transit epoch is treated using the convolution theorem, while the planet-to-star radius ratio distribution per template is obtained using model linearity. In the end, the per-template distributions are marginalized to obtain the final planet-to-star radius ratio posterior.
</div>
