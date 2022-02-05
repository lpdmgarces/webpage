---
title: Exchange Options under Stochastic Volatility and Jump-Diffusion Dynamics
summary: PhD Project at the University of South Australia. Commenced 23 July 2018, ended 18 October 2021.

authors:
  - admin

# tags:
# - Deep Learning
date: "2018-07-23"

# Optional external URL for project (replaces project detail page).
# external_link: ""

# image:
  # caption: Photo by rawpixel on Unsplash
  # focal_point: Smart

# links:
# - icon: twitter
  # icon_pack: fab
  # name: Follow
  # url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

This thesis addresses the problem of pricing European and American exchange options when the underlying asset price processes are modelled as stochastic volatility and jump-diffusion (SVJD) processes. While it is known that European exchange option prices can be computed exactly given the joint characteristic function for the underlying market variables, there has been little attention paid to American exchange options due to complications in characterizing the early exercise boundary, more so when using an SVJD model for asset prices. Furthermore, a numerical solution of the corresponding integro-partial differential equation (IPDE) is by no means trivial due to its multi-dimensional nature and the early exercise feature. Thus, this thesis characterizes exchange option prices when the underlying asset price model is a two-asset version of the Bates (1996) SVJD model. Furthermore, it extends existing work that have examined exchange options in the jump-diffusion framework and the stochastic volatility framework separately. 

We construct equivalent martingale measures with respect to our asset price model and derive the IPDEs and boundary conditions for the exchange option prices. We then derive probabilistic representations of the European exchange option price using two approaches: the change-of-numeraire technique and Fourier inversion formulas. We then derive an early exercise representation for the American exchange option price. From this representation, we find that the presence of jumps significantly impacts the early exercise option since American option holders stand to lose on their investment when asset prices suddenly jump in an undesirable direction, rendering the exercise suboptimal. This loss is referred to as the rebalancing costs due to jumps.

We also consider a proportional SVJD model for asset prices. The proportional SVJD model assumes that the two price processes share a single stochastic volatility process and, by construction, belongs to the class of affine jump-diffusions. This model specification allows us to directly solve the exchange option pricing IPDE and the corresponding Kolmogorov backward equation for the joint transition density function of the market variables using Fourier and Laplace transforms, thereby extending work on single-asset American options.

To further simplify the American exchange option pricing problem, we use the put-call transformation technique introduced by Bjerskund and Stensland (1993). This technique involves taking one of the assets as the numeraire, reducing the problem to an American call option on the ratio of the two assets. While this technique has been applied to the European case, its implementation to the American case under SVJD dynamics has yet to be seen. With this simplification, we also analyze the behavior of the early exercise boundary near maturity and discuss the substantial effect of jumps, consistent with the idea of rebalancing costs due to jumps.

Finally, we propose a method of lines (MOL) based approach to solve the option pricing IPDE. The MOL is considered efficient since it can accommodate the free-boundary case with minimal adjustments and is able to generate the option price, delta, and gamma in a single implementation. The MOL also performs faster and more accurately than comparable methods for American option pricing, namely the least squares Monte Carlo (LSMC) method and a projected successive overrelaxation (PSOR) solution of the linear complementary problem. With exchange option prices approximated using the MOL, we find that option prices and the early exercise boundary are significantly affected by the jump and stochastic volatility model parameters.

- **Principal Supervisor:** [Dr Gerald Cheang](https://people.unisa.edu.au/Gerald.Cheang)
- **Associate Supervisors:** [A/Prof John van der Hoek](https://people.unisa.edu.au/John.vanderHoek) and [A/Prof Anatoli Torokhti](https://people.unisa.edu.au/Anatoli.Torokhti))
- **Examiners:** [A/Prof Jonathan Ziveyi](https://www.unsw.edu.au/staff/jonathan-ziveyi) and [Prof Wolfgang Runggaldier](https://www.math.unipd.it/~runggal/)
- **Scholarship/Funding:** My PhD was generously supported by an Australian Government Research Training Program Scholarship (RPTi). I am also grateful for the the financial support provided by the Loyola Schools of Ateneo de Manila University.
