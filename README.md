# Nama Kelompok 2 :
- Muhammad Rozagi (G1A022008)
- Ulfa Stevi Juliana (G1A022042)
- Revo pratama (G1A022058)
- Rizki Ramadani D. (G1A022054)
- Ahmad Zul Zhafran (G1A022088)

# 📊 Customer Segmentation using Clustering Algorithms

Proyek ini merupakan studi eksploratif untuk membandingkan tiga algoritma *unsupervised learning* dalam melakukan segmentasi pelanggan berdasarkan dataset ritel. Tiga algoritma yang digunakan yaitu **K-Means**, **K-Medoids**, dan **DBSCAN**.

## 📁 Dataset

Dataset berisi informasi pelanggan seperti:
- Usia (*Age*)
- Pendapatan tahunan (*Annual Income*)
- Skor pengeluaran (*Spending Score*)

Dataset ini cocok digunakan untuk tugas segmentasi pelanggan dalam konteks ritel atau pemasaran.

## 🎯 Tujuan

Melakukan studi perbandingan efektivitas dari tiga algoritma clustering dalam mengelompokkan pelanggan, dengan mengevaluasi hasil klaster berdasarkan karakteristik setiap kelompok dan nilai **Silhouette Score**.

## 🛠️ Algoritma yang Digunakan

- **K-Means**: Mengelompokkan data berdasarkan centroid yang dihitung dari rata-rata.
- **K-Medoids**: Mirip dengan K-Means, tetapi menggunakan titik data aktual sebagai pusat cluster.
- **DBSCAN**: Mengelompokkan data berdasarkan kepadatan dan dapat mengidentifikasi outliers (noise).

## 📌 Hasil Singkat

- K-Means dan K-Medoids membentuk 4 cluster yang serupa dengan Silhouette Score yang cukup tinggi.
- DBSCAN mendeteksi outliers dan menghasilkan cluster dengan bentuk yang lebih fleksibel, namun Silhouette Score lebih rendah.
- Segmentasi pelanggan berhasil menunjukkan kelompok konsumen aktif dan tidak aktif, terlepas dari tingkat pendapatan.

## 📈 Evaluasi

Setiap model dievaluasi menggunakan metrik:
- **Silhouette Score**: untuk mengukur seberapa baik klaster terbentuk.
- **Analisis karakteristik klaster**: untuk menilai relevansi dan keterpisahan antar kelompok.

| Algoritma  | Jumlah Cluster | Silhouette Score |
|------------|----------------|------------------|
| K-Means    | 4              | 0.4932           |
| K-Medoids  | 4              | 0.4913           |
| DBSCAN     | 3 + noise      | 0.3989           |

## 💻 Tools

- Python
- Scikit-learn
- NumPy, Pandas
- Matplotlib, Seaborn

## 📚 Kesimpulan

K-Means dan K-Medoids menghasilkan segmentasi pelanggan yang cukup baik dan seimbang, sementara DBSCAN lebih unggul dalam mendeteksi data yang tidak sesuai pola (*outliers*). Pemilihan algoritma terbaik bergantung pada kebutuhan analisis, apakah lebih menekankan pada segmentasi umum atau deteksi anomali.
