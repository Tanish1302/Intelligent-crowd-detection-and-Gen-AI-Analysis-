# 🧠 Intelligent Crowd Detection and Analysis System
### Computer Vision & Generative AI

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red.svg)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-OpenCV-green.svg)
![GPU](https://img.shields.io/badge/GPU-NVIDIA%20Tesla%20T4-lightgrey.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

---

## 📌 Overview

An **AI-powered crowd detection, tracking, and analysis system** that leverages **Computer Vision**, **Multi-Object Tracking**, **Clustering**, and **Generative AI** to automatically analyze surveillance video feeds and generate actionable insights for **security, event management, and crowd safety**.

---

## 🎯 Problem Statement

Manual monitoring of surveillance footage is inefficient and error-prone due to:
- Occlusions and overlapping individuals  
- Dynamic lighting conditions  
- High crowd density  

This project provides a **fully automated, real-time crowd analytics pipeline** to address these challenges.

---

## 🚀 Key Features

- Robust **person detection** using Faster R-CNN  
- **Hybrid multi-person tracking** with Kalman Filters  
- Dynamic **crowd clustering** using DBSCAN  
- **Generative AI-based frame understanding**  
- Automated **HTML reports, CSV, JSON exports, and annotated videos**

---

## 🏗️ System Architecture

Video Input

↓

Person Detection (Faster R-CNN)

↓

Hybrid Tracking (Kalman + IoU + Appearance)

↓

Crowd Clustering (DBSCAN)

↓

GenAI Frame Analysis (BLIP)

↓

Reports & Visual Outputs


---

## 🧠 Core Modules

### 1️⃣ Person Detection Module
- **Model:** Faster R-CNN (ResNet50 FPN v2)
- Two-tier confidence thresholding
- Non-Maximum Suppression (IoU = 0.45)
- CUDA-enabled GPU inference

---

### 2️⃣ Hybrid Tracking Module
- Kalman Filter–based motion prediction
- Two-stage matching:
  - IoU + appearance matching
  - IoU-only fallback for occlusions
- Maintains identity consistency across frames

---

### 3️⃣ Crowd Clustering Module
- **Algorithm:** DBSCAN (GPU-accelerated via cuML)
- Adaptive clustering radius based on person height
- Minimum 3 people required to form a crowd

---

### 4️⃣ Generative AI Frame Analysis
- **Model:** BLIP Image Captioning
- Identifies high-activity frames
- Produces natural-language scene descriptions

---

### 5️⃣ Report Generation
Automatically generates:
- 📄 Interactive HTML report  
- 📊 CSV crowd statistics  
- 🎥 Annotated output video  
- 🧾 JSON structured data  

---

## 📊 Results & Performance

| Metric | Value |
|------|------|
| Frames Analyzed | 274+ |
| Video Duration | ~12 seconds |
| Average Crowd Size | 17.5 |
| Peak Crowd Size | 33 |
| Significant Events | 24 |
| Unique Person Tracks | 1000+ |
| Crowd Clusters | 50+ |

---

## ⏱️ Crowd Timeline Summary

| Time Range (s) | Activity |
|--------------|---------|
| 0–1 | Initial formation |
| 1–3 | Crowd diversification |
| 3–5 | Peak activity |
| 5–8 | Moderate consolidation |
| 8–12 | Dispersal phase |

---

## 🖼️ Sample Outputs

### Crowd Detection & Clustering
<img width="900" height="507" alt="image" src="https://github.com/user-attachments/assets/3295974d-9989-46cf-9c2e-01b03aa13842" />

### Interactive HTML Report
<img width="900" height="503" alt="image" src="https://github.com/user-attachments/assets/d92035f2-69c1-4a06-8c94-588475ebb447" />
<img width="944" height="540" alt="image" src="https://github.com/user-attachments/assets/d150a834-d851-4138-9eaa-8e8725395e85" />




### CSV Data Output
<img width="935" height="564" alt="image" src="https://github.com/user-attachments/assets/9e03d149-6c51-4a1f-a372-5128d8992635" />


---

## ⚙️ Tech Stack

### Computer Vision & AI
- OpenCV  
- PyTorch & Torchvision  
- Faster R-CNN  
- Kalman Filter  
- DBSCAN (cuML)

### Generative AI
- Hugging Face Transformers  
- BLIP Image Captioning  
- BART Model  

### Data & Optimization
- NumPy, Pandas  
- SciPy (Linear Assignment)  
- CuPy (GPU acceleration)

---

## 🖥️ Hardware Configuration

- **GPU:** NVIDIA Tesla T4 (15 GB VRAM)
- **CUDA:** 12.4
- **Latency:** < 40 ms per frame
- **Processing Speed:** 25+ FPS
- **Full Analysis Time:** < 5 minutes (12s video)

---

## 📂 Output Files

├── ai_enhanced_crowd_data.csv

├── ai_crowd_analysis_report.html

├── annotated_output_video.mp4

├── analysis_data.json


---

## 🏁 Conclusion

This project demonstrates a **production-grade AI pipeline** capable of detecting, tracking, clustering, and analyzing crowds in real time. The integration of **Generative AI** enhances situational awareness, making the system suitable for **real-world deployments** in surveillance, public safety, and event monitoring.

---

## 👥 Team Members

- **Tanish Punamiya**
- **Shobhit Shah**
- **Atharva Pande** 

---
