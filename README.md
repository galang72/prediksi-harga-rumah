# RealEstatePrediction-Streamlit

## 📝 Deskripsi
Real Estate Prediction adalah aplikasi berbasis web yang dikembangkan menggunakan Streamlit untuk memprediksi harga rumah. Aplikasi ini mengimplementasikan dua model machine learning: Multiple Linear Regression dan Backpropagation Neural Network untuk memberikan estimasi harga yang akurat berdasarkan berbagai fitur properti.

## 🚀 Fitur Utama
- Prediksi harga rumah menggunakan dua model machine learning
- Uji akurasi model dengan dataset kustom
- Visualisasi perbandingan performa model
- Interface yang user-friendly dan responsif

## 🛠️ Teknologi yang Digunakan
- Python 3.x
- Streamlit
- TensorFlow
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Joblib
- Streamlit-option-menu

## 📊 Variabel Input
- Luas Tanah (m²)
- Luas Bangunan (m²)
- Jumlah Kamar Tidur
- Jumlah Kamar Mandi
- Keberadaan Garasi

## 💻 Instalasi

1. Clone repository
```bash
git clone https://github.com/username/RealEstatePrediction.git
cd RealEstatePrediction
```

2. Install dependencies yang diperlukan
```bash
pip install streamlit tensorflow scikit-learn pandas numpy matplotlib seaborn joblib streamlit-option-menu
```

3. Jalankan aplikasi
```bash
streamlit run forecasting.py
```

## 📦 Struktur Project
```
.streamlit/
├── forecasting.py        # File utama aplikasi
├── model_bpn.h5         # Model Backpropagation Neural Network
├── model_mlr.pkl        # Model Multiple Linear Regression
├── README.md            # Dokumentasi
├── scaler.pkl          # Standard Scaler untuk preprocessing
└── HARGA RUMAH JAK... # Dataset harga rumah
```

## 🔍 Cara Penggunaan

### Prediksi Harga
1. Pilih menu "Prediksi Harga"
2. Masukkan nilai untuk setiap variabel input
3. Pilih algoritma prediksi yang diinginkan
4. Klik tombol "Prediksi Harga"
5. Hasil prediksi akan ditampilkan

### Uji Akurasi
1. Pilih menu "Uji Akurasi"
2. Upload file dataset (.xlsx)
3. Sistem akan menampilkan:
   - Metrik evaluasi kedua model
   - Scatter plot perbandingan hasil prediksi
   - Analisis performa model

## 📊 Metrik Evaluasi
- R² Score (Coefficient of Determination)
- MSE (Mean Squared Error)
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- MAPE (Mean Absolute Percentage Error)

## 📋 Format Dataset
File Excel (.xlsx) dengan kolom:
- LT (Luas Tanah)
- LB (Luas Bangunan)
- JKT (Jumlah Kamar Tidur)
- JKM (Jumlah Kamar Mandi)
- GRS (Garasi - "ADA"/"TIDAK ADA")
- HARGA
- KOTA (Opsional, tidak digunakan dalam prediksi)

