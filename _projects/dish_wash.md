---
layout: project
title: Behavioral learning of dish rinsing and scrubbing based on interruptive direct teaching considering assistance rate
journal: Advanced Robotics
authors:
  - name: Shumpei Wakabayashi 
    url: "https://shmpwk.github.io"
    is_self: true
  - name: Kento Kawaharazuka
    url: "https://haraduka.github.io/"
  - name: Kei Okada
  - name: Masayuki Inaba
affiliation: JSK Robotics Laboratory, The University of Tokyo, Japan
paper_url: "https://www.tandfonline.com/doi/abs/10.1080/01691864.2024.2379393" 
arxiv_url: "https://arxiv.org/abs/2408.09360"
video_url: "https://youtu.be/db4OcVsz3YY?si=n_huevCWTMdhP1Ry"
---

Robots are expected to manipulate objects in a safe and dexterous way. For example, washing dishes is a dexterous operation that involves scrubbing the dishes with a sponge and rinsing them with water. It is necessary to learn it safely without splashing water and without dropping the dishes. In this study, we propose a safe and dexterous manipulation system. The robot learns a dynamics model of the object by estimating the state of the object and the robot itself, the control input, and the amount of human assistance required (assistance rate) after the human corrects the initial trajectory of the robot’s hands by interruptive direct teaching. By backpropagating the error between the estimated and the reference value using the acquired dynamics model, the robot can generate a control input that approaches the reference value, for example, so that human assistance is not required and the dish does not move excessively. This allows for adaptive rinsing and scrubbing of dishes with unknown shapes and properties. As a result, it is possible to generate safe actions that require less human assistance.

## Autoregressive Model Learning with Interruptive Human Assistance and Manipulation Modification during Optimization

To achieve safe and dexterous operation, we propose an autoregressive dynamics model including interruptive human assistance and an optimization that modifies the control input so that human assistance is less necessary.

<div class="train">
  <img src="{{ site.baseurl }}/assets/images/training.svg" alt="Experiment result" style="transform: scale(1.2);">
</div>

<div class="inference">
  <img src="{{ site.baseurl }}/assets/images/inference.svg" alt="Experiment result" style="transform: scale(1.2);">
</div>

## Path Planning for Autoregressive Model Validation

In order to confirm the usefulness of the optimization using the autoregressive model, we conducted a preliminary experiment in path planning to avoid dynamic obstacles.

<div class="path-planning">
  <img src="{{ site.baseurl }}/assets/videos/pathplan.gif" alt="Experiment result" style="transform: scale(1.2);">
</div>

## Dish Washing Experiment

<div class="experiment-section">
  <img src="{{ site.baseurl }}/assets/videos/dish_training.gif" alt="Experiment result" style="transform: scale(1.2);">
</div>

<div class="opt-section">
  <img src="{{ site.baseurl }}/assets/videos/dish_opt.gif" alt="Experiment result" style="transform: scale(1.2);">
</div>


## Bibtex

```bibtex
@article{doi:10.1080/01691864.2024.2379393,
  author = {Shumpei Wakabayashi, Kento Kawaharazuka, Kei Okada and Masayuki Inaba},
  title = {Behavioral learning of dish rinsing and scrubbing based on interruptive direct teaching considering assistance rate},
  journal = {Advanced Robotics},
  volume = {38},
  number = {15},
  pages = {1052--1065},
  year = {2024},
  publisher = {Taylor \& Francis},
  doi = {10.1080/01691864.2024.2379393},
}
```

## Contact

If you have any questions, please feel free to contact Shumpei Wakabayashi (email: wakabayashi(at)jsk.imi.i.u-tokyo.ac.jp)
