---
title: Estimating Philippine Dealing System Treasury (PDST) reference rate yield curves using a state-space representation of the Nelson-Siegel model

event: The 2nd International Conference on Computing, Mathematics and Statistics 2015
# event_url: 

location: Langkawi Island, Malaysia
# address:
  # street: 450 Serra Mall
  # city: Stanford
  # region: CA
  # postcode: '94305'
  # country: United States

# summary: An example talk using Wowchemy's Markdown slides feature.
abstract: ""

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2015-11-04"
# date_end: "2030-06-01T15:00:00Z"
all_day: true

# Schedule page publish date (NOT talk date).
publishDate: "2015-11-04"

authors:
  - admin
  - Maria Eleanor R. Reserva

tags: []

# Is this a featured talk? (true/false)
featured: false

# image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/bzdhc5b3Bxs)'
  # focal_point: Right

# links:
# - icon: twitter
  # icon_pack: fab
  # name: Follow
  # url: https://twitter.com/georgecushen
# url_code: ""
# url_pdf: ""
# url_slides: ""
# url_video: ""

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
# projects:
# - PhD
---

Interest rate modelling serves a crucial role in the pricing of financial instruments and the management of risks in bond portfolios due to fluctuations in interest rates. A prominent approach in interest rate modelling is that of Nelson and Siegel, who use an exponential model to emulate typical shapes of the yield curve—monotonic, s-shaped, or humped. The Nelson-Siegel model for yield curves follow from a differential equation relating forward rates and prices of zero-coupon bonds and expressing the forward rate using a three-factor model with exponential decay components. Diebold and Li develop a dynamic latent factor model from the Nelson-Siegel yield curve, where four time-evolving parameters govern the shape of the yield curve—the level, the slope, the curvature, and the decay factors. Diebold, et al. reformulate the dynamic latent factor model into a state-space system, under the assumption that the level, slope, and curvature factors follow a vector autoregressive (VAR) process of order 1. This paper uses the dynamic latent factor approach to the Nelson-Siegel model for estimating yield curves for daily Philippine Dealing System Treasury (PDST) reference rates from March 2007 to April 2014. The goal of the paper is to see whether the time-varying Nelson-Siegel model is sufficient to fit yield curves on PDST reference rates by comparing out-of-sample data points on those forecasted by the model. In order to estimate the time series for the level, slope, and curvature and the parameters of the VAR(1) model for the latent factor, the MARSS (Multivariate Autoregressive State Space) package in R, developed by Holmes, et al. was used. The decay factor λ used, obtained via grid search, was that which maximizes the R2 in regressing PDST-F rates against the factor loadings in the Nelson-Siegel model. It is shown that the level, slope, and curvature latent factors are highly correlated with their respective empirical proxies and lag-1 values, while forecasted and actual yield data are sufficiently consistent, especially on shorter maturities. Yield curve estimates are also shown to follow the prevalent yield curve shapes posited by Nelson and Siegel.

{{< icon name="download" pack="fas" >}} Download the presentation slides {{< staticref "uploads/2015-iCMS.pdf" "newtab" >}}here{{< /staticref >}}.

