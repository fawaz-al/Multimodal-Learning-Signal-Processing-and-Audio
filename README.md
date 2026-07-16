# Multimodal-Learning-Signal-Processing-and-Audio

Repositori ini memuat implementasi komprehensif dari berbagai arsitektur *Machine Learning* untuk memecahkan masalah di ranah pemrosesan sinyal, audio, dan data deret waktu (*time series*). Proyek ini dirancang secara modular untuk memfasilitasi eksperimen *multimodal learning*.

## 🚀 Fitur Utama & Model
Proyek ini terbagi menjadi tiga pilar fungsionalitas utama:

1. **Automatic Speech Recognition (ASR)**
   * **Fungsi:** Mentranskripsikan data audio (suara) menjadi teks dengan akurasi tinggi, bahkan pada lingkungan yang *noisy*.
   * **Model:** [Whisper (OpenAI)](https://github.com/openai/whisper)

2. **Voice Cloning / Text-to-Speech (TTS)**
   * **Fungsi:** Menghasilkan ucapan sintetis yang terdengar natural dari teks masukan, dengan kemampuan meniru karakteristik suara (*voice cloning*).
   * **Model:** Qwen3 TTS 

3. **Time Series Forecasting**
   * **Fungsi:** Menganalisis dan memprediksi pola data berurutan waktu (seperti fluktuasi sinyal audio historis, data metrik, atau tren sejenis).
   * **Pendekatan:** Pemodelan statistik dan *Deep Learning* untuk deret waktu.

## 🛠️ Tech Stack & Library
* **Bahasa:** Python 3.x
* **Framework DL:** PyTorch / TensorFlow 
* **Audio Processing:** Librosa, Torchaudio, SoundFile
* **Data Science:** Pandas, NumPy, Scikit-learn
* **Model Hub:** Hugging Face Transformers

## ⚙️ Instalasi (Installation)
Disarankan untuk menjalankan proyek ini di dalam lingkungan virtual (Virtual Environment) untuk menghindari bentrok pustaka.

1. Clone repositori ini:
   ```bash
   git clone [https://github.com/fawaz-al/Multimodal-Learning-Signal-Processing-and-Audio.git](https://github.com/fawaz-al/Multimodal-Learning-Signal-Processing-and-Audio.git)
   cd Multimodal-Learning-Signal-Processing-and-Audio
2. Buat dan aktifkan virtual environment:
    ```bash
    python -m venv venv
    # Windows
    venv\Scripts\activate
    # Linux/Mac
    source venv/bin/activate
3. Instal dependensi:
    ```bash
    pip install -r requirements.txt
(Catatan: Konfigurasi PyTorch dengan dukungan CUDA sangat disarankan untuk mempercepat proses inferensi Whisper dan Qwen3).

## 📂 Struktur Direktori (Folder Structure)
Untuk menjaga agar repositori tetap rapi, kode dibagi berdasarkan domain tugasnya:

```text
Multimodal-Learning-Signal-Processing-and-Audio/
├── data/                   # Dataset audio dan file CSV (time series)
├── models/                 # Pre-trained weights untuk Qwen3 dan Whisper
├── src/
│   ├── asr/                # Modul Automatic Speech Recognition (Whisper)
│   ├── tts/                # Modul Voice Cloning & TTS (Qwen3)
│   └── forecasting/        # Modul prediksi Time Series
├── notebooks/              # Jupyter Notebook untuk EDA dan eksperimen
├── requirements.txt        # Daftar dependensi library
└── README.md               # Dokumentasi utama
```
