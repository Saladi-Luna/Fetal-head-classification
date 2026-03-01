# Fetal Head Classification - Real-Time Implementation

This repository accompanies the **Ripples 2026** poster presentation at the **Indian Institute of Science (IISc)**, Bengaluru, submitted as part of ongoing PhD research in the **UTSAAH Lab**.

## Overview

The project demonstrates a 2 stage deep-learning-based fetal head classification pipeline deployed in two real-time settings:

1. **Real-Time Implementation on an OEM Ultrasound Scanner**  
   The trained classification models were deployed for live inference using a commercial (OEM) ultrasound scanner. Image frames were captured via a frame grabber and processed on a secondary laptop in real time.

This setup demonstrates the practical feasibility of integrating the model with clinical-grade imaging hardware, validating its potential for real-world clinical deployment.

2. **Real-Time Implementation in 3D Slicer**  
   Live inference within [3D Slicer](https://www.slicer.org/), operating on a volumetric ultrasound dataset acquired using the **Secure Ultrasound system** at the **UTSAAH Lab** (IISc). This demonstrates end-to-end volumetric  AI-assisted classification in a research software environment.

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
│   ├── real time video - 1.mp4      # OEM Ultrasound Scanner real-time demo
│   └── slicer video.mp4         # 3D Slicer real-time demo (UTSAAH Lab volume)
└── README.md
```

## About

- **Event:** Ripples 2026 – Annual Technical Symposium, IISc
- **Lab:** UTSAAH Lab, Indian Institute of Science, Bengaluru
- **Context:** PhD research on AI-assisted fetal ultrasound analysis
