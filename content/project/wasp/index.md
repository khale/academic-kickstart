---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/
title: "Wasp: Pushing Serverless Computing to the Limit"
summary: ""
authors: [Nicholas Wanninger, Josh Bowden, admin]
tags: [os, virt, pl, hpc]
categories: []
date: 2020-03-16T09:38:53-05:00

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
Current serverless and micro-service architectures rely on existing system
software to preserve compatibility and minimize development effort.
However, they also inherit the latencies and overheads that existing
systems carry with them. Existing serverless architectures resort to
process-level or language-based abstractions in order to achieve the
latencies that a real-time, micro-service oriented application requires.
While these abstractions offer certain levels of isolation, true
full-system isolation is sometimes required. 

Until now, achieving  full-system isolation necessitated the use of
heavy-weight virtual machines, raising the lower bound on response latencies.
In this project, we aim to demonstrate that the lower bound on latencies in
a fully virtualized environment is much lower than existing technology allows.
We leverage this opportunity to eschew traditional OS interfaces and
demonstrate a custom, microservice platform called Wasp.
