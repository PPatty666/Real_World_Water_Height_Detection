## Tide Monitoring, Water Level Detection, and Early Flood Warnings

# Key Findings

## 1. Object Detection for Flood Depth Estimation

We applied object detection models to estimate flood depth from water-level poles across diverse environmental conditions.

- Models trained under **dry conditions** transferred well to tranquil  sites.
- Transferability degraded under **extreme hurricane conditions**, particularly at coastal locations where images became heavily blurred due to intense precipitation, tides, and wind. In some cases, the water-level pole was barely distinguishable, even to the human eye.


---

## 2. Rapid Adaptation via Lightweight Active Learning

To address transfer failure under extreme conditions:

- Implemented a **lightweight active-learning pipeline** to identify missed or low-confidence detections.
- Rapidly labeled selected failure cases for incremental retraining.
- Balanced:
  - Model architecture complexity  
  - Retraining speed  
  - Real-time deployment constraints  

This approach enabled fast recovery of detection accuracy while maintaining operational feasibility during unfolding flood events.

---

## 3. Nighttime Performance Degradation Analysis

Unexpectedly, we observed performance degradation under **binary nighttime imagery**, where simpler visual structure might suggest easy transferability.

Systematic diagnosis identified two primary causes:

- **Camera–pole distance**: the physical distance between the camera and the water-level measurement pole.

- **Background interference** (reflections of background objects)

---

## 4. Deployment-Oriented Insight

Our goal is to:

> Capture the real-time evolution of flooding that would otherwise go unobserved.

Reasonable and robust depth estimation under extreme conditions provides actionable information for monitoring and decision-making, even in the presence of unavoidable measurement uncertainty.

---


# Contributors
Patty(Mengjue) Zhu (mzhu356@gatech.edu), Animesh Agrawal (anagrawal@gatech.edu)
Subhrajit Guhathakurta (subhro.guha@design.gatech.edu)
Barnali Dixon (bdixon@usf.edu)

