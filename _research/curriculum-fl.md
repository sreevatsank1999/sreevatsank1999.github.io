---
title: "When Do Curricula Work in Federated Learning?"
group: earlier
order: 1
period: "2022"
image: /images/research/curriculum-fl.png
image_alt: "Illustration of training data split across two clients and an easy-first curriculum"
badges: ["ICCV 2023"]
team: "with Saeed Vahidian, Mubarak Shah, Bill Lin, and others"
links:
  - label: Paper
    url: https://openaccess.thecvf.com/content/ICCV2023/html/Vahidian_When_Do_Curricula_Work_in_Federated_Learning_ICCV_2023_paper.html
  - label: arXiv
    url: https://arxiv.org/abs/2212.12712
---
Curriculum learning orders training data from easy to hard. We studied it systematically in federated learning, where every client trains on its own skewed slice of the data. Ordered learning largely offsets the damage done by non-IID data, and the more the clients' distributions differ, the more they gain. We explain this with a convergence analysis that models curriculum training as local SGD with locally biased gradients. We also introduce a curriculum over clients, bringing them in from easy to hard, which compounds the gains.
