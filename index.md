---
title       : Slidify
author      : Ramnath Vaidyanathan
framework   : minimal
highlighter : prettify
hitheme     : twitter-bootstrap
mode        : selfcontained
github      : {user: slidify, repo: workshops, branch: gh-pages}
---

# Slidify Workshops

<a href="http://prose.io/#{{site.github.user}}/{{site.github.repo}}/edit/gh-pages/index.Rmd" class="button icon edit">Edit Page</a>




This repository consists of material that I will use for workshops on Slidify.

## Installation

Slidify is not on CRAN and needs to be installed from `github` using the `devtools` package. I would recommend installing the `dev` version of the package.

```S
pkgs <- c("slidify", "slidifyLibraries", "rCharts")
devtools::install_github(pkgs, "ramnathv", ref = "dev")
```

While the installation process from `github` is relatively painless for Mac/Linux/Ubuntu users, it can make Windows users jump through hoops. For those of you on Windows that hit a bottleneck, here is an [excellent blog post](http://thiagosilva.wordpress.com/2013/02/17/installing-slidify-on-a-windows-machine/) that takes you through an alternate installation process that has been reported to work well.

If you are attending a Slidify workshop, and are having installation troubles, please post it as an [issue](http://github.com/slidify/workshop/issues/new). Make sure to outline the exact steps you undertook, and also paste the output of your `sessionInfo()` so that it would be easier for me to help you debug. 

__Given that installation can be time consuming (especially on Windows), I would strongly urge everyone attending the workshop to pre-install it beforehand.__

## Tutorials

1. [Introduction](tutorials/01)
2. [Frameworks](tutorials/02)
3. [Layouts](tutorials/03)


<style>ol.linenums {margin-left: -5px;}</style>
