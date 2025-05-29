# Synthetic Data for Stroke Prediction: Bayesian Network vs Generative Adversarial Network (GAN)

![Ilustrasi Stroke Prediction](https://github.com/adstika20/medical-stroke-data-synthesis/blob/main/2807765_18140.jpg)

Ilustrasi oleh Freepik - [https://www.freepik.com](https://www.freepik.com)


Proyek ini membahas penggunaan **data sintetis** untuk meningkatkan akurasi model prediksi risiko stroke, terutama dalam situasi terbatasnya akses terhadap data medis asli yang bersifat sensitif dan dilindungi.

Dua pendekatan generatif yang dibandingkan dalam penelitian ini:
- **Bayesian Network (Jaringan Bayesian)**
- **Generative Adversarial Network (GAN)**

Data sintetis dihasilkan dalam dua skala, yaitu sebanyak **500 entri** dan **1000 entri**. Data ini digunakan untuk melatih model prediksi stroke dan dievaluasi berdasarkan:
- **Kualitas data sintetis**
- **Kinerja model prediksi**
- **Kelayakan penggunaan untuk aplikasi medis yang menjaga privasi**

> ⚠️ *Repositori ini tidak memuat data medis asli. Seluruh data yang digunakan merupakan data sintetis yang dihasilkan untuk keperluan penelitian.*


## 📊 Dataset Description
Dataset yang digunakan dalam proyek ini berasal dari salah satu rumah sakit dan memuat **100 entri data medis pasien stroke**. Tabel berikut menjelaskan masing-masing variabel dalam dataset:

| Variable | Description                   | Data Type | Unit              |
|----------|-------------------------------|-----------|-------------------|
| Stroke   | Stroke status (0 = stroke, 1 = non-stroke) | int64     | -                 |
| BPMJ     | Fingertip Pulse               | int64     | bpm (beats/min)   |
| BPMP     | Wrist Pulse                   | int64     | bpm (beats/min)   |
| SPOJ     | Fingertip Oxygen Saturation   | int64     | %                 |
| SPOP     | Wrist Oxygen Saturation       | int64     | %                 |
| SUHUJ    | Fingertip Temperature         | float64   | °C                |
| SUHUP    | Wrist Temperature             | float64   | °C                |

## 🛠 Perangkat dan Teknologi

Proyek ini menggunakan pustaka **[SynthCity](https://github.com/vanderschaarlab/synthcity)**, yaitu sebuah library Python untuk sintesis data tabular berbasis metode generatif, termasuk GAN dan Bayesian Network. Dokumentasi resmi dapat diakses melalui tautan berikut:  
🔗 [SynthCity Documentation – Read the Docs](https://github.com/vanderschaarlab/synthcity)

Library lain yang digunakan dalam proyek ini adalah:
- `pandas`, `numpy`, `matplotlib` – untuk manipulasi data dan visualisasi.
- `scikit-learn` – untuk evaluasi model prediksi dan uji performa.

---

## 📈 Metode Evaluasi

Kualitas data sintetis dievaluasi menggunakan tiga pendekatan utama berikut:

- **Kolmogorov–Smirnov (KS) Test**  
  Mengukur kesamaan distribusi antara data asli dan data sintetis untuk setiap fitur numerik.

- **Principal Component Analysis (PCA)**  
  Digunakan untuk memvisualisasikan distribusi data sintetis dibandingkan dengan data asli dalam ruang berdimensi rendah (reduksi dimensi).

- **Train on Synthetic, Test on Real (TSTR)**  
  Mengukur kemampuan generalisasi model yang dilatih menggunakan data sintetis dan diuji pada data asli. Metode ini menguji seberapa “realistis” data sintetis dalam konteks pelatihan model prediktif.

## Hasil dan Analisis



## ⚙️ Installation
Untuk menjalankan proyek ini secara lokal, ikuti langkah-langkah berikut:

### 1. Clone the repository

```bash
git clone https://github.com/username/your-repo-name.git
cd your-repo-name
```
### 2. Buat dan aktifkan environment virtual (opsional tetapi disarankan)
```
python -m venv venv
source venv/bin/activate        # Untuk Linux/macOS
venv\Scripts\activate           # Untuk Windows
```
### 3. Instal semua dependensi
Pastikan Anda telah menginstal `pip`. Kemudian jalankan perintah:
```
pip install -r requirements.txt
```
## 📌 Next Steps
