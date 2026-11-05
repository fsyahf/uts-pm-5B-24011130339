# LAPORAN UTS PEMROGRAMAN MOBILE 2

## A. Identitas Mahasiswa

- **Nama:** FERDIAN SYAHFIZRAH
- **NIM:** 24011130339
- **Program Studi:** D3 Manajemen Informatika
- **Kelas:** 5B
- **Mata Kuliah:** Pemrograman Mobile 2
- **Universitas:** Universitas Bani Saleh

## B. Deskripsi Proyek

Proyek ini merupakan aplikasi Profil Mahasiswa berbasis Flutter yang digunakan untuk menampilkan informasi pribadi mahasiswa, foto profil, statistik pengikut, informasi kontak, keahlian, dan galeri proyek.

Pada pengerjaan Ujian Tengah Semester (UTS), dilakukan perbaikan terhadap delapan bug yang terdapat pada aplikasi starter. Selain memperbaiki bug, dilakukan penggantian data mahasiswa dan penyesuaian desain antarmuka agar aplikasi memiliki tampilan yang lebih menarik dan responsif.

## C. Dokumentasi Perbaikan 8 Bug

### 1. Foto Profil Tidak Muncul

- **Gejala:** Foto profil tidak tampil dan muncul kesalahan saat aplikasi memuat gambar.
- **File:** `pubspec.yaml` dan `lib/data/data_profil.dart` (sesuaikan).
- **Penyebab:** Konfigurasi atau lokasi aset gambar belum sesuai.
- **Perbaikan:** Memperbaiki konfigurasi aset pada `pubspec.yaml` dan memastikan lokasi foto profil sesuai dengan path yang digunakan aplikasi.
- **Hasil:** Foto profil berhasil ditampilkan.

### 2. Setengah Bagian Foto Terpotong

- **Gejala:** Bagian bawah foto profil terpotong pada area banner.
- **File:** File widget header atau profil (sesuaikan).
- **Penyebab:** Pengaturan posisi dan ukuran foto belum sesuai dengan tata letak banner.
- **Perbaikan:** Menyesuaikan posisi, ukuran, dan tata letak foto profil agar tampil dengan baik.
- **Hasil:** Foto profil tampil bulat dan tidak terpotong.

### 3. Kartu Informasi Menampilkan Layar Merah

- **Gejala:** Kartu informasi menyebabkan aplikasi menampilkan layar merah.
- **File:** File widget kartu informasi (sesuaikan).
- **Penyebab:** Terdapat kesalahan pada struktur layout atau pengaturan widget.
- **Perbaikan:** Memperbaiki susunan widget dan menyesuaikan ukuran komponen kartu informasi.
- **Hasil:** Kartu informasi dapat ditampilkan dengan normal.

### 4. Email dan Program Studi Melewati Batas Layar

- **Gejala:** Teks email dan program studi terlalu panjang sehingga melewati batas kanan layar.
- **File:** File widget informasi profil (sesuaikan).
- **Penyebab:** Teks belum memiliki pengaturan agar menyesuaikan ruang yang tersedia.
- **Perbaikan:** Menyesuaikan pengaturan layout teks agar dapat membungkus atau menyesuaikan ukuran ruang.
- **Hasil:** Teks tampil dengan rapi tanpa overflow.

### 5. Chip Keahlian Melewati Batas Layar

- **Gejala:** Daftar chip keahlian melewati batas kanan layar.
- **File:** File widget keahlian (sesuaikan).
- **Penyebab:** Susunan chip belum mendukung perpindahan ke baris berikutnya.
- **Perbaikan:** Menyesuaikan susunan chip agar dapat berpindah ke baris berikutnya ketika ruang tidak mencukupi.
- **Hasil:** Seluruh chip keahlian tampil tanpa overflow.

### 6. Galeri Proyek Menampilkan Layar Merah

- **Gejala:** Bagian galeri proyek menyebabkan aplikasi menampilkan layar merah.
- **File:** File widget galeri proyek (sesuaikan).
- **Penyebab:** Terdapat ketidaksesuaian pengaturan layout pada daftar proyek.
- **Perbaikan:** Memperbaiki struktur layout dan pengaturan tampilan galeri proyek.
- **Hasil:** Galeri proyek dapat ditampilkan dengan normal.

### 7. Tampilan Rusak pada Layar Lebar

- **Gejala:** Tampilan aplikasi mengalami kerusakan atau error pada layar dengan lebar 600 dp ke atas.
- **File:** File halaman utama atau widget layout responsif (sesuaikan).
- **Penyebab:** Pengaturan layout belum menangani perbedaan ukuran layar.
- **Perbaikan:** Menyesuaikan layout responsif agar menggunakan satu kolom pada layar di bawah 600 dp dan dua kolom pada layar 600 dp ke atas.
- **Hasil:** Tampilan aplikasi dapat menyesuaikan ukuran layar dengan baik.

### 8. Tombol Ikuti Tidak Berfungsi

- **Gejala:** Ketika tombol Ikuti ditekan, tampilan tombol dan jumlah pengikut tidak berubah.
- **File:** File widget tombol Ikuti (sesuaikan).
- **Penyebab:** Pengelolaan state pada tombol belum berjalan dengan benar.
- **Perbaikan:** Memperbaiki pengelolaan state agar perubahan status tombol dan jumlah pengikut dapat diperbarui.
- **Hasil:** Tombol Ikuti dapat mengubah status dan jumlah pengikut.

## D. Pengujian Aplikasi

Pengujian dilakukan untuk memastikan aplikasi dapat berjalan dengan baik pada berbagai ukuran layar.

| No. | Pengujian | Hasil |
|---|---|---|
| 1 | Tampilan layar 360 dp | Menunggu pengujian |
| 2 | Tampilan layar 800 dp | Menunggu pengujian |
| 3 | Foto profil | Berhasil tampil |
| 4 | Kartu informasi | Berhasil tampil |
| 5 | Chip keahlian | Tidak overflow |
| 6 | Galeri proyek | Berhasil tampil |
| 7 | Tombol Ikuti | Menunggu pengujian |

## E. Perubahan Desain dan Data

Selain perbaikan bug, dilakukan beberapa penyesuaian pada aplikasi, antara lain:

1. Mengganti informasi profil menggunakan data mahasiswa.
2. Mengganti foto profil dengan foto pribadi.
3. Menyesuaikan warna dan tampilan antarmuka.
4. Mengubah susunan elemen pada halaman profil.
5. Menyesuaikan tampilan kartu informasi.
6. Memperbarui tampilan galeri proyek.
7. Menyesuaikan tampilan agar responsif pada berbagai ukuran layar.

## F. Penggunaan AI

Dalam pengerjaan proyek UTS ini, AI digunakan sebagai alat bantu untuk memahami kesalahan kode, menganalisis penyebab bug, memberikan saran perbaikan, serta membantu penyusunan dokumentasi proyek.

Seluruh perubahan kode tetap diperiksa dan diuji kembali pada aplikasi Flutter.

## G. Kesimpulan

Berdasarkan pengerjaan proyek UTS Pemrograman Mobile 2, dilakukan perbaikan terhadap delapan bug pada aplikasi Profil Mahasiswa. Selain itu, dilakukan penggantian data pribadi dan penyesuaian desain antarmuka.

Melalui perbaikan tersebut, aplikasi diharapkan dapat berjalan dengan baik, memiliki tampilan yang lebih menarik, serta mampu menyesuaikan ukuran layar perangkat.

---

**Repository GitHub:**  
https://github.com/fsyahf/uts-pm-5B-24011130339