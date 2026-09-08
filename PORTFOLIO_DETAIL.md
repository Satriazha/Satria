# 📊 Case Study: Production Planning & Inventory Control (PPIC) System

## 📌 Project Overview
Sistem perencanaan produksi dan pengendalian inventaris terpadu (*Production Planning and Inventory Control System*) berbasis spreadsheet yang dirancang untuk mengoptimalkan kebutuhan bahan baku, mencegah *stockout* pada lini perakitan, serta mengendalikan biaya pemesanan (*Purchase Order*).

* **Model Manufaktur:** Perakitan Router / Modem Internet (Router X-100)
* **Lead Time Default Supplier:** 7 Hari (Sesuai kebijakan pengadaan)
* **Safety Stock Target:** 100 Pcs / Komponen
* **Model Perencanaan:** Master Production Schedule (MPS) & Material Requirement Planning (MRP)

---

## 🛠️ Data Master Bill of Materials (BOM)

Tabel di bawah ini merupakan basis data resep produksi (*Master BOM*) yang mencatat stok awal, mutasi harian, serta stok akhir riil di gudang[cite: 1]:

| Kode Material | Nama Material | Qty / Unit | Stok Awal | Satuan | Harga / Unit (Rp) | Lead Time | Barang Masuk | Barang Keluar | Stok Akhir |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **MAT-01** | Casing Plastik Top/Bottom | 1 | 500 | Pcs | *(Custom)* | 7 Hari | 0 | 0 | **500** |
| **MAT-02** | Main PCB Board | 1 | 350 | Pcs | *(Custom)* | 7 Hari | 0 | 0 | **350** |
| **MAT-03** | Antena Wi-Fi 5GHz | 2 | 800 | Pcs | *(Custom)* | 7 Hari | 0 | 0 | **800** |
| **MAT-04** | Power Adapter 12V | 1 | 200 | Pcs | *(Custom)* | 7 Hari | 0 | 0 | **200** |
| **MAT-05** | Baut / Screw Set | 4 | 2.500 | Pcs | *(Custom)* | 7 Hari | 100 | 0 | **2.600** |

---

## 💻 Sistem Material Requirement Planning (MRP) & ROP

Sistem perhitungan otomatis yang menghubungkan **Rencana Target Produksi** dengan keterisian stok akhir gudang, *Reorder Point* (ROP), dan kebutuhan rilis *Purchase Order* (PO)[cite: 1]:

> **🎯 Target Produksi Simulasi:** 300 Unit Router X-100

| Kode Material | Nama Material | Kebutuhan Produksi | Stok Gudang | Safety Stock | Status Stok | Jumlah Beli (PO) | Lead Time | Reorder Point (ROP) | Tgl Order | Total Biaya |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **MAT-01** | Casing Plastik | 300 | 500 | 100 | 🟢 AMAN | 0 | 7 Hari | 170 | Aman | Rp 0 |
| **MAT-02** | Main PCB Board | 300 | 350 | 100 | 🔴 BAHAYA | **50** | 7 Hari | 170 | TODAY() | Rp 0 |
| **MAT-03** | Antena Wi-Fi | 600 | 800 | 100 | 🟢 AMAN | 0 | 7 Hari | 240 | Aman | Rp 0 |
| **MAT-04** | Power Adapter | 300 | 200 | 100 | 🔴 BAHAYA | **200** | 7 Hari | 170 | TODAY() | Rp 0 |
| **MAT-05** | Baut / Screw Set | 1.200 | 2.600 | 100 | 🟢 AMAN | 0 | 7 Hari | 380 | Aman | Rp 0 |

---

## ⚙️ Formula Kunci & Logika Spreadsheet

1. **Sinkronisasi Stok Akhir Gudang (Sheet BOM):**
   ```excel
   =D5 + I5 - J5
---

## 📞 Ringkasan Ringkas & Kontak

Dokumen ini menunjukkan perpaduan keahlian teknis TIK, logika sistematis dalam operasional & PPIC, serta kemampuan komunikasi pedagogis.

* **Penulis:** Satria Dawas Zhalifunas, S.Kom
* **Lokasi:** Karawang, Jawa Barat, Indonesia
* **Kontak / LinkedIn:** [Profil LinkedIn](https://linkedin.com) | Email: satriazhalifunas@gmail.com
