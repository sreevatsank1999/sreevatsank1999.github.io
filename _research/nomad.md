---
title: "Nomad: Providing Insights into the Spectrum Environment"
group: spectrum
order: 1
period: "2022 – 2024"
image: /images/research/nomad.png
image_alt: "Nomad architecture: an API controller and FIFO buffer feed I/Q samples through shared memory to signal-detection and classifier containers that share a GPU, coordinated by a command-and-control database and an RF scheduler"
badges: ["IARPA-funded", "ACM MobiCom 2024"]
links:
  - label: Paper
    url: https://doi.org/10.1145/3636534.3698867
---
Nomad watches a wide swath of spectrum in real time and reports what it finds there. I architected its high-throughput pipeline, which ingests I/Q samples at a 40 Gbit/s line rate. Containerized microservices handle buffering, signal detection, and classification. They pass samples through zero-copy shared memory across C++, Python, and MATLAB components, share GPUs, and coordinate through a Redis-based command-and-control database alongside an RF scheduler.
