# Struktur File

## bab4_kompresi_gambar_kmeans.ipynb
File ini berisi eksperimen kompresi gambar menggunakan algoritma KMeans. Output dari eksperimen ini berupa file ZIP yang mencakup:

- Gambar hasil kompresi
- File CSV yang berisi kumpulan data eksperimen seperti nilai PSNR, Compression Ratio (CR), waktu komputasi, dan lainnya File CSV inilah yang kemudian digunakan untuk proses analisis selanjutnya.

## result-240630_11-27.csv
File CSV hasil eksperimen yang dilakukan pada 30 Juni 2024 . Data ini digunakan sebagai dasar dalam analisis awal untuk menentukan nilai K optimal.

## BAB4-DATA-ANALYSIS.ipynb
Notebook analisis data yang dibuat sebagai bagian dari skripsi. File ini menganalisis data eksperimen dari result-240630_11-27.csv. Analisis ini menghasilkan kesimpulan bahwa nilai K optimal = 96 berdasarkan kriteria tertentu.

## Revisiting_BAB4_DATA_ANALYSIS.ipynb
Merupakan revisi atau pendekatan alternatif terhadap analisis data hasil eksperimen. File ini menggunakan data eksperimen ulang yang dijalankan pada 8 Juni 2025 , tersimpan dalam file result-250608_09-45.csv.

## Perbedaan Hasil Analisis
Hasil analisis antara analisis original (2024) dan analisis alternatif (2025) menghasilkan nilai K optimal yang berbeda:

- Analisis Original (2024): Nilai K optimal = 96
- Analisis Alternatif (2025): Nilai K optimal = 64

Perbedaan ini muncul karena adanya perbedaan pendekatan dalam pengelolaan data serta kriteria seleksi nilai K.

### Perbedaan Pendekatan Analisis
#### Pendekatan Statistik untuk Agregasi Data
Analisis Original: Dataset dikelompokkan berdasarkan nilai K, lalu setiap variabel direpresentasikan dengan nilai rata-rata (mean) .
Analisis Alternatif: Tetap menggunakan pengelompokan berdasarkan nilai K, namun memilih median sebagai representasi tiap variabel.
Alasan: Median lebih stabil dan representatif dalam dataset yang memiliki sebaran data luas dan outlier tinggi.

#### Perbedaan Kriteria Seleksi K Optimal
**Analisis Original (2024)**  
Kandidat nilai K dipilih berdasarkan tiga kriteria:

- cr >= 0.67 → rasio kompresi minimal sebanding JPEG
- mse <= rata-rata MSE → galat tidak boleh melebihi rata-rata
- psnr >= 30.0 → kualitas gambar tetap terjaga

**Analisis Alternatif (2025)**  
Kriteria seleksi dikembangkan menjadi lebih adaptif dan didasarkan pada distribusi data:

- cr >= 0.67 → tetap menggunakan threshold industri
- psnr >= Q50 → ambil nilai K dengan PSNR masuk ke 50% teratas
- comp_time <= Q70 → ambil nilai K dengan waktu komputasi masuk ke 70% tercepat

Dengan pendekatan ini, analisis menjadi lebih fleksibel dan realistis, terutama jika datanya heterogen atau tidak ideal.

### Kesimpulan
Perbedaan hasil antara kedua analisis bukanlah suatu kesalahan, melainkan wujud dari evolusi pemikiran dan penyempurnaan metode analisis . Dengan pendekatan yang lebih modern dan sesuai karakteristik data, kita bisa mendapatkan hasil yang lebih valid dan generalizable

