# California Housing Income Prediction

## Project Introduction

Proyek ini bertujuan untuk memprediksi **Median Income** pada wilayah California menggunakan dataset California Housing. Model dibuat untuk membantu analisis ekonomi wilayah dan pengambilan keputusan terkait perencanaan pembangunan, investasi properti, serta kebijakan sosial-ekonomi.

## Latar Belakang

California adalah wilayah dengan variasi pendapatan yang besar dan perbedaan kondisi lingkungan yang signifikan. Dataset California Housing menyediakan informasi demografis dan geospasial seperti total kamar, jumlah penduduk, usia bangunan, serta kedekatan terhadap laut. Prediksi median income dapat membantu mengurangi biaya survei langsung dan memberikan estimasi yang lebih cepat untuk berbagai pemangku kepentingan.

## Tujuan Proyek

1. Membangun model regresi untuk memprediksi nilai median income.
2. Mengidentifikasi fitur yang paling berpengaruh terhadap prediksi.
3. Menemukan model terbaik dengan akurasi prediksi yang tinggi.
4. Memberikan insight hubungan antara karakteristik lingkungan dan pendapatan.

## Dataset

Dataset yang digunakan adalah `data_california_house.csv`. Fitur penting di antaranya:

- `longitude` dan `latitude`
- `housing_median_age`
- `total_rooms`
- `total_bedrooms`
- `population`
- `households`
- `ocean_proximity`
- `median_income` (target)

## Pendekatan

Analisis dilakukan melalui beberapa tahapan:

1. Eksplorasi data dan pemahaman distribusi fitur.
2. Pembersihan data dengan menangani missing values pada `total_bedrooms`.
3. Feature engineering untuk membuat fitur baru seperti `rooms_per_household`, `bedrooms_per_room`, `population_per_household`, dan `lon_lat_interaction`.
4. Preprocessing data dengan imputasi, standardisasi numerik, dan one-hot encoding untuk fitur kategori.
5. Pelatihan model regresi Linear Regression dan Random Forest Regressor.
6. Evaluasi model menggunakan MAE, RMSE, dan R².

## Hasil Utama

- Model Random Forest memberikan performa lebih baik dibanding Linear Regression.
- Random Forest mencapai R² yang lebih tinggi dan error yang lebih rendah.
- Fitur yang paling berpengaruh adalah rasio `bedrooms_per_room`, diikuti oleh `rooms_per_household` dan kategori `ocean_proximity`.
- Model terbaik disimpan dalam file `best_model_random_forest.pkl`.

## Rekomendasi

1. Gunakan Random Forest sebagai model utama untuk prediksi Median Income.
2. Tambahkan data eksternal seperti tingkat pendidikan, kriminalitas, dan kualitas fasilitas untuk meningkatkan akurasi.
3. Lakukan hyperparameter tuning lebih mendalam untuk optimasi model.
4. Coba model boosting seperti XGBoost atau LightGBM.
5. Visualisasikan hasil prediksi secara geospasial untuk insight lebih kuat.
6. Kembangkan model menjadi API menggunakan Flask atau FastAPI untuk deployment.
7. Lakukan retraining berkala agar model tetap relevan dengan perubahan kondisi ekonomi.

## File Penting

- `Capstone_Project_Kelompok4.ipynb`: notebook analisis dan pemodelan.
- `data_california_house.csv`: dataset California Housing.
- `best_model_random_forest.pkl`: model Random Forest terbaik yang disimpan.

## Cara Menjalankan

1. Pastikan semua dependensi Python tersedia (`pandas`, `seaborn`, `matplotlib`, `scikit-learn`, `pickle`).
2. Jalankan `Capstone_Project_Kelompok4.ipynb` di Jupyter Notebook atau JupyterLab.
3. Pastikan file `data_california_house.csv` berada di direktori yang sama.
