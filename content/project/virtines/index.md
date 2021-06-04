---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/
title: "Virtines: Isolated Execution at Function Call Granularity"
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

We are exploring the limits of hardware virtualization by running
individual *functions* in lightweight, virtualized execution environments
called *virtines*. Programmers create virtines by annotating existing functions
in C or Rust, and our runtime system (Wasp) manages virtual machines automatically. 

