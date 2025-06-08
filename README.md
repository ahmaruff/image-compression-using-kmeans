# Ekstraksi Palet Warna untuk Kompresi Gambar Digital menggunakan Algoritma K-Means

Repositori ini berisi kode dan hasil penelitian skripsi/tugas akhir tentang ekstraksi palet warna untuk kompresi gambar digital menggunakan algoritma K-Means.

## Abstrak

Seiring berkembangnya teknologi berdampak pada makin meningkatnya kebutuhan untuk efisiensi kompresi data gambar. Penelitian ini bertujuan untuk mengevaluasi performa algoritma K-Means dalam kompresi gambar digital. Algoritma K-Means digunakan untuk mengekstraksi palet warna dominan pada gambar, diikuti oleh proses kuantisasi warna untuk rekonstruksi gambar. Penelitian ini mengeksplorasi dampak jumlah klaster (K) terhadap rasio kompresi dan nilai Peak Signal to Noise Ratio (PSNR).

Penelitian ini menggunakan metode eksperimen dengan melakukan kompresi pada gambar RGB 24-bit dengan berbagai resolusi (VGA, SVGA, HD, FHD) menggunakan jumlah klaster yang bervariasi (8, 16, 32, 64, 96, 128). Analisis deskriptif dan korelasi dilakukan untuk mengevaluasi hubungan antara variabel jumlah klaster, rasio kompresi, nilai MSE (Mean Squared Error), nilai PSNR, dan durasi komputasi.

Hasil penelitian menunjukkan bahwa algoritma K-Means efektif dalam kompresi gambar dengan rata-rata rasio kompresi 67%, nilai MSE 63,747, nilai PSNR 33,47 dB, dan durasi komputasi 2,59 detik. Jumlah klaster berpengaruh kuat terhadap kualitas kompresi, dengan nilai PSNR dan rasio kompresi meningkat seiring bertambahnya jumlah klaster. Jumlah klaster optimal untuk kompresi gambar adalah 96, yang menghasilkan kompresi berkualitas baik dengan durasi komputasi yang efisien.

**Kata Kunci:** Kompresi gambar, K-Means, Ekstraksi palet warna, Kuantisasi warna.

## Deskripsi

Repositori ini berisi implementasi dan analisis dari metode kompresi gambar menggunakan algoritma K-Means untuk ekstraksi palet warna. Penelitian ini fokus pada pengoptimalan jumlah klaster untuk mendapatkan keseimbangan terbaik antara rasio kompresi dan kualitas gambar.

### Fitur Utama

- Kompresi gambar digital menggunakan algoritma K-Means
- Analisis hubungan antara jumlah klaster dan kualitas kompresi
- Evaluasi performa menggunakan metrik PSNR dan MSE
- Eksplorasi parameter optimal untuk berbagai resolusi gambar

## Dataset

Dataset yang digunakan dalam penelitian ini dapat diakses melalui [link dataset](https://drive.google.com/drive/u/1/folders/13cc9m-1gNY--0HOwyTi2XadrwHo5KsvH). Dataset terdiri dari gambar dengan berbagai resolusi (VGA, SVGA, HD, FHD) untuk menguji performa algoritma kompresi.

## Hasil Penelitian

Beberapa hasil utama dari penelitian ini:

- Algoritma K-Means efektif dalam mengekstraksi palet warna untuk kompresi gambar
- Rata-rata rasio kompresi mencapai 67%
- Nilai PSNR rata-rata 33,47 dB
- Jumlah klaster optimal adalah 96, memberikan keseimbangan antara kualitas gambar dan efisiensi komputasi

## Kontribusi

Kontribusi untuk perbaikan atau pengembangan lebih lanjut sangat diterima. Silakan buat *pull request* atau buka *issue* untuk diskusi lebih lanjut.

## Lisensi

Proyek ini dilisensikan di bawah Lisensi MIT - lihat file [LICENSE](LICENSE) untuk detail lebih lanjut.

## Kontak

[Ahmad Ma'ruf] - [ahmadmaruf2701@gmail.com]

Link Proyek: [https://github.com/ahmaruff/image-compression-using-kmeans](https://github.com/ahmaruff/image-compression-using-kmeans)