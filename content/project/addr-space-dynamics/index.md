---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Address Space Dynamics"
summary: ""
authors: [Justin Goodman, Ganesh Mahesh, Brian Tauro, admin]
tags: [os, systems, modeling]
categories: []
date: 2020-03-16T11:23:06-05:00

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

In Physics, we can use the laws of motion, or the Lagrange equation, to
describe the trajectory of an object in a system. An object is described by
a state vector--a list of orthogonal dimensions.  We can think of a process 
as a trajectory through a state space. The dimensions are given
by the bits of memory, the registers, and the internal state of hardware. 
Thinking about processes this way allows us to formulate methods to understand
their execution externally. Obviously a program's execution is determined by its code,
but if this code is not available, we can use observations of its state
at discrete points in time and space to glean information about it, for example by
feeding a feature vector into an recurrent neural network to predict the next state.
We can also use this information to visualize a process over time (e.g. using
FFTs and dimensionality reduction techniques) or generate program fingerprints
for classification and computation of similarity metrics. 

We are currently using these techniques for low-latency malware classification.

