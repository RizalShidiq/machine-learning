# Proyek Prediksi Permintaan Berbagi Sepeda

Proyek ini bertujuan untuk memprediksi jumlah total sepeda yang disewa dalam satu jam berdasarkan atribut lingkungan dan musiman. Model *machine learning* dibangun menggunakan data historis dari program berbagi sepeda.

## Ringkasan

Sistem berbagi sepeda merupakan alternatif yang sehat dan ramah lingkungan untuk transportasi perkotaan. Kemampuan untuk memprediksi permintaan sepeda sangat penting untuk manajemen inventaris, realokasi sepeda, dan untuk memastikan ketersediaan bagi pengguna. Proyek ini mengeksplorasi kumpulan data berbagi sepeda untuk membangun model prediksi yang akurat.

## Dataset

Dataset yang digunakan dalam proyek ini adalah kumpulan data **Bike Sharing**, yang berisi informasi cuaca dan waktu per jam serta jumlah sepeda sewaan. Atribut-atribut utama dalam dataset meliputi:

  * **datetime**: Tanggal dan jam pengukuran
  * **season**: Musim (1: semi, 2: panas, 3: gugur, 4: dingin)
  * **holiday**: Indikator hari libur
  * **workingday**: Indikator hari kerja
  * **weather**: Kondisi cuaca (1: Cerah, 2: Berawan, 3: Hujan ringan, 4: Hujan lebat)
  * **temp**: Temperatur dalam Celsius
  * **atemp**: Temperatur "terasa" dalam Celsius
  * **humidity**: Kelembapan
  * **windspeed**: Kecepatan angin
  * **casual**: Jumlah pengguna biasa
  * **registered**: Jumlah pengguna terdaftar
  * **count**: Jumlah total sepeda yang disewa (target)

## Proses Proyek

1.  **Eksplorasi dan Pra-pemrosesan Data**: Tahap ini mencakup pembersihan data, penanganan nilai yang hilang, dan rekayasa fitur untuk mengekstrak informasi yang relevan dari atribut `datetime`.
2.  **Visualisasi Data**: Membuat visualisasi untuk memahami hubungan antara berbagai fitur dan variabel target.
3.  **Pemilihan dan Pelatihan Model**: Beberapa model regresi dievaluasi untuk memprediksi permintaan sepeda, antara lain:
      * *Linear Regression*
      * *Random Forest Regressor*
      * *Gradient Boosting Regressor*
4.  **Evaluasi Model**: Kinerja model dievaluasi menggunakan metrik seperti *Mean Absolute Error (MAE)*, *Mean Squared Error (MSE)*, dan *R-squared ($R^2$)*.
5.  **Interpretasi Hasil**: Menganalisis hasil prediksi untuk mendapatkan wawasan tentang faktor-faktor utama yang memengaruhi permintaan sepeda.

## Kebutuhan Sistem

Untuk menjalankan *notebook* Jupyter dalam repositori ini, Anda memerlukan pustaka Python berikut:

  * pandas
  * numpy
  * scikit-learn
  * matplotlib
  * seaborn

Anda dapat menginstal dependensi yang diperlukan menggunakan pip:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## Cara Menjalankan

1.  *Clone* repositori ini ke mesin lokal Anda:
    ```bash
    git clone https://github.com/RizalShidiq/machine-learning.git
    ```
2.  Buka direktori proyek:
    ```bash
    cd machine-learning/Bike%20Sharing%20Demand%20Prediction
    ```
3.  Jalankan Jupyter Notebook:
    ```bash
    jupyter notebook "Bike Sharing Demand Prediction.ipynb"
    ```

## Hasil

Model yang dikembangkan menunjukkan kinerja yang baik dalam memprediksi permintaan berbagi sepeda. Model *Gradient Boosting Regressor* mencapai hasil terbaik dengan nilai $R^2$ yang signifikan, menunjukkan bahwa model tersebut dapat menjelaskan sebagian besar varians dalam data. Analisis lebih lanjut mengungkapkan bahwa jam, suhu, dan hari kerja adalah prediktor paling signifikan dari permintaan sepeda.

## Kontributor

  * **Rizal Shidiq** - [RizalShidiq](https://www.google.com/search?q=https://github.com/RizalShidiq)
