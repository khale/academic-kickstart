---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Low-Latency, In-Kernel AI"
summary: ""
authors: [admin, Brian Tauro, Eduardo Romero, Christopher Stewart]
tags: [os, ai, security, arch]
categories: []
date: 2020-03-16T09:39:04-05:00

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

Operating systems (OS) provide the interface for programs to access privileged
hardware and decide which programs can access system resources, when they can
access them and for how long. Within the OS kernel, these decisions are made
during scheduling, workload placement and mapping, resource
accounting and various kinds of application and VM introspection. 

Today, however, OS kernels leave several dynamic factors on the
table when making these decisions. For example, a simple fair-share scheduler
provides equal CPU access all threads, but does not prioritize threads that
safely access hardware and avoid out-of-bounds memory accesses. Malicious
programs can exploit this blind spot and steal information from co-resident
processes and the OS itself. We hypothesize that AI inference could (1)
label dynamic execution behaviors and (2) provide timely advice that could
fundamentally improve security and efficiency.  However, current AI inference
platforms are designed for user-space, i.e., they use high-level languages and
libraries that depend on drivers present in the OS. As a result, widely used
packages like PyTorch cannot be used within the OS kernel, because the it would
need a built-in Python runtime, library support, and an in-kernel CUDA
interface. Further, decisions that OSes make occur in a tight timing envelope,
e.g. within 10ms between scheduler ticks. This puts the requirements of OS
decision-making at odds with the capabilities of current ML techniques, which
are largely batch-oriented and involve costly transfers over an interconnect
fabric (PCI) to use GPUs or other accelerators.  

In this project we are (1) integrating low-latency AI capabilities into an OS kernel and (2)
applying that AI to create two novel kernel services. The first service will
efficiently and accurately fingerprint and identify applications using
non-traditional methods and the second involves tailoring OS-directed execution
contexts to user-provided code, a nascent scheduling problem enabled by
research done in the HExSA Lab on virtualization and OS techniques.
