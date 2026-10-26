---
title: "mmsRAN: Multimodal Cellular Uplink for Physical AI"
group: physical-ai
order: 2
period: "2025 – present"
image: /images/research/mmsran.png
image_alt: "mmsRAN scheduling loop: the edge application shares future sensing decisions and an EdgeRIC app schedules each user's sensor streams per RAN slot"
figure: wide
badges: ["Qualcomm Innovation Fellowship 2026", "WiP · ACM MobiCom 2026"]
team: "with Ushasi Ghosh, Srinivas Shakkottai, and Dinesh Bharadia"
links:
  - label: Paper
    url: https://doi.org/10.1145/3795866.3844782
  - label: Project Page
    url: https://edgeric.ucsd.edu/projects/multimodal-sensing.html
---
A robot's control loop runs in timesteps, and the edge can act only once every sensor stream for a timestep has arrived. Over the cellular uplink those streams arrive skewed, both across one robot's sensors and across robots sharing a cell; in our multi-user measurements the skew alone adds about 13 ms. mmsRAN makes the RAN aware of multimodal flows. Each sensor modality gets its own QoS flow and data radio bearer, and a scheduler running on [EdgeRIC](https://edgeric.ucsd.edu/) allocates uplink resources slot by slot so that a timestep's streams arrive together. In early over-the-air results on our 5G testbed, tuning the network cut median sensor-frame latency from 30.4 ms to 18.9 ms. Bearer-level prioritization then roughly halved the latency of a high-priority stream without starving the others.
