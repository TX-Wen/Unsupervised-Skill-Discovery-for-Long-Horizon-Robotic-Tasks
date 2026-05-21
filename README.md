# 🚀 Unsupervised Skill Discovery for Long-Horizon Robotic Tasks

[![Status](https://img.shields.io/badge/Status-Under_Review-orange.svg)]()
[![Paper](https://img.shields.io/badge/Paper-Coming_Soon-blue.svg)]()

> **Note:** The full methodology, rigorous mathematical proofs, and quantitative evaluations are currently under review for IEEE TRO / CoRL. The complete codebase and pre-trained weights will be released upon acceptance.

This repository provides a preliminary showcase of a data-driven framework designed to autonomously segment and extract skill primitives from long-horizon robotic demonstrations, strictly under **unsupervised conditions**. 

By evaluating datasets and mapping demonstrations without manual annotations, this framework extracts actionable skill primitives that can be seamlessly integrated into Vision-Language-Action (VLA) architectures for advanced logical reasoning and real-world deployment.

## ✨ Core Capabilities

* **Data-Driven Temporal Segmentation:** Automatically slices continuous, long-horizon expert trajectories into semantically meaningful sub-task nodes without requiring predefined heuristics.
* **Non-parametric Modality Recognition:** Effectively filters local drift noise and identifies divergent behavior modalities (e.g., distinct topological paths or grasping poses) for the same underlying sub-task.
* **Plug-and-Play VLA Integration:** The discovered autonomous skill nodes are designed to serve as high-level decision foundations for subsequent end-to-end policy execution.

---

## 📊 Visual Results

Our framework has been successfully evaluated across diverse simulation environments, spanning 2D state spaces to complex visuo-motor manipulation tasks.

### 1. 2D Navigation: Trajectory Modality Segmentation
The framework maps raw demonstrations onto progress-value dimensions, achieving a **33.9% increase in classification accuracy** for 2D navigation tasks. 

<div align="center">
  <img src="assets/2d_nav_comparison.png" width="800" alt="2D Navigation Comparison">
  <p><i>Left: Raw unclassified trajectories. Right: Unsupervised extraction of distinct navigation modalities.</i></p>
</div>

### 2. PushT: Continuous Sub-task Discovery
In continuous visuo-motor control tasks like PushT, the framework continuously evaluates state connectivity. Different colors in the trajectory indicate automatically segmented skill nodes transitioning in real-time.

<div align="center">
  <img src="assets/pusht_segmentation.gif" width="600" alt="PushT Temporal Segmentation">
</div>

### 3. LIBERO: Multimodal Behavior Recognition
For identical manipulation objectives in the LIBERO suite, our approach robustly clusters trajectories into distinct skill-affinity matrices, recognizing different operational modes for the same task.

<div align="center">
  <img src="assets/libero_multimodal.gif" width="800" alt="LIBERO Multimodal Execution">
</div>

---

## 👨‍💻 Author

**Tongxin Wen**
* M.Eng. in Mechanical Engineering, Harbin Institute of Technology (HIT)
* Affiliated with the State Key Laboratory of Robotics and System (SKL)
* [Homepage: TX-Wen.github.io](https://TX-Wen.github.io) 
* Contact: wen78675847@gmail.com

For academic inquiries or potential collaborations, please feel free to reach out via email.
