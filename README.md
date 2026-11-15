# AKUISISI DATA TEMPAT WISATA DI PROVINSI BALI MENGGUNAKAN OPENSTREETMAP

Nama: Maria Indriani Lelu
NIM: 2501010335
Mata Kuliah: Akuisisi dan Manajemen Data - BIFP-243
Program Studi: Informatika - INSTIKI
Semester / Kelas: 3 / F
Dosen Pengampu: Dr. I Gede Totok Suryawan, S.Kom., M.T.

## Tujuan
Mengumpulkan data tempat wisata di Provinsi Bali sebagai bahan analisis pariwisata, dan sebagai dataset mentah untuk RTM Tugas 2. Data tempat wisata dipilih karena Bali memiliki sebaran atraksi yang luas di sembilan kabupaten/kota, dan datanya tersedia terbuka di OpenStreetMap.

## 1. Sumber data
- **Nama:** OpenStreetMap
- **URL:** https://www.openstreetmap.org/
- **Endpoint API:** https://overpass-api.de/api/interpreter
- **Penerbit:** OpenStreetMap contributors
- **Atribusi:** © OpenStreetMap contributors

## 2. Tanggal dan jam akses
2026-11-15 WITA (sama dengan waktu_akuisisi di docs/provenance.json)

## 3. Metode akuisisi
- **Jenis:** API resmi, Overpass API tanpa API key
- **Parameter:** query Overpass QL untuk objek dengan tag tourism di wilayah Provinsi Bali (area Bali), output JSON, timeout 180 detik
- Kode memakai timeout, User-Agent dengan nama dan NIM pengambil, penanganan status code, dan jeda minimal 1 detik antar-request. Hanya memakai satu request utama agar tidak membebani server.
- **Wilayah
