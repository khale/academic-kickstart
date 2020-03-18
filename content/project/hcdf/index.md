---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Hybrid Runtimes for Compiled Dataflows"
summary: ""
authors: [admin, Qitian Zeng, Boris Glavic]
tags: [os, systems, db]
categories: []
date: 2020-03-16T09:37:29-05:00

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

We observe that the OS and database communities face a similar challenge: how
do we optimize systems to exploit the characteristics of specialized hardware
without sacrificing the flexibility of general-purpose designs? Both
communities have independently made progress on developing high-performance
systems that exploit modern hardware and that --- to a lesser degree --- retain
flexibility.  However, there is scant work that consolidates the efforts from
these two core systems communities in the context of the advances mentioned
above.  We argue that this is an important oversight since a general-purpose OS
can *get in the way* of a high-performance data processing platform
resulting in an unnecessary reduction in performance. The mismatch between
abstractions and interfaces provided by the OS and the intent of the programmer
might also require that the application programmer employ workarounds,
essentially gaming the OS. These can be time-intensive, error-prone, and
detrimental to the clarity, elegance, and longevity of application code.  The
goal of this research is to integrate specialization techniques from the OS
community (hybrid runtimes, hybrid virtual machines, and advanced
virtualization techniques) and DB community (compiled queries and hardware-conscious query execution techniques) for
high-performance query processing on modern hardware.  *Specifically, we
propose to  develop a high-performance data processing platform called
HCDF that runs atop a hybrid of a compilation-based data-flow engine and
a lightweight, specialized OS which is optimized for data processing*. Our
approach will leverage ideas from extant work on specialized operating
systems and data processing techniques that exploit modern hardware.

In collaboration with [Boris Glavic](http://www.cs.iit.edu/~dbgroup/members/bglavic.html) and the DBGroup at IIT.
