# README - Analisis Perbandingan ARIMA vs Auto ARIMA

## 📌 Deskripsi Singkat
Notebook ini melakukan analisis time series terhadap kurs USD/IDR menggunakan dua pendekatan:
1. **Manual ARIMA (7,2,8)**
2. **Auto ARIMA (10,2,0)**

Model diuji terhadap data aktual selama 30 hari terakhir dan dianalisis dari segi akurasi serta residual error-nya.

---

## 📊 1. Evaluasi Akurasi Model
| Model                  | MAE      | RMSE     |
|------------------------|----------|----------|
| **Manual ARIMA (7,2,8)** | 74.66    | 89.15    |
| **Auto ARIMA (10,2,0)**  | 72.86    | 85.40    |

### 🔍 Interpretasi:
- **Auto ARIMA** memiliki performa sedikit lebih baik berdasarkan MAE dan RMSE.
- Perbedaan relatif kecil, menunjukkan keduanya cukup kompetitif.

---

## 🧮 2. Analisis Residual
### 🔧 Manual ARIMA
- Residual lebih fluktuatif (~35–48).
- Menandakan model mampu menangkap dinamika jangka pendek lebih baik.

### 🤖 Auto ARIMA
- Residual lebih konsisten dan lebih besar (~70-an di awal).
- Cenderung menghasilkan prediksi yang lebih halus atau "rata".

---

## 📈 3. Visualisasi Prediksi
- **Manual ARIMA (Merah)** mengikuti fluktuasi data aktual dengan lebih baik.
- **Auto ARIMA (Oranye)** lebih konservatif dan cenderung linier.
- Di akhir periode, Manual ARIMA sedikit lebih responsif terhadap kenaikan.

---

## ✅ 4. Kesimpulan dan Rekomendasi
- **Auto ARIMA** cocok untuk baseline model dengan akurasi yang cukup dan proses otomatis.
- **Manual ARIMA (7,2,8)** lebih baik dalam menangkap dinamika dan tren harian meski memerlukan tuning manual.

---

Created by: **Pauwerfull**
Date: April 2025
