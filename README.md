# End-to-End-Supervised-Learning-Data-Preprocessing-to-Modelling

Ringkasan Proyek
Proyek ini berisi penerapan supervised learning menggunakan dua dataset berbeda untuk masalah klasifikasi dan regresi. Fokus utamanya adalah pada alur kerja machine learning secara end-to-end, mulai dari pemahaman data, feature engineering, pembangunan model prediktif, hingga evaluasi kinerja dan interpretasi hasil untuk mendapatkan insight yang relevan. Proyek ini juga menampilkan kemampuan dalam menangani data numerik dan kategorikal, termasuk penanganan outliers dan missing values.

Dataset yang Digunakan :
Dataset Hepatitis: Data klinis untuk memprediksi Hepatitis C, menyoroti penanganan missing values dan outliers pada data medis.
Dataset Fuel Consumption Ratings: Data karakteristik kendaraan untuk memprediksi emisi CO2, fokus pada aplikasi model regresi.

Metodologi & Alur Kerja
Proyek ini terbagi menjadi dua bagian, masing-masing dengan pendekatan yang disesuaikan.

Bagian 1: Dataset Fuel Consumption Ratings
Bagian ini berfokus pada pemilihan fitur dan pembangunan model regresi.
Pengambilan & Pemahaman Data: Dataset dimuat dan dieksplorasi untuk memahami strukturnya.
Pemilihan Fitur: Kolom yang tidak relevan ('Make', 'Model', 'Vehicle Class', 'Fuel Type', 'Transmission') dihilangkan.
Pembangunan Model Regresi:
Regresi Linier: Model dasar dilatih untuk prediksi emisi CO2.
Regresi Polinomial: Fitur diubah dengan PolynomialFeatures (derajat 2) untuk menangkap hubungan non-linier sebelum melatih model regresi.
Evaluasi & Perbandingan Model: Kedua model dievaluasi menggunakan Mean Absolute Error (MAE) dan R-squared (R² Score), dan hasilnya dibandingkan untuk menentukan performa terbaik.

Bagian 2: Dataset Hepatitis 
Bagian ini berfokus pada pemrosesan data medis untuk klasifikasi dan evaluasi model.
Pengambilan & Pemahaman Data: Dataset dimuat dan dieksplorasi untuk mengidentifikasi struktur, dimensi, dan keberadaan missing values serta duplikat.
Pembersihan & Preprocessing data:
Missing Values: Fitur numerik diimputasi dengan nilai rata-rata, sedangkan fitur kategorikal ('Sex') diimputasi dengan modus.
Outliers: Deteksi outliers dilakukan menggunakan Histogram dan Boxplot. Penanganannya menggunakan metode Interquartile Range (IQR) 1.5 dan nilai-nilai outliers dibatasi (capped) pada batas yang dihitung.
Encoding Kategorikal: Fitur kategorikal ('Sex', 'Category') diubah menjadi numerik menggunakan LabelEncoder.
Penskalaan Fitur: Fitur numerik diskalakan menggunakan StandardScaler.
Pembangunan Model Klasifikasi: Model RandomForestClassifier dilatih pada data yang telah diproses.
Evaluasi & Interpretasi Model: Kinerja model dievaluasi menggunakan accuracy score, confusion matrix, classification report, serta perbandingan model

Kesimpulan :
Proyek ini telah mendemonstrasikan kapabilitas dalam seluruh siklus supervised learning. Saya belajar bahwa data preprocessing yang teliti, pemilihan model yang tepat, dan interpretasi hasil yang mendalam adalah kunci untuk membangun solusi berbasis data yang akurat dan dapat dipercaya dalam berbagai skenario.

Tools & Library
Bahasa Pemrograman: Python

Library: pandas, numpy, matplotlib, seaborn, scipy.stats, sklearn (termasuk model_selection, preprocessing, ensemble, linear_model, metrics)

Cara Menjelajahi Proyek
Untuk melihat alur kode dan analisis secara detail, buka file 3323600055_Farhan Hasbi Hasyidan_Supervised Learning.ipynb menggunakan Jupyter Notebook atau Google Colab.

Dataset yang digunakan dapat ditemukan di folder /dataset dalam repositori ini.
