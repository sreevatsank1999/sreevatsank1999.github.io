---
title: "Nomad: Providing Insights into the Spectrum Environment"
group: spectrum
order: 4
period: "2022 – 2024"
teaser: "A high-throughput spectrum sensing system with a line rate of 40 Gbit/s."
image: /images/research/nomad.png
image_alt: "Nomad architecture: an API controller and FIFO buffer feed I/Q samples through shared memory to signal-detection and classifier containers that share a GPU, coordinated by a command-and-control database and an RF scheduler"
badges: ["IARPA-funded", "ACM MobiCom 2024"]
links:
  - label: Paper
    url: https://doi.org/10.1145/3636534.3698867
  - label: Project Page
    url: https://wcsng.ucsd.edu/signals-lab/project/nomad/
---
I architected the system's high-throughput pipeline. Containerized microservices handle buffering, signal detection, and classification, exchanging samples through a copy-efficient shared-memory interface and coordinating through a Redis-based in-memory database.
