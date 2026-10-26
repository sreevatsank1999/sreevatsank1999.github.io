---
title: "PHYNet: A Gold-Standard Labelled PHY-Layer Dataset"
group: spectrum
order: 2
period: "2024 – 2026"
image: /images/research/phynet.jpg
image_alt: "The same over-the-air capture labelled two ways: PHYNet's ground truth marks each transmission, while an energy detector merges some bursts and fragments others"
figure: wide
---
PHY-layer detectors and classifiers are hard to compare because there is no large, accurately labelled dataset of real over-the-air signals; most real-world datasets serve RF fingerprinting for a single protocol. PHYNet builds one, labelling every transmission in a capture from the decodes of hardware sniffers for Wi-Fi, BLE, Zigbee, LoRa, and 5G, alongside GNU Radio transmitters. The hard part is time. Sniffer timestamps jitter by milliseconds, so we anchor them to hardware fine-time counters and correct clock drift, which brings labels to within about 2 µs of the IQ samples. A successive decoding and cancellation pipeline replays a capture over a cable into a sniffer, labels and removes the packets it decodes, and replays the remainder at higher gain to recover weaker transmissions, at 40 s per iteration instead of 10 minutes. With these labels we can score energy detection, modulation recognition, RF fingerprinting, and source identification, and the scores show how little today's spectrum-awareness tools know about the signals around them.
