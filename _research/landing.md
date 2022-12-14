---
title: "Landing Site Selection and Divert Maneuver Planning with Deep Reinforcement Learning"
excerpt: "Applying reinforcement learning algorithms to design landing site selection policy and closed-loop controller for hazard detection and avoidance"
period: "2020/1 - Present"
image: 
  url: '/images/landing/landing_trajectory.png'
  width: '464'
  height: '428'
collection: project
---

<img src = "https://dl.dropboxusercontent.com/s/fnlga64x94mw7hh/landing_concept_972x493.png?dl=0">
<div style="text-align: center;">
<i>Figure 1. Concept of the Research</i>
</div>
<br>
Autonomous hazard detection and avoidance (HD&A) is of great importance in future planetary landing missions. This research proposes a new integrated framework for identifying safe landing sites and planning in-flight divert maneuvers. Conventional landing site selection algorithms rely on calculated local terrain features (e.g., slope and roughness) to find and prioritize candidate landing sites. However, they cannot select a target landing site that maximizes the expected probability of successful landing with explicit consideration of future divert maneuvers and observation. This study aims to optimize the landing site selection strategy concurrently with guidance and control policy by reinforcement learning to maximize the expected ratio of a successful landing by formulating the HD&A sequence as a Partially Observable Markov Decision Process (POMDP). 

The developed framework was applied to a 3-DOF lunar landing with a Lidar observation scenario. The (high) dimension of Lidar DEM data was reduced with the trained auto-encoder, while stability is guaranteed by utilizing the ZEM-ZEV feedback controller as a baseline control law. The target landing position and control gain of the ZEM-ZEV controller was adjusted by the reinforcement learning agent trained by both memory-based and memory-less algorithms. The investigation of the obtained result showed the capability of the agent to effectively adjust the control gain to achieve both long and short divert maneuvers. 

We are currently working on increasing the fidelity of the simulator using [Blensor](https://www.blensor.org/pages/documentation.html) and a more detailed comparison of the performance with non-RL methods. 

This research is a collaboration project with [Space Systems Optimization Group](https://ssog.ae.gatech.edu/) in Georgia Institute of Technology. 

<img src = "https://dl.dropboxusercontent.com/s/xlbuddt6b0iq3t5/landing_method_970x613.png?dl=0">
<div style="text-align: center;">
<i>Figure 2. Overall Framework</i>
</div>

---
Related Publications:
1. **Iiyama, K**, Tomita, K., Jagatia, B.A., Nakagawa, T., and Ho, K., ???Deep Reinforcement Learning for Safe Landing Site Selection with Concurrent Consideration of Divert Maneuvers???, 2020 AAS/AIAA Astrodynamics Specialist Conference, Lake Tahoe, CA, The United States, 2020 [[paper](/files/ASC_2020_iiyama.pdf)]
2. Tomita, K., Skinner, K., **Iiyama, K.**, Jagatia, B.A., Nakagawa, T., and Ho, K., ???Real-Time Terrain Mapping and Processing for Safe Landing via Deep Neural Networks???, ASCEND, Las Vegas, NV, The United States, 2020 [[paper](https://arc.aiaa.org/doi/abs/10.2514/6.2020-4150)]