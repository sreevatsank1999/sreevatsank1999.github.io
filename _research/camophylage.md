---
title: "CamoPHYlage: Hiding Signals in Plain Sight"
group: spectrum
order: 2
period: "2024 – 2026"
teaser: "Adversarial mimicking techniques that evade PHY-layer detectors and enable covert communication in plain sight."
image: /images/research/camophylage.png
image_alt: "CamoPHYlage techniques. Alter: packet length extension, spectral sub-carriers, and modulation over modulation. Mimic: a desynchronized preamble."
---
Security monitoring rarely extends to the physical layer. CamoPHYlage studies covert transmissions whose energy distribution in time and frequency resembles ordinary traffic. *Alter* techniques hide data in a side channel of a legitimate signal through packet length extension, spectral sub-carriers, or modulation over modulation. *Mimic* techniques synthesize a non-protocol-compliant signal with a target's PHY signature, found through Bayesian optimization and neural parameter estimation from spectrograms. Measured by Fréchet Inception Distance, both are far closer to normal traffic than conventional low-probability-of-intercept signals, and a battery-powered SDR prototype reached a receiver approximately 300 m away.
