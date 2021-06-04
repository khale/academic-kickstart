---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Exploring Julia at the Large Scale"
summary: ""
authors: [Amal Rizvi, admin]
tags: [systems, pl, hpc, ds]
categories: []
date: 2020-03-16T09:38:47-05:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

Practitioners of high-performance parallel computing have long sought better
programming models and languages to ease the task of writing programs for
large-scale systems. However, there is an undeniable tension that exists
between extreme performance and developer friendliness. While the steadily
increasing performance of high-level languages shows promise, and the
ubiquity of concurrent programming is on the rise, these advancements have not
yet made a significant impact in the HPC community. The [Julia language](https://julialang.org) is of
particular interest as it boasts single-threaded performance on par with C and
Fortran while retaining familiar echoes of MATLAB, Python, and Ruby-like syntax
in the language. In this project, we are experimenting with Julia's ability to 
scale to large machines using benchmarks such as [HPCG](https://www.hpcg-benchmark.org/) and custom microbenchmarking. We are
also exploring ways to enhance Julia with the [Hybrid Runtime Model]({{< ref "/publication/hale-2015-nautilus" >}}).
