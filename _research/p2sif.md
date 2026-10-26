---
title: "P2SIF: Plug-n-Play Sensor Integration Framework"
group: physical-ai
order: 4
image: /images/research/p2sif.png
image_alt: "P2SIF architecture: specialist models for radar, camera, LiDAR, and GPS feed a knowledge-fusion stage and a generalist LLM"
team: "with Pushkal Mishra and Dinesh Bharadia"
links:
  - label: Proposal
    url: https://drive.google.com/file/d/1ftWI2YqR6nS3bKjvxw3UFfHv4UBvn5-R/view?usp=drive_link
---
General-purpose LLMs reason well but cannot read raw LiDAR or radar: when we asked frontier models about such data, they found cars in a scene that had none. Fine-tuning and adapter layers fix this only by tying each sensor to one model's weights. P2SIF keeps the two apart. Specialist models turn each sensor stream (camera, LiDAR, radar, GPS) into short text reports, a knowledge-fusion stage merges the reports, and an unmodified generalist LLM makes the decision. New sensors plug in without retraining, the LLM can be swapped for a better one, and every decision leaves a human-readable trail for attributing failures. We target autonomous-driving tasks in CARLA and on real LiDAR, radar, and camera data, including fog and night driving.
