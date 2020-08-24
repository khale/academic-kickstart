---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Next-Generation Near-Data Processing Architectures"
summary: ""
authors: [admin, Rujia Wang, Xian-He Sun, Peng Jiang]
tags: [arch, os, ds, ai]
categories: []
date: 2020-03-16T11:56:38-05:00

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

In this work, we propose an integrated, full-stack System to enable
Memory-Centric Computing (SMC2). We target a system that has near-memory data
processors (NDP) as well as an extendable memory pool. We work on the entire
system stack to minimize the performance impact of memory accesses from the
research tasks in architecture, SW/HW interface, programming model/compiler,
and performance model/optimization. First, we propose to utilize the NDP
hardware to build an active memory system that supports intelligent data
prefetch and speculative data push, which can overlap the data access time with
computation. Next, we revisit current memory management mechanisms in order to
support NDP function calls, data push operations and virtualization. The new
SW/HW interface allows us to propose a new programming model, which can allow
the programmer to specify which tasks can run on the NDP resources, and allow
efficient NDP to NDP communication. Lastly, we try to optimize the system
performance with the help of NDP through a new memory-centric performance model
and a global performance optimization framework. Putting the four pieces
together, our proposed system support can maximize the performance of
memory-centric computing with new system abstractions and theories.
