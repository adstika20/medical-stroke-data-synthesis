# Synthetic Data for Stroke Prediction: Bayesian Network vs Generative Adversarial Network (GAN)

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

## 🛠 Tools & Technologies
Menggunakan Librarty synthcity dokumentasi resmi nya kunjungi [Read the docs](https://github.com/vanderschaarlab/synthcity)

Evaluasi menilai 3 poin ini :
- KS Test (Kolmogorov-Smirnov Test)
- PCA (Principal Component Analysis)
- TSTR (Train on Synthetic, Test on Real)

## 🧪 Project Highlights


## 📌 Next Steps
