# Dashboard Inflasi Indonesia
### Analisis dan Prediksi Inflasi Menggunakan Machine Learning

---

## Ringkasan Proyek
**Dashboard Inflasi Indonesia** merupakan aplikasi dashboard interaktif berbasis Streamlit yang dirancang untuk melakukan analisis komprehensif serta prediksi tingkat inflasi Indonesia menggunakan pendekatan statistik dan machine learning.

Platform ini mengintegrasikan eksplorasi data time series, analisis hubungan antar variabel makroekonomi, serta simulasi prediktif untuk membantu memahami dinamika inflasi secara lebih mendalam dan berbasis data.

---

## 🎯 Objectives
* Menganalisis pola historis inflasi Indonesia
* Mengidentifikasi faktor makroekonomi yang mempengaruhi inflasi
* Membandingkan performa model regresi linear dan non-linear
* Menyediakan simulasi prediksi inflasi berbasis input variabel ekonomi

---

## 🚀 Fitur Dashboard
### 1. Time Period Control
* Pemilihan rentang waktu analisis (bulan & tahun)
* Pembaruan visualisasi secara dinamis
* Ringkasan data berdasarkan periode terpilih

---

### 2. Macroeconomic Indicators
Menampilkan indikator ekonomi utama pada periode terakhir yang dipilih:
* Tingkat Inflasi (%)
* BI Rate (%)
* Nilai Tukar IDR/USD
* Uang Beredar (M2)
* Investasi
* Ekspor
* Impor

---

### 3. Trend & Pattern Analysis
* Visualisasi tren inflasi bulanan
* Perbandingan dengan target inflasi Bank Indonesia
* Statistik deskriptif (mean, maksimum, minimum, volatilitas)
* Analisis pola musiman (seasonality detection)

---

### 4. Comparative Economic Analysis
* Perbandingan inflasi dengan variabel makro lainnya
* Visualisasi dual-axis chart
* Scatter plot dengan trendline
* Matriks korelasi antar variabel

---

### 5. Modeling & Forecasting
* Implementasi model regresi linear dan non-linear
* Visualisasi data aktual vs hasil prediksi
* Evaluasi performa model
* Simulasi interaktif: pengguna dapat memasukkan nilai variabel ekonomi untuk memprediksi inflasi

---

### 6. Data Explorer
* Tabel data time series yang dapat difilter
* Ringkasan statistik numerik
* Export data dalam format CSV dan Excel

---

## 🛠️ Teknologi yang Digunakan
* **Streamlit** – Interactive dashboard framework
* **Pandas & NumPy** – Data processing dan manipulasi
* **Plotly** – Visualisasi interaktif
* **Scikit-learn** – Machine learning modeling
* **XGBoost** – Gradient boosting regression
* **Statsmodels** – Statistical time series modeling

---

## 📊 Data Overview
* Periode data: Januari 2010 – Desember 2024
* Frekuensi: Bulanan (Time Series)
* Total observasi: ±180 data
* Sumber: Badan Pusat Statistik (BPS) dan sumber ekonomi internasional

### Variabel yang Digunakan
| Variabel  | Deskripsi                       |
| --------- | ------------------------------- |
| Inflasi   | Tingkat inflasi bulanan (%)     |
| BI Rate   | Suku bunga acuan (%)            |
| Kurs      | Nilai tukar Rupiah terhadap USD |
| M2        | Jumlah uang beredar             |
| Investasi | Total investasi domestik        |
| Ekspor    | Nilai ekspor                    |
| Impor     | Nilai impor                     |

---

## 🔬 Pendekatan Analisis
### Feature Engineering
* Ekstraksi fitur waktu (bulan, tahun)
* Lag features (lag 1, lag 3, lag 12)
* Rolling mean dan rolling standard deviation
* Transformasi log untuk stabilisasi variansi

---

### Model yang Dibandingkan
#### Regresi Linear
* Ordinary Least Squares (OLS)
* Lasso Regression
* Ridge Regression

#### Regresi Non-Linear
* Support Vector Regression (SVR)
* Random Forest Regressor
* XGBoost Regressor

---

### Evaluasi Model
Model dievaluasi menggunakan:
* **MAE (Mean Absolute Error)**
* **RMSE (Root Mean Squared Error)**
* **R² Score (Coefficient of Determination)**

Model terbaik dipilih berdasarkan kombinasi error terendah dan nilai R² tertinggi.

---

## ⚙️ Instalasi & Menjalankan Aplikasi
### Clone Repository
```bash
git clone https://github.com/EvindaEka/Dashboard-Inflasi
cd Dashboard-Inflasi
```

### Setup Virtual Environment
```bash
python -m venv venv

# Windows
venv\Scripts\activate

# Mac/Linux
source venv/bin/activate
```

### Install Dependencies
```bash
pip install -r requirements.txt
```

### Jalankan Dashboard
```bash
streamlit run app.py
```

Aplikasi dapat diakses melalui:
`http://localhost:8501`

---

## 📁 Struktur Proyek
```
Dashboard-Inflasi/
│
├── app.py
├── ridge_model.pkl
├── data_inflasi_JSON.json
├── requirements.txt
└── README.md
```

---

## ⚠️ Catatan Penting
* Pastikan format data sesuai dengan struktur yang digunakan sistem
* Gunakan encoding UTF-8
* Model terlatih disimpan dalam format `.pkl`
* Performa optimal pada dataset time series bulanan

---

## 👥 Pengembangan
Dikembangkan sebagai proyek akademik pada mata kuliah **Workshop Analitika Data Terapan**.

---
