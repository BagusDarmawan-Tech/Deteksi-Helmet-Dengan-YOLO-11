# 🪖 Deteksi Helm dengan YOLOv11

Proyek ini mendeteksi penggunaan helm pada manusia menggunakan YOLOv11, cocok untuk keamanan dan pemantauan.

##  Training Colabs

[Training Colabs](https://colab.research.google.com/drive/17VnnHTPFaXMK2Mye3U3wQtf71Qn3QK6C?usp=sharing)

##  Fitur

* Deteksi: `Helmet`, `Without Helmet`
* YOLOv11 (modifikasi)
* Deteksi langsung dari kamera, video, gambar
* Visualisasi kotak batas & keyakinan

## ⚙️ Instalasi

1.  **Clone Repository:**

    ```bash
    git clone [https://github.com/BagusDarmawan-Tech/Deteksi-Helmet-Dengan-YOLO-11.git](https://github.com/BagusDarmawan-Tech/Deteksi-Helmet-Dengan-YOLO-11.git)
    cd Deteksi-Helmet-Dengan-YOLO-11
    ```

2.  **Anaconda & PyTorch:**

    * [Install Anaconda](https://repo.anaconda.com/archive/Anaconda3-2024.10-1-Windows-x86_64.exe)
    * Anaconda Prompt:

        ```bash
        conda create --name yolo-env1 python=3.12
        conda activate yolo-env1
        cd /PATH/direktori/my_model
        pip3 install --upgrade torch torchvision torchaudio --index-url [https://download.pytorch.org/whl/cu124](https://download.pytorch.org/whl/cu124)
        ```

3.  **Jalankan Deteksi:**

    * Kamera:

        ```bash
        python yolo_detect.py --model my_model.pt --source usb0 --resolution 1280x720
        ```

    * Video:

        ```bash
        python yolo_detect.py --model my_model.pt --source cctv.mp4
        ```

    * Gambar:

        ```bash
        python yolo_detect.py --model my_model.pt --source test_1.jpg
        ```

### Penjelasan:

* `--model`: Path model YOLOv11.
* `--source`: Input (kamera, video, gambar).
* `--resolution`: Resolusi input.

### Catatan:

* Pastikan path model & sumber input benar.
* Driver kamera terinstal.
* Model terlatih untuk hasil terbaik.
