# Audio Classification CNN

Classify short audio clips (e.g., **dog bark**, **bird chirp**, **siren**, **rain**) with a ResNet-style CNN trained on **Mel Spectrograms**. The project includes a full **training pipeline (PyTorch)**, **FastAPI** inference service, **serverless GPU inference with Modal**, and an **interactive Next.js + React dashboard** for uploads, real-time predictions, and feature‑map visualization.

<img src="https://img.shields.io/badge/Next.js-000?logo=nextdotjs&logoColor=fff&style=for-the-badge" /> <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" /> <img src="https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/PyTorch-DE3412?style=for-the-badge&logo=pytorch&logoColor=white" /> <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" /> <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" /> <img src="https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white" />

---

## ✨ Features

* 🧠 **Deep Audio CNN** for sound classification
* 🧱 **ResNet-style** architecture with residual blocks
* 🎼 **Mel Spectrogram** audio-to-image conversion
* 🎛️ **Data augmentation**: Mixup + SpecAugment (Time/Freq masking)
* ⚡ **Serverless GPU inference** with **Modal**
* 📊 **Interactive Next.js & React dashboard** (Tailwind + shadcn/ui)
* 📈 **Real-time classification** with confidence scores
* 🌊 **Waveform & Spectrogram** visualization
* 🚀 **FastAPI** inference endpoint (+ Pydantic validation)
* 📈 **TensorBoard** integration for training analysis
* ✅ **Pydantic** validation for robust API requests

---

## 🧱 Architecture Overview

* **Why Mel Spectrograms?** They convert audio to a perceptual time–frequency image that CNNs handle well.
* **Why ResNet?** Residual connections ease optimization of deeper models and boost accuracy.
* **Why Mixup/SpecAugment?** Strong regularization for robustness against noise and domain shift.

---

## 🧩 Project Setup

### 1. Python environment

```bash
cd server
conda create -n audio-cnn python=3.11 -y
conda activate audio-cnn
pip install -r requirements.txt
```

### 2. Next.js frontend

```bash
cd client
npm install
npm run dev
```

---

## 🔧 Environment Variables

Create `.env` in your client root

```
NEXT_PUBLIC_MODAL_API_ENDPOINT="Your_API_Key"
```

---

## Features and Interfaces

<img width="1920" height="1080" alt="cnn-1" src="https://github.com/user-attachments/assets/82bcd6d6-410a-4605-a564-ff0c67c57b1e" />

<img width="1920" height="1080" alt="cnn-2" src="https://github.com/user-attachments/assets/f4315322-216d-44a1-a1e1-9384806ad253" />

---

## 🧰 Troubleshooting

* **Torchaudio backend errors**: ensure `ffmpeg`/`libsndfile` installed.
* **Noisy predictions**: raise clip length, tweak Mixup `alpha`, reduce masks.
* **Overfitting**: stronger Mixup/SpecAug, Dropout in classifier, early stopping.
* **Underfitting**: deeper ResNet, higher `base_channels`, longer training, lower weight decay.

---

## 🚀 Need Help??

Feel free to contact me on [Linkedin](https://www.linkedin.com/in/amankrsahu)

[![Instagram URL](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/itz.amansahu/) &nbsp; [![Discord URL](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](discordapp.com/users/539751578866024479)
