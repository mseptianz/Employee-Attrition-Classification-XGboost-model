# Prediksi Klasifikasi Atrisi Karyawan💡 - ![XGBoost](https://img.shields.io/badge/XGBoost-00B140?style=for-the-badge&logo=XGBoost&logoColor=white)

Repositori ini berisi project prediksi konversi menggunakan beberapa model (KNN, SVM, Decision Tree, Random Forest, XGBoost) klasifikasi dengan base parameter, lalu model terbaik selanjutnya dilakukan hyperparameter tuning, hasilnya model ini menggunakan **XGBoost** sebagai model prediksi. Project ini bertujuan untuk menerapkan model machine learning untuk memprediksi konversi kemungkinan karyawan left dari perusahaan berdasarkan dataset yang tersedia. Repositori ini mencakup file Jupyter Notebook yang menjelaskan proses secara menyeluruh, mulai dari eksplorasi data hingga percobaan model menggunakan unseen data.

## Daftar Isi 🗒️
1. [Link Terkait Project](#link-terkait-project-)
2. [Project Overview](#project-overview-)
3. [Latar Belakang Masalah](#latar-belakang-masalah-)
4. [Problem Statement](#problem-statement-)
5. [Penjabaran Masalah](#penjabaran-masalah-)
6. [Metode yang Digunakan](#metode-yang-digunakan-)
7. [Kesimpulan Analisa](#kesimpulan-analisa)
8. [Test Unseen Data](#test-unseen-data-)
4. [File yang Tersedia](#file-yang-tersedia-)
5. [Cara Menggunakan Project Ini](#cara-menggunakan-project-ini-)
6. [Dependencies](#dependencies-)
7. [Libraries](#libraries-)
8. [Author](#author-)

## Link Terkait Project ⛓️‍💥

- [Dataset](https://www.kaggle.com/datasets/stealthtechnologies/employee-attrition-dataset?select=train.csv)
- [Deployment](https://huggingface.co/spaces/mseptianz/Employee_Attrition)

## Project Overview 📝

Dalam proyek ini, saya menggunakan beberapa model klasifikasi dengan base parameter, lalu model terbaik selanjutnya dilakukan hyperparameter tuning untuk menganalisis data dan membangun model prediksi konversi. Beberapa langkah utama yang dicakup dalam proyek ini adalah:

1. **Import Libraries dan Eksplorasi Data**:
    - Memuat dataset dan melakukan eksplorasi awal untuk memahami struktur dan karakteristik data.

2. **Preprocessing Data**:
    - Melakukan pembersihan dan persiapan data, termasuk penanganan outlier dan imputasi nilai yang hilang.

3. **Pengembangan Model**:
    - Membangun dan melatih model lima model klasifikasi untuk memprediksi konversi.

4. **Evaluasi Model**:
    - Menggunakan metrik evaluasi untuk menilai kinerja model.

5. **Hyperparameter Tuning**:
   - Melakukan hyperparameter tuning menggunakan model terbaik.
     
7. **Evaluasi Model**:
   - Melakukan evaluasi terhadap model yang sudah dituning
     
9. **Pengambilan Keputusan untuk Model dan Bisnis**:
    - Mengambil keputusan terhadap model dan untuk bisnis

## Latar Belakang Masalah 🧐

Dalam dunia bisnis yang kompetitif, sumber daya manusia merupakan aset yang sangat berharga bagi keberhasilan organisasi. Namun, tingkat attrisi karyawan yang tinggi dapat menjadi tantangan signifikan bagi perusahaan, baik dari segi biaya maupun efisiensi operasional. Pergantian karyawan sering kali mengakibatkan penurunan produktivitas, peningkatan biaya rekrutmen, pelatihan, serta hilangnya pengetahuan dan keahlian yang telah dibangun selama bertahun-tahun.

Salah satu pendekatan yang dapat membantu perusahaan dalam mengelola masalah ini adalah dengan menggunakan teknologi prediktif berbasis machine learning. Dengan memanfaatkan data historis karyawan, seperti kinerja, gaji, jabatan, dan indikator lainnya, perusahaan dapat membangun model klasifikasi untuk memprediksi kemungkinan attrisi.

Proyek ini bertujuan untuk mengembangkan model prediksi klasifikasi attrisi karyawan menggunakan teknik machine learning. Dalam proses ini, metrik recall digunakan sebagai ukuran utama keberhasilan model, karena dalam konteks ini, lebih penting untuk meminimalkan kesalahan pada prediksi karyawan yang berisiko tinggi untuk keluar. Dengan model yang akurat dan dapat diandalkan, perusahaan dapat mengidentifikasi pola-pola kritis, membuat strategi retensi yang efektif, dan pada akhirnya meningkatkan stabilitas serta produktivitas organisasi secara keseluruhan.

## Problem Statement √

**Specific:** Membangun model machine learning untuk mendeteksi attrisi karyawan berdasarkan fitur-fitur seperti demografi, karakteristik pekerjaan, dan keadaan pribadi. Tujuan utama adalah mengidentifikasi karyawan yang berisiko keluar dari perusahaan.

**Measurable:** Keberhasilan model akan diukur dengan metrik berikut:

- Akurasi: Minimal 75% dalam prediksi attrisi karyawan.
- Presisi: Menentukan seberapa baik model dalam mengidentifikasi karyawan yang benar-benar berisiko keluar.
- Recall: Fokus pada mendeteksi karyawan berisiko tinggi agar tidak terlewatkan.

**Achievable:** 
- Dataset yang digunakan memiliki kualitas tinggi dan mencakup fitur relevan seperti demografi, gaji, masa kerja, performa, dan lainnya.
- Model akan dilatih menggunakan teknik machine learning seperti Logistic Regression, Decision Tree,XGboost, atau Random Forest, yang sesuai untuk klasifikasi.

**Relevant**: Attrisi karyawan adalah tantangan utama bagi perusahaan karena memengaruhi biaya rekrutmen, pelatihan, dan produktivitas. Dengan model prediksi ini, perusahaan dapat membuat strategi retensi yang lebih efektif, mengurangi kehilangan talenta, dan meningkatkan stabilitas tenaga kerja
**Time-bound:** Proyek ini akan diselesaikan dalam waktu 1 bulan.

**Problem statement:**
Membangun model machine learning yang dapat mendeteksi attrisi karyawan secara akurat berdasarkan fitur profil karyawan yang rinci, termasuk demografi, karakteristik terkait pekerjaan, dan keadaan pribadi dalam satu bulan. Keberhasilan akan diukur menggunakan metrik akurasi, presisi, dan recall, dengan target mencapai tingkat akurasi setidaknya 75% dalam memprediksi karyawan yang berisiko keluar. Proyek ini akan menggunakan dataset profil karyawan yang berisi fitur relevan untuk pelatihan model, memastikan akses ke data berkualitas untuk pemodelan yang efektif.

## Metode yang Digunakan 🛠️

- Statistik Inferensial
- Machine Learning
- Visualisasi Data
- Pemodelan Prediktif

## Kesimpulan Analisa 🧠

1. Berdasarkan hasil dari eksplorasi data, adapun hal yang bisa diimplementasikan dalam mencapai tujuan bisnis:
- Analisis Faktor Kepuasan Kerja
Lakukan analisis lebih lanjut terhadap faktor-faktor yang berkontribusi pada tingginya tingkat kepuasan kerja di kalangan karyawan yang berisiko. Memahami apa yang membuat mereka tetap terlibat dapat membantu menciptakan kondisi serupa di seluruh organisasi.

- Sesuaikan Strategi Rekrutmen
Tinjau praktik rekrutmen untuk mengidentifikasi calon karyawan yang memiliki karakteristik yang terkait dengan risiko attrisi lebih rendah, seperti keterlibatan tinggi dalam aktivitas tim atau umpan balik positif dari rekan kerja. Pendekatan proaktif ini dapat membantu membangun tenaga kerja yang lebih tangguh.

- Pantau Tren Industri
Tetap terinformasi tentang tren industri dan praktik pesaing terkait keterlibatan dan retensi karyawan. Mengadopsi praktik terbaik dari industri dapat membantu organisasi tetap kompetitif dalam menarik dan mempertahankan talenta terbaik.

- Ciptakan Budaya Umpan Balik
Bangun budaya di mana umpan balik secara rutin dipertukarkan antara karyawan dan manajemen. Mendorong diskusi terbuka dapat membantu menangani masalah secara proaktif dan menciptakan lingkungan kerja yang lebih mendukung.
Rekomendasi ini akan membantu organisasi menciptakan pendekatan yang komprehensif untuk retensi karyawan, dengan menangani berbagai faktor yang berkontribusi terhadap attrisi sekaligus memanfaatkan kekuatan prediktif dari model machine learning.

2. Model XGBoost yang dituning menunjukkan bahwa tuning berhasil meningkatkan kemampuan model dalam membedakan antara karyawan yang akan melakukan attrisi dan yang tidak. Sehingga selanjutnya dilakukan beberapa pendekatan dalam strategi bisnis untuk menciptakan dan meningkatkan retensi.

## File yang Tersedia 📂

- `model_trial.ipynb`: Jupyter Notebook yang berisi langkah-langkah analisis data, pengembangan model XGBoost, evaluasi model, dan wawasan yang diperoleh dari analisis.
- `file_inference.ipynb`: Jupyter Notebook yang berisi prediksi unseen data menggunakan model yang sudah dibuat sebelumnya
- `model.pkl`: Hasil penyimpanan model dan preprocessing
- `Dataset/..`: Raw dataset
  
## Cara Menggunakan Project Ini 💻

1. Clone repositori ini ke dalam lokal Anda:
    ```bash
    git clone https://github.com/mseptianz/Employee-Attrition-Classification-XGboost-model.git
    ```

2. Jalankan Jupyter Notebook untuk mengikuti alur analisis data:
    ```bash
    jupyter notebook model_trial.ipynb
    ```

## Dependencies ⚙️

- ![Jupyter Notebook](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)
- ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) 3.10.14
- ![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)

## Libraries 📚
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Plotly
- Seadborn
- Matplotlib


## Author ✍️
**Muhammad Septian Zamzani**

[![linkedin](https://www.linkedin.com/in/muhammad-septian-zamzani-a9a8b5230/)
