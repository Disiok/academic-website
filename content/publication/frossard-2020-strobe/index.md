---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'StrObe: Streaming Object Detection from LiDAR Packets'
subtitle: ''
summary: ''
authors:
- Davi Frossard
- "**Simon Suo**"
- Sergio Casas
- James Tu
- Rui Hu
- Raquel Urtasun
tags: []
categories: []
date: '2020-11-12'
lastmod: 2020-11-12T23:05:07-05:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2020-11-13T04:05:07.011529Z'
publication_types:
- '0'
abstract: 'Many modern robotics systems employ LiDAR as their main sensing
modality due to its geometrical richness. Rolling shutter LiDARs are particularly
common, in which an array of lasers scans the scene from a rotating base. Points
are emitted as a stream of packets, each covering a sector of the 360° coverage.
Modern perception algorithms wait for the full sweep to be built before processing
the data, which introduces an additional latency. For typical 10Hz LiDARs this
will be 100ms. As a consequence, by the time an output is produced, it no longer
accurately reflects the state of the world. This poses a challenge, as robotics
applications require minimal reaction times, such that maneuvers can be quickly
planned in the event of a safety-critical situation. In this paper we propose StrObe,
a novel approach that minimizes latency by ingesting LiDAR packets and emitting
a stream of detections without waiting for the full sweep to be built. StrObe
reuses computations from previous packets and iteratively updates a latent spatial
representation of the scene, which acts as a memory, as new evidence comes in,
resulting in accurate low-latency perception. We demonstrate the effectiveness
of our approach on a large scale real-world dataset, showing that StrObe far
outperforms the state-of-the-art when latency is taken into account, and matches
the performance in the traditional setting.'
publication: ''
publication_short: "CoRL 2020 (<font color='red'>**Spotlight**</font>)"
url_pdf: 'https://arxiv.org/pdf/2011.06425.pdf'
url_video_long: 'https://youtu.be/Gy97AnWdGn8'
---
