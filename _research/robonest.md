---
title: "RoboNEST: Robotics Networked Edge Systems Testbed for Physical AI"
group: physical-ai
order: 1
period: "2025 – present"
image: /images/research/robonest.jpg
image_alt: "RoboNEST testbed: robot arms and a TurtleBot, Ethernet, Wi-Fi and private 5G access networks, and edge GPU compute"
figure: wide
badges: ["Demo · ACM MobiCom 2026"]
team: "with Ushasi Ghosh and Dinesh Bharadia"
links:
  - label: Paper
    url: https://doi.org/10.1145/3795866.3848480
  - label: Project Page
    url: https://edgeric.github.io/projects/robonest.html
---
RoboNEST brings real robots, interchangeable wireless networks, and edge GPUs into one instrumented testbed, so the full sensing-to-action path of a Physical AI task can be measured and controlled end to end. Two xArm7 arms, SO-101 leader-follower arms, and a TurtleBot stream camera, LiDAR, depth, and IMU data to the edge over Ethernet, Wi-Fi 6, or a private 5G network running [EdgeRIC](https://wcsng.ucsd.edu/edgeric/). There, vision-language-action (VLA) policies run on GPUs ranging from A10s to an RTX 6000 and a GB10. Clock-synchronized logging ties every application event to RAN state, modem diagnostics, and GPU inference. On a 1080p manipulation task over 5G, moving the policy from an A10 to an RTX 6000 cuts glass-to-action latency from 179 ms to 111 ms; on the same GPU, Wi-Fi and Ethernet come in at 77 ms and 68 ms.
