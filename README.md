# Ekstraksi Palet Warna untuk Kompresi Gambar Digital menggunakan Algoritma K-Means

Repositori ini berisi kode dan hasil penelitian skripsi/tugas akhir tentang ekstraksi palet warna untuk kompresi gambar digital menggunakan algoritma K-Means.

Publikasi hasil penelitian ini dapat diakses melalui:

[Ma’ruf, A., Sibyan, H., & Mardiyantoro, N. (2025). *Ekstraksi Palet Warna untuk Kompresi Gambar Digital menggunakan Algoritma K-Means*. Jurnal Informatika dan Rekayasa Perangkat Lunak, 7(1), 134–141.](https://publikasiilmiah.unwahas.ac.id/JINRPL/issue/view/540)

---

## Abstract

The growing needs for efficient image data compression have been driven by rapid technological advancement. This study evaluates the effectiveness of the K-Means algorithm for digital image compression through dominant color palette extraction and subsequent color quantization for image reconstruction.

The research investigates how the number of clusters (K) affects both compression ratio and Peak Signal-to-Noise Ratio (PSNR). An experimental approach was implemented, compressing 24-bit RGB images at various resolutions (VGA, SVGA, HD, FHD) using different cluster quantities (8, 16, 32, 64, 96, 128). Through descriptive and correlation analyses, relationships between cluster numbers, compression ratio, Mean Squared Error (MSE), PSNR values, and computation time were examined.

Results demonstrate that the K-Means algorithm achieves effective image compression, with an average compression ratio of 67%, MSE of 0.00077, PSNR of 81.43 dB, and computation time of 0.73 seconds. Compression quality was strongly influenced by cluster quantity, with both PSNR values and compression ratios improving as cluster numbers increased. The research determined that 96 clusters represents the optimal configuration, delivering high-quality compression with reasonable computational efficiency

**Keywords** Color palette extraction, K-Means, Image compression, Color quantization

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

## Library
Sebagai bagian dari penelitian ini, saya mengembangkan sebuah library Python yang mengimplementasikan metode kompresi gambar menggunakan algoritma K-Means.  
Library tersebut dapat diakses melalui repositori berikut:  
[kmeans-img-compress](https://github.com/ahmaruff/kmeans-img-compress)

## Lisensi

Proyek ini dilisensikan di bawah Lisensi MIT - lihat file [LICENSE](LICENSE) untuk detail lebih lanjut.

## Kontak

[Ahmad Ma'ruf](ahmadmaruf2701@gmail.com)
