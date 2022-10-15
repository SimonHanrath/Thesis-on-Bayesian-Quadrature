# Thesis-on-Bayesian-Quadrature
My Bachelors thesis on the re-weighting trick in Bayesian quadrature and the slides for the presentation.

Abstract:

A task that frequently occurs in machine learning is the computation of inte-
grals. These integrals are often intractable, and we must resort to approxima-
tion methods. One of these approximation methods is Bayesian quadrature.
It seeks to turn the problem of evaluating the integral into a Bayesian in-
ference task. We start with a prior over the integrand and make inferences
about it from a set of samples giving the posterior distribution over the in-
tegrand. A convenient way of putting priors over the integrand is through a
Gaussian process. For some kernel embeddings, the integral over the posterior
Gaussian process can be computed analytically. If we want to use Bayesian
quadrature for other kernel embeddings, an importance re-weighting trick be-
comes necessary. Similar to importance sampling, we rewrite the integral by
introducing a new probability density. However, the re-weighting trick has not
been explored in-depth, and it is unclear if re-weighting affects the performance
of Bayesian quadrature. In this thesis, we show that, depending on the new
probability density, re-weighting might severely affect the accuracy of Bayesian
quadrature. We propose ways of quantifying the expected performance drop
and design algorithms to choose parameters for the new probability density
in order to minimize the effect of re-weighting. Further, we conduct empirical
experiments that suggest that the proposed methods help reduce the potential
negative impact of re-weighting on Bayesian quadrature performance.
