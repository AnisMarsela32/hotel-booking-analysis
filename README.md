# Analisis Pembatalan Reservasi Hotel

## Repository Outline

Berikut isi dari repository ini:

1. **README.md** – Penjelasan umum mengenai project
2. **notebook.ipynb** – Notebook Python berisi proses analisis data
3. **hotel\_bookings.csv** – Dataset mentah dari Kaggle
4. **data\_bersih\_hotel\_bookings.csv** – Dataset hasil pembersihan

---

## Problem Background

Pembatalan reservasi hotel menjadi tantangan besar dalam industri perhotelan. Dampaknya mencakup:

* Kehilangan pendapatan
* Ketidakefisienan dalam perencanaan sumber daya
* Gangguan operasional

Dengan menganalisis data historis, kita bisa mengetahui faktor-faktor yang menyebabkan pembatalan, lalu menggunakannya untuk membuat strategi bisnis yang lebih baik.

---

## Project Output

Project ini menghasilkan:

* **Analisis data** menggunakan Python
* **Statistik deskriptif dan inferensial**
* **Visualisasi dashboard interaktif** menggunakan Tableau
* **Insight dan rekomendasi** untuk mendukung keputusan bisnis

---

## Data

Dataset yang digunakan adalah **Hotel Booking Demand** dari Kaggle:

* Jumlah kolom: 32
* Jumlah baris: ±119.000
* Format: CSV
* Terdapat missing values pada kolom `agent`, `company`, dan `country`
* Tipe data: numerik, kategorikal, dan waktu
* Target variabel: `is_canceled` (0 = tidak batal, 1 = batal)

---

## Method

### 1. Data Preparation

* Menghapus duplikat
* Menangani missing value
* Transformasi tipe data

### 2. Exploratory Data Analysis (EDA)

* Statistik deskriptif: mean, median, std
* Visualisasi: histogram, boxplot, bar chart
* Identifikasi outlier dan pola

### 3. Statistical Inference

* Uji hipotesis (2-sample t-test) antara `lead_time` pelanggan yang batal dan tidak batal

---

## Tools & Stack

| Tools/Library        | Fungsi                             |
| -------------------- | ---------------------------------- |
| **Python**           | Bahasa pemrograman utama           |
| **Pandas**           | Manipulasi dan pembersihan data    |
| **Matplotlib**       | Visualisasi dasar                  |
| **Seaborn**          | Visualisasi statistik              |
| **Jupyter Notebook** | Mencatat dan menjalankan analisis  |
| **Tableau**          | Visualisasi interaktif (dashboard) |
| **GitHub**           | Repositori dan kolaborasi project  |

---

## Tableau Public Dashboard (Live)

🔗 **Link dashboard Tableau interaktif:**
[Klik di sini untuk melihat dashboard Hotel Booking di Tableau Public](https://public.tableau.com/views/HotelBookingDemand_17478335915830/HotelBookingDemand?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

---

## Insight & Rekomendasi

### Temuan Utama:

1. Tingkat pembatalan sebesar **27.8%**
2. **City Hotel** memiliki pembatalan lebih tinggi dibanding Resort Hotel
3. Semakin panjang **lead time**, semakin besar kemungkinan reservasi dibatalkan
4. Pelanggan dengan **"No Deposit"** lebih cenderung membatalkan

### Rekomendasi Bisnis:

* Terapkan sistem **deposit minimal**
* Berikan **insentif bagi early booking**
* Targetkan segmen pelanggan yang lebih stabil (misal keluarga)
* Gunakan model prediksi pembatalan untuk manajemen risiko

---

## Reference

* [Pandas Tutorial – W3Schools](https://www.w3schools.com/python/pandas/default.asp)
* [Matplotlib Pyplot – W3Schools](https://www.w3schools.com/python/matplotlib_intro.asp)
* [Visualisasi Data – YouTube Megabagus Herlambang](https://www.youtube.com/@megabagusherlambang/videos)
* [Dataset Kaggle – Hotel Booking Demand](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
* [Tableau Public Dashboard](https://public.tableau.com/views/HotelBookingDemand_17478335915830/HotelBookingDemand)

