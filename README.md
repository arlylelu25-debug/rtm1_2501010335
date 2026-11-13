# TUGAS 1 – AKUISISI DAN MANAJEMEN DATA

# AKUISISI DATA TEMPAT WISATA DI PROVINSI BALI MENGGUNAKAN OPENSTREETMAP


## 1. IDENTITAS

- **Mata Kuliah:** Akuisisi dan Manajemen Data
- **Kode Mata Kuliah:** BIFP-243
- **Program Studi:** Informatika
- **Institusi:** Institut Bisnis dan Teknologi Indonesia (INSTIKI)
- **Semester/Kelas:** 3 / F
- **Dosen Pengampu:** Dr. I Gede Totok Suryawan, S.Kom., M.T.
- **Nama :** Maria indriani lelu
- **NIM:** 2501010335

## 2. DESKRIPSI PROYEK

Proyek ini bertujuan mengumpulkan data tempat wisata di Provinsi Bali menggunakan OpenStreetMap melalui Overpass API.

Data yang diperoleh akan disimpan dalam format CSV dan digunakan untuk memenuhi tugas praktik mata kuliah Akuisisi dan Manajemen Data.

## 3. WILAYAH PENGUMPULAN DATA

Wilayah yang menjadi cakupan pengumpulan data adalah sembilan kabupaten/kota di Provinsi Bali:

1. Kabupaten Badung
2. Kabupaten Gianyar
3. Kabupaten Tabanan
4. Kabupaten Bangli
5. Kabupaten Klungkung
6. Kabupaten Karangasem
7. Kabupaten Buleleng
8. Kabupaten Jembrana
9. Kota Denpasar

## 4. SUMBER DATA

- **Nama sumber:** OpenStreetMap
- **Penyedia:** OpenStreetMap contributors
- **API:** Overpass API
- **Website:** https://www.openstreetmap.org/
- **Dokumentasi:** https://wiki.openstreetmap.org/wiki/Overpass_API

## 5. METODE AKUISISI

Pengumpulan data direncanakan menggunakan bahasa pemrograman Python melalui Google Colab dengan library Requests.

Permintaan data dilakukan melalui Overpass API. Data hasil akuisisi akan disimpan dalam format CSV dan JSON sesuai kebutuhan tugas.

## 6. RENCANA KOLOM DATASET

| Nama Kolom | Keterangan |
|---|---|
| nama_wisata | Nama tempat wisata |
| kategori | Kategori objek wisata |
| kabupaten_kota | Kabupaten atau kota |
| latitude | Garis lintang |
| longitude | Garis bujur |
| alamat | Informasi alamat jika tersedia |
| osm_id | Identitas objek di OpenStreetMap |

Data yang tidak tersedia dari sumber akan dibiarkan kosong dan tidak dibuat-buat.

## 7. ETIKA PENGUMPULAN DATA

Pengumpulan data memperhatikan ketentuan penggunaan OpenStreetMap dan Overpass API, termasuk lisensi, batas permintaan, serta penggunaan data secara bertanggung jawab.

Data pribadi seperti nomor telepon, alamat email, dan identitas individu tidak menjadi target pengumpulan.

Atribusi OpenStreetMap akan dicantumkan sesuai ketentuan lisensi.

## 8. STRUKTUR REPOSITORY

```text
rtm1_2501010335/
├── notebooks/
│   └── akuisisi_openstreetmap_bali.ipynb
├── data/
│   └── raw/
├── docs/
│   ├── provenance.json
│   └── data_ethics_checklist.csv
└── README.md
```

## 9. STATUS PENGERJAAN

- [x] Membuat repository GitHub
- [x] Menentukan topik dan sumber data
- [ ] Melakukan akuisisi data
- [ ] Menyimpan dataset mentah
- [ ] Membuat provenance.json
- [ ] Membuat data_ethics_checklist.csv
- [ ] Melengkapi dokumentasi dan pengujian notebook

## 10. LISENSI DAN ATRIBUSI

OpenStreetMap menggunakan Open Database License (ODbL).

© OpenStreetMap contributors

Data dan dokumentasi akhir akan dilengkapi setelah proses akuisisi selesai.
