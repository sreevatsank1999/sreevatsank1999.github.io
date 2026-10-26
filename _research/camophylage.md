---
title: "CamoPHYlage: Hiding Signals in Plain Sight"
group: spectrum
order: 3
period: "2024 – 2026"
image: /images/research/camophylage.png
image_alt: "CamoPHYlage techniques. Alter: packet length extension, spectral sub-carriers, and modulation over modulation. Mimic: a desynchronized preamble."
figure: wide
---
Network security stops at the PHY layer: firewalls and intrusion detection inspect packets, but almost nothing watches the raw spectrum. A $100 software-defined radio can leak data even out of an air-gapped space, while wideband monitoring costs a defender a thousand times more. CamoPHYlage builds covert transmissions that PHY-layer detectors cannot flag, because their energy in time and frequency looks like ordinary traffic. *Alter* techniques hide data in a side channel of a legitimate signal by extending its packets, adding spectral sub-carriers, or modulating on top of its constellation. *Mimic* techniques synthesize a signal with a target's PHY signature that follows no protocol, so it cannot be decoded; we search for its waveform with Bayesian optimization and with neural networks that predict waveform parameters from spectrograms. Measured by Fréchet Inception Distance, both look far more like normal traffic than conventional low-probability-of-intercept signals do, trading covertness against range and throughput. Over the air, a battery-powered tiny SDR reached a receiver about 300 m away across campus, and a short DSSS sync sequence lets the receiver average through interference from overlapping Wi-Fi cells.
