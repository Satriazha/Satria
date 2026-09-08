# 📁 Detailed Portfolio Case Studies

Selamat datang di repositori studi kasus dan portofolio detail saya! Dokumen ini memuat dokumentasi komprehensif dari tiga bidang keahlian utama saya: **Operasional PPIC & Supply Chain**, **Pendidikan Informatika & CS Unplugged**, serta **Administrasi & Validasi Dokumen**.

---

## 📌 Daftar Isi
1. [Studi Kasus 1: Production Planning & Inventory Control (PPIC)](#-studi-kasus-1-production-planning--inventory-control-ppic)
2. [Studi Kasus 2: Paket Kurikulum & Modul Ajar TIK Sekolah Dasar](#-studi-kasus-2-paket-kurikulum--modul-ajar-tik-sekolah-dasar)
3. [Studi Kasus 3: Operasional Administrasi & Validasi Berkas](#-studi-kasus-3-operasional-administrasi--validasi-berkas)
4. [Ringkasan Ringkas & Kontak](#-ringkasan-ringkas--kontak)

---

## 📊 Studi Kasus 1: Production Planning & Inventory Control (PPIC)

### 1. Overview & Latar Belakang
Pada industri manufaktur modern, ketidakseimbangan antara ketersediaan bahan baku (*raw material*) dan jadwal produksi sering menyebabkan *bottleneck* serta biaya penyimpanan (*holding cost*) yang membengkak. Studi kasus ini mensimulasikan sistem pengendalian inventaris dan perencanaan produksi terpadu.

### 2. Tantangan Utama
* **Stockout vs Overstock:** Fluktuasi permintaan pasar yang menyebabkan risiko kekurangan bahan baku saat proses perakitan.
* **Accuracy Tracking:** Ketidaksesuaian antara jumlah stok di sistem digital dengan kondisi riil di gudang.
* **Procurement Lead Time:** Keterlambatan pengiriman bahan baku dari vendor yang berdampak pada *master production schedule* (MPS).

### 3. Solusi & Metodologi
1. **Demand Forecasting & Safety Stock:**
   * Menggunakan metode *Exponential Smoothing* untuk memprediksi kebutuhan bahan baku selama 3 bulan ke depan.
   * Menghitung nilai **Safety Stock (SS)** dan **Reorder Point (ROP)** menggunakan formula:
     $$	ext{ROP} = (	ext{Daily Usage} 	imes 	ext{Lead Time}) + 	ext{Safety Stock}$$
2. **Material Requirements Planning (MRP):**
   * Menyusun Bill of Materials (BOM) multi-level untuk melacak komponen hingga tingkat terkecil.
   * Menerapkan *Lot-for-Lot (L4L)* dan *Economic Order Quantity (EOQ)* untuk menentukan ukuran pesanan yang efisien.
3. **Stock Ledger & Audit Trail:**
   * Membangun formulir penerimaan/pengeluaran barang yang terintegrasi dengan rumus perkalian otomatis (`VLOOKUP`, `SUMIFS`, `INDEX-MATCH`) pada Excel untuk memperbarui stok secara real-time.

### 4. Hasil & Dampak Operasional
| Parameter | Sebelum Optimasi | Setelah Optimasi | Peningkatan |
| :--- | :--- | :--- | :--- |
| **Akurasi Stok Gudang** | 82% | 98.5% | **+16.5%** |
| **Kejadian Stockout** | 4-5x / bulan | < 1x / bulan | **Penerunan 80%** |
| **Lead Time Pengadaan** | 7 hari | 4 hari | **Lebih Cepat 42%** |

---

## 📚 Studi Kasus 2: Paket Kurikulum & Modul Ajar TIK Sekolah Dasar

### 1. Overview & Latar Belakang
Mengajarkan Informatika kepada siswa Sekolah Dasar (Fase A dan Fase C) membutuhkan pendekatan adaptif. Di banyak sekolah, keterbatasan jumlah perangkat komputer menjadi tantangan utama. Oleh karena itu, dirancang modul ajar berbasis **Computer Science (CS) Unplugged** dan *Problem-Based Learning* (PBL).

### 2. Struktur Modul & Metode Pembelajaran
* **Fase A (Kelas 1):** Pengenalan Konsep Simbol & Logika Pengelompokan.
* **Fase C (Kelas 5):** Bab Analisis Data & Visualisasi (Sensus Hobi / Survei Lingkungan).
* **Pendekatan Deep Learning:**
  * *Unplugged Informatics:* Siswa belajar logika algoritma, pencatatan turus/tally mark, dan pengelompokan data menggunakan kertas, kartu, dan aktivitas fisik tanpa tergantung pada layar komputer.
  * *Plugged Digitalization:* Demonstrasi digitalisasi data langsung ke lembar kerja Excel/PowerPoint untuk menampilkan grafik batang otomatis secara real-time.

### 3. Komponen Lembar Kerja Peserta Didik (LKPD)
1. **Aktivitas Wawancara (Detektif Data):** Siswa bergerak secara interaktif (kinestetik) untuk mengumpulkan data dari 10 teman sekelas.
2. **Pengolahan Data Manual:** Mengubah data acak menjadi tabel turus (*tally mark*).
3. **Visualisasi Grafik:** Menggambar grafik batang sederhana secara manual sebelum dikonversi ke format digital.

### 4. Rubrik Asesmen & Evaluasi
* **Asesmen Diagnostik:** Pengukuran emosional dan kognitif awal siswa.
* **Asesmen Formatif:** Observasi dinamika kelompok dan kecermatan pencatatan data.
* **Asesmen Sumatif:** Tes pemahaman konseptual dan penyusunan kalimat dari data.

---

## 📑 Studi Kasus 3: Operasional Administrasi & Validasi Berkas

### 1. Overview & Latar Belakang
Dalam lingkungan kerja administrasi skala besar (seperti di BPN Karawang via agency tata.id), validasi dokumen dan pengarsipan yang tepat merupakan kunci keamanan dan kepatuhan hukum (*legal compliance*).

### 2. Workflow & Standar Operasional Prosedur (SOP)

| Tahap | Aktivitas Utama | Deskripsi & Target | Media / Tool |
| :---: | :--- | :--- | :--- |
| **01** | **📥 Penerimaan Berkas** | Penyerahan fisik berkas & pencatatan registrasi awal | Logbook / Google Sheets |
| **02** | **🔍 Verifikasi & Validasi** | Pemeriksaan keabsahan stempel, tanda tangan & data legal | Checklist SOP Validasi |
| **03** | **💻 Input Data Digital** | Merekam meta-data dokumen ke dalam basis data | Aplikasi BPN / Excel |
| **04** | **🏷️ Pengkodean & Barcode** | Penempelan label identifikasi unik/barcode pada folder | Printer Barcode & Label |
| **05** | **📁 Pengarsipan Ganda** | Penyimpanan fisik (Warkah) & backup data ke cloud | Rak Arsip & Cloud Storage |

> **⚠️ Alur Penanganan Kendala (Retur/Revisi):** 
> Apabila pada **Tahap 02** berkas dinyatakan *tidak lengkap*, berkas akan dikembalikan ke pemohon beserta lembar *Checklist Kekurangan* untuk dilengkapi terlebih dahulu sebelum masuk ke **Tahap 03**.

### 3. Key Achievements & Best Practices
* **Peningkatan Efisiensi Pengarsipan:** Mengimplementasikan penataan kode indeks yang sistematis sehingga waktu pencarian berkas (*retrieval time*) berkurang dari 15 menit menjadi kurang dari 3 menit.
* **Akurasi Data:** Memvalidasi ribuan lembar dokumen pertanahan dengan tingkat kesalahan (*error rate*) di bawah 0.1%.
* **Kerapihan Logbook Digital:** Memelihara *Audit Trail* dan logbook penyerahan berkas harian menggunakan Google Workspace / Excel.

---

## 📞 Ringkasan Ringkas & Kontak

Dokumen ini menunjukkan perpaduan keahlian teknis TIK, logika sistematis dalam operasional & PPIC, serta kemampuan komunikasi pedagogis.

* **Penulis:** Satria Dawas Zhalifunas, S.Kom
* **Lokasi:** Karawang, Jawa Barat, Indonesia
* **Kontak / LinkedIn:** [Profil LinkedIn](https://linkedin.com) | Email: satriazhalifunas@gmail.com
