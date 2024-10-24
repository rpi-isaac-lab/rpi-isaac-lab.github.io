---
layout: project
title: Autonomous Helicopter Aerial Refueling
researcher: Damsara Jayarathne
img: assets/img/heli_refuel_img.png
importance: 1
category: current
related_publications: true
---

![](/assets/img/heli_refuel_img.png)

My primary research focuses on developing a novel guidance, navigation, and control (GNC) architecture for autonomous helicopter aerial refueling. This complex maneuver involves guiding the helicopter's probe to dock with the drogue trailing behind a tanker aircraft, a task that demands significant pilot skill due to several challenges:

1. Aerodynamic interactions between the tanker, drogue, and helicopter,
2. Strict safety constraints,
3. Limited time available to complete the docking process.

To address these challenges, my work proposes an autonomous control methodology capable of handling the uncertainties in drogue dynamics and aerodynamic interactions while ensuring safety and stability. The control architecture integrates a dynamic inversion-based model-based controller with a reinforcement learning controller. Preliminary results indicate that this hybrid approach improves performance by 24% compared to using a model-based controller alone when deployed on a high fidelity UH60 Black Hawk helicopter.

![](/assets/img/heli_refuel_logic.png)

![](/assets/img/heli_refuel_diagram.png)

Aspects of this work have been presented in the following papers: {% cite jayarathne_allocation_2024 %}, {% cite jayarathne_safe_2023 %}.
