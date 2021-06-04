---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Coordinated Resource Management for Cloud-based Specialized Operating Systems"
summary: ""
authors: [admin, Conghao Liu, Brian Tauro, Jack Lange, Jinpeng Zhou]
tags: [os, ds, virt, hpc]
categories: []
date: 2020-03-16T09:38:00-05:00

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

Containerization has recently gained significant interest among cloud providers
and users due to its ease of deployment and lightweight virtualization
capabilities. The key feature of these approaches is the sharing of a single
Linux OS instance among each active container environment. By sharing a single
OS environment containers are able to exhibit much greater resource efficiency
by avoiding the replicated state that arises in heavy-weight virtualization.
However, the container approach has the drawback of relying on a single general
purpose OS, whose design decisions might not align with those of the
application. A recent resurgence of Specialized Operating Systems and Runtimes
(SOS/Rs) has shown that significant performance and efficiency improvements can
be made by codesigning the OS and application runtime environment together. The
goal of this project is to enable the flexible deployment of these SOS/Rs
alongside current container based solutions. This work will allow application
services to be deployed on an optimal system software stack, and to react
dynamically to changing hardware resource availability.

Collaborative effort with the [Prognostic Lab](http://www.prognosticlab.org/) at The University of
Pittsburgh.


