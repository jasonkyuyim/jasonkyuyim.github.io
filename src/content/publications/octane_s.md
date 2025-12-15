---
title: 'Octane-S'
---

My first project at DeepMind and first time on a large scale deep learning project. I was the sole research engineer responsible for data, training, evaluation, and collaborating with human doctors. We trained a large 3D U-Net (large at the time) on gigapixel medical volumetric scans to predict if the patient would develop eye disease in the next 6 months. We tried lots of modeling ideas that attempted to incorporate time series of how the 3D scans changed over time (hence modeling 4D data). But the rregular time intervals between scans and small number of scans per patient led to the 4D model not outperforming the 3D U-net. Real world data, especially medical data, is notoriously messy. Data ingestion and cleaning took a significant amount of time. We worked with optometrists to relabel the data and ran a prospective study of comparing the model's performance against 6 optometrists out of which the model performed better than 5. 
