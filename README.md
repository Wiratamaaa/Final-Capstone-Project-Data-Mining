# Final-Capstone-Project-Data-Mining

## Deskripsi Project

Project ini merupakan implementasi metode **Machine Learning** untuk memprediksi harga rumah berdasarkan berbagai karakteristik atau fitur yang dimiliki suatu properti. Tujuan utama dari project ini adalah membangun model prediksi yang mampu memberikan estimasi harga rumah secara akurat melalui proses pengolahan data, pemodelan, dan evaluasi model.

Dalam pengerjaannya, project mengikuti tahapan data science secara lengkap, mulai dari **data preprocessing**, **feature engineering**, **pembangunan model**, **evaluasi performa**, hingga **hyperparameter tuning** untuk memperoleh model terbaik.

## Tujuan Project

Project ini dibuat dengan tujuan untuk:

* Membangun model Machine Learning untuk memprediksi harga rumah.
* Melakukan preprocessing data agar siap digunakan dalam proses pelatihan model.
* Membandingkan performa beberapa algoritma regresi.
* Mengoptimalkan performa model menggunakan hyperparameter tuning.
* Menyimpan model terbaik sehingga dapat digunakan kembali tanpa melakukan proses training ulang.

## Metodologi

Tahapan yang dilakukan dalam project ini meliputi:

1. Import library yang diperlukan.
2. Memuat dataset.
3. Exploratory Data Analysis (EDA).
4. Data preprocessing menggunakan **Pipeline** dan **ColumnTransformer**.
5. Pembagian data menjadi data training dan data testing.
6. Pelatihan beberapa model regresi.
7. Evaluasi performa model menggunakan metrik yang sesuai.
8. Hyperparameter tuning pada model Random Forest.
9. Pemilihan model terbaik.
10. Penyimpanan model menggunakan format **Pickle (.pkl)**.

## Teknologi yang Digunakan

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

## Model yang Digunakan

Project ini menggunakan beberapa algoritma Machine Learning, di antaranya:

* Linear Regression
* Random Forest Regressor

Selain itu, preprocessing dan model digabungkan menggunakan **Scikit-learn Pipeline**, sehingga seluruh proses transformasi data dan prediksi dapat dijalankan secara otomatis dalam satu objek model.

## Hasil

Berdasarkan proses pelatihan dan evaluasi, dilakukan perbandingan beberapa model regresi dan proses hyperparameter tuning untuk memperoleh model dengan performa terbaik. Model terbaik kemudian disimpan dalam format **Pickle (.pkl)** sehingga dapat digunakan kembali untuk melakukan prediksi tanpa perlu melakukan training ulang.
