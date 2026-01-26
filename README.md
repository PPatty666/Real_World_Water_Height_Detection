## Tide Monitoring, Water Level Detection, and Early Flood Warnings

In this project, we apply object detection techniques to identify poles and estimate their above-water (above-flood) height for flood monitoring during hurricanes. We collected time-lapse images every 15 minutes during Hurricane Helene, Hurricane Milton, and all dry periods, as the cameras operate continuously.

We investigate different training protocols, including labeling strategies and training image time frames, to assess model accuracy over time and generalizability across cameras. We are also exploring an active learning framework, in which the model is periodically retrained to mitigate performance degradation. Our experiments show that models trained before Hurricane Helene experienced reduced accuracy when evaluated on Hurricane Milton, highlighting the importance of continual model updates.

# Contributors
Patty(Mengjue) Zhu (mzhu356@gatech.edu), Animesh Agrawal (anagrawal@gatech.edu)
Subhrajit Guhathakurta (subhro.guha@design.gatech.edu)
Barnali Dixon (bdixon@usf.edu)

