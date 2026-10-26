---
title: "SpecSense: Learning-Based Wideband Spectrum Sensing"
group: spectrum
order: 5
period: "Summer 2022 · JASR Systems"
image: /images/research/specsense.jpg
image_alt: "Signals in the wild: sparse occupancy across the sub-6 GHz band, and periodic, bursty, always-on, and frequency-hopping signals"
team: "with Raghav Subbaraman"
links:
  - label: Poster
    url: https://drive.google.com/file/d/16-F9lr1lG-SX6eIBbNx_kEmRo0NkkKR_/view?usp=sharing
---
Watching 6 GHz of spectrum continuously would take a prohibitive number of radios. Real spectrum use is sparse and structured, though: signals are periodic, bursty, always on, or frequency hopping. During my internship at JASR Systems I built an online-learning approach for blind detection and tracking of low-probability-of-intercept signals. It learns each signal's arrival process from heavily undersampled observations, with only 1–5% real-time coverage, and uses that model to point a few radios where signals will appear. Cooperative scheduling across receivers, adaptive combining for non-stationary signals, and maximum-likelihood attribution of arrival times improved prediction over the state of the art.
