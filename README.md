<h1 align="center">Jishan Shaikh</h1>
<p align="center">
  M.S. Computer Science (AI) @ University of Southern California · Los Angeles, CA<br/>
  Parameter-efficient fine-tuning · Vision Transformers · Computer Vision · NLP
</p>
<p align="center">
  <a href="mailto:jishanshaikh1004@gmail.com">Email</a> ·
  <a href="LINKEDIN_URL">LinkedIn</a> ·
  <a href="GOOGLE_SCHOLAR_URL">Google Scholar</a> ·
  <a href="RESUME_PDF_URL">Resume</a>
</p>

---

## About

I'm an M.S. student at USC (Artificial Intelligence, Spring 2026 – present) with three published or accepted papers in computer vision and NLP, and an ongoing independent research project on **adaptive LoRA rank allocation for Vision Transformers**. I like experiment-driven work: baselines, ablations, error analysis and reproducible pipelines.

**Currently:** developing Curvature-Guided Rank Selection (CGRS) on USC CARC (V100/A100, Slurm).
**Looking for:** ML / Applied Science / Research internships in efficient fine-tuning, computer vision and NLP.

---

## Current Research

### Curvature-Guided Rank Selection (CGRS) for LoRA on ViTs
*Independent research, USC · Spring 2026 – present · Paper in preparation*

Instead of one fixed LoRA rank everywhere, CGRS uses the **diagonal Fisher Information (λmax)** of each transformer layer to allocate rank per layer of ViT-Base/16.

| Dataset | Result |
|---|---|
| CIFAR-100 | **90.61%** with **1.92M** trainable parameters (best variant 90.85%), beating fixed-rank LoRA (r=64) with fewer parameters |
| CIFAR-10 | **98.78%** vs. 98.81% for full fine-tuning (within 0.03 points), after fixing a threshold-calibration anomaly with a fractional-threshold policy |

- Four-phase pipeline: fixed-rank baselines → curvature profiling → global CGRS → per-layer CGRS
- Also tested on SVHN and Flowers102, with an AdaLoRA comparison in the repo
- 🔗 [Code](https://github.com/jish2003/Curvature-Guided-Rank-Selection-for-LoRA-Fine-Tuning-of-Vision-Transformers)

---

## Publications

| Year | Paper | Venue | Notes |
|---|---|---|---|
| 2024 | **Brain Tumor Classification using Transfer Learning and Ensemble Approach**. J. Shaikh, K. Shaikh | *Journal of Soft Computing Paradigm*, 6(3), 284–298 · [DOI](https://doi.org/10.36548/jscp.2024.3.005) | VGG19 + Random Forest reached 93% on a 7,023-image MRI dataset, ahead of EfficientNetB3 + RF (89%) and a KNN+SVM hybrid (91.2%) |
| 2024 | **Multilingual Misinformation Detection: Deep Learning Approaches for News Authenticity Assessment** | IEEE ICCCNT | BiLSTM and 1D-CNN-BiLSTM on a new 29,484-article English–Hindi dataset; about 92% accuracy per language and multilingual |
| 2024 | **Deep Learning Based Defect Detection and Segmentation for High Energy Material Applications**. S. Jaiswal, K. Shaikh, J. Shaikh, P. Mishra, A. S. Deshmukh, M. Bharadwaj | HEMCE (accepted) | Fine-tuned YOLOv8 segmentation on noisy grayscale images, 98% mAP, compared against Mask R-CNN. Work done at DRDO HEMRL |
| 2024 | **FasterViT for Fine-Grained Image Classification** | IEEE PuneCon 2024 (submitted) | Benchmarked against VGG16 and EfficientNet, 92% accuracy |

---

## Research Experience

**Research Intern, Applied AI & Computer Vision** · DRDO, India · Jul – Nov 2023
Built a YOLOv8 defect-detection pipeline robust to noise, low contrast and occlusion. Ran ablations on anchors and augmentation policy, which became the HEMCE paper.

**Independent Research, FasterViT** · 2024
Implemented FasterViT in PyTorch and benchmarked convergence against CNN baselines.

---

## Selected Projects

| Project | What it is |
|---|---|
| [Curvature-Guided Rank Selection](https://github.com/jish2003/Curvature-Guided-Rank-Selection-for-LoRA-Fine-Tuning-of-Vision-Transformers) | Adaptive per-layer LoRA rank for ViTs (above) |
| [Brain Tumor Classification](https://github.com/jish2003/Brain-Tumor-Classification-using-Transfer-Learning-and-Ensemble-Approach) | Code for the published JSCP paper: VGG19/EfficientNetB3 features + Random Forest, with HPO notebook |
| [OCR with Qwen2-VL](https://github.com/jish2003/OCR-using-Qwen2-VL) | Hindi + English text extraction from images with Qwen2-VL and Byaldi, Streamlit UI and keyword search |
| [Sentiment Analysis for Reviews](https://github.com/jish2003/Sentiment-Analysis-for-Reviews) | BERT-based sentiment on scraped movie reviews |
| [Smart India Hackathon – Scout School](https://github.com/jish2003/Smart-India-Hackathon-Product) | Student–college platform; **Grand Finalist**, led a 6-member team in a 36-hour national competition |

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?logo=opencv&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)

**Models & methods:** CNNs, ViT, FasterViT, LoRA / PEFT, Fisher Information, transfer learning, YOLOv8, BiLSTM, ensembles
**Research practice:** benchmarking, ablations, error analysis, dataset curation, reproducibility
**Compute:** Slurm (USC CARC), V100/A100, Google Colab

---

## Education

- **University of Southern California**, M.S. Computer Science (Artificial Intelligence), 2026 – present. Coursework: Foundations of AI, Machine Learning, Deep Learning, Applied NLP, Web Technology
- **Savitribai Phule Pune University**, B.E. Computer Engineering, 2020 – 2024, CGPA 8.48/10

## Honors

- Smart India Hackathon 2022, Grand Finalist
- Amazon ML Summer School, selected participant
- Top 10%, Python Programming Event, IIT Kharagpur
- Event Coordinator, Computer Engineering Student Association (CESA)
