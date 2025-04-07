# 🪖 Helmet Detection with YOLOv11

Proyek ini bertujuan untuk mendeteksi penggunaan helm pada manusia menggunakan model YOLOv11. Sistem ini dapat digunakan untuk keperluan keamanan dan monitoring.
## 🚀 Training Colabs
[Training Colabs](https://colab.research.google.com/drive/17VnnHTPFaXMK2Mye3U3wQtf71Qn3QK6C?usp=sharing)

---

## 📦 Fitur
- Deteksi dua kelas: `Helmet` dan `Without Helmet`
- Menggunakan YOLOv11 (versi modifikasi)
- Real-time inference dari kamera atau video
- Visualisasi bounding box dan confidence score

---
### 1. Clone Repository
```bash
git clone https://github.com/BagusDarmawan-Tech/Deteksi-Helmet-Dengan-YOLO-11.git
cd Deteksi-Helmet-Dengan-YOLO-11

## ⚙️ Instalasi
### 🐍 Requirement
[Install Anaconda](https://repo.anaconda.com/archive/Anaconda3-2024.10-1-Windows-x86_64.exe)

Masuk ke Anaconda Prompt dan jalankan:
```bash
### 1. Install Yolo
conda create --name yolo-env1 python=3.12
conda activate yolo-env1
### 2.Install pytorch
cd /PATH/direktori/my_model
pip3 install --upgrade torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124

### 3.Run
python yolo_detect.py --model my_model.pt --source usb0 --resolution 1280x720

python yolo_detect.py --model my_model.pt --source cctv.mp4

python yolo_detect.py --model my_model.pt --source test_1.jpg
---

