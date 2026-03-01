# Fetal Head Classification – Real-Time Implementation

This repository accompanies the **Ripples 2026** poster presentation at the **Indian Institute of Science (IISc)**, Bengaluru, submitted as part of ongoing PhD research in the **UTSAAH Lab**.

## Overview

The project demonstrates a deep-learning-based fetal head classification pipeline deployed in two real-time settings:

1. **Real-Time Implementation on an OEM Ultrasound Scanner**  
   Live inference of fetal head standard-plane classification directly on a commercial (OEM) ultrasound scanner, showcasing the feasibility of deploying the trained model in a clinical-grade hardware environment.

2. **Real-Time Implementation in 3D Slicer**  
   Live inference within [3D Slicer](https://www.slicer.org/), operating on a volumetric ultrasound dataset reconstructed using the **secure ultrasound system** developed in-house at the **UTSAAH Lab** (IISc). This demonstrates end-to-end volumetric acquisition, reconstruction, and AI-assisted classification in a research software environment.

## Demo Videos

| Demo | Description |
|------|-------------|
| `videos/oem_scanner_demo.mp4` | Real-time fetal head classification on OEM Ultrasound Scanner |
| `videos/slicer3d_demo.mp4` | Real-time classification in 3D Slicer on a reconstructed volume |

> **Note:** Video files will be added to the `videos/` directory once finalised for the poster presentation.

## Repository Structure

```
Fetal-head-classification/
├── videos/
│   ├── oem_scanner_demo.mp4      # OEM Ultrasound Scanner real-time demo
│   └── slicer3d_demo.mp4         # 3D Slicer real-time demo (UTSAAH Lab volume)
└── README.md
```

## About

- **Event:** Ripples 2026 – Annual Technical Symposium, IISc
- **Lab:** UTSAAH Lab, Indian Institute of Science, Bengaluru
- **Context:** PhD research on AI-assisted fetal ultrasound analysis