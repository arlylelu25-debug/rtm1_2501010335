# AKUISISI DATA TEMPAT WISATA DI PROVINSI BALI MENGGUNAKAN OPENSTREETMAP

## 1. IDENTITAS
- Mata Kuliah: Akuisisi dan Manajemen Data
- Kode Mata Kuliah: BIFP-243
- Program Studi: Informatika
- Institusi: Institut Bisnis dan Teknologi Indonesia (INSTIKI)
- Semester/Kelas: 3 / F
- Dosen Pengampu: Dr. I Gede Totok Suryawan, S.Kom., M.T.
- Nama: Maria Indriani Lelu
- NIM: 2501010335

## 2. DESKRIPSI PROYEK
Proyek ini mengumpulkan data tempat wisata di Provinsi Bali menggunakan OpenStreetMap melalui Overpass API.

Data berhasil diperoleh sebanyak 713 tempat wisata pada tanggal 15 November 2026 dan disimpan dalam format CSV di data/raw/openstreetmap_bali_20261115.csv untuk memenuhi tugas praktik mata kuliah Akuisisi dan Manajemen Data.

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
- Nama sumber: OpenStreetMap
- Penyedia: OpenStreetMap contributors
- API: Overpass API
- Website: https://www.openstreetmap.org/
- Dokumentasi: https://wiki.openstreetmap.org/wiki/Overpass_API

## 5. METODE AKUISISI
Pengumpulan data dilakukan menggunakan bahasa pemrograman Python melalui Google Colab dengan library Requests.

Permintaan data dilakukan melalui Overpass API dengan query objek tourism di wilayah Provinsi Bali. Data hasil akuisisi disimpan dalam format CSV dan dilengkapi dengan file provenance di docs/provenance.json sebagai bukti asal data.

## 6. KOLOM DATASET
File: data/raw/openstreetmap_bali_20261115.csv

Nama Kolom - Keterangan
nama_wisata - Nama tempat wisata
kategori - Kategori objek wisata
kabupaten_kota - Kabupaten atau kota
latitude - Garis lintang
longitude - Garis bujur
alamat - Informasi alamat jika tersedia
osm_id - Identitas objek di OpenStreetMap

Data yang tidak tersedia dari sumber dibiarkan kosong dan tidak dibuat-buat.

## 7. ETIKA PENGUMPULAN DATA
Pengumpulan data memperhatikan ketentuan penggunaan OpenStreetMap dan Overpass API, termasuk lisensi, batas permintaan, serta penggunaan data secara bertanggung jawab.

Data pribadi seperti nomor telepon, alamat email, dan identitas individu tidak menjadi target pengumpulan.

Atribusi OpenStreetMap dicantumkan sesuai ketentuan lisensi.

## 8. STRUKTUR REPOSITORY
rtm1_2501010335/
- data/
    - raw/
        - openstreetmap_bali_20261115.csv
- docs/
    - provenance.json
    - data_ethics_checklist.csv
- README.md

## 9. STATUS PENGERJAAN
- [x] Membuat repository GitHub
- [x] Menentukan topik dan sumber data
- [x] Melakukan akuisisi data
- [x] Menyimpan dataset mentah (713 data)
- [x] Membuat provenance.json
- [ ] Membuat data_ethics_checklist.csv
- [ ] Melengkapi dokumentasi dan pengujian notebook

## 10. LISENSI DAN ATRIBUSI
OpenStreetMap menggunakan Open Database License (ODbL).

(C) OpenStreetMap contributors

Data tersedia di data/raw/openstreetmap_bali_20261115.csv dan bukti asal data di docs/provenance.json.

