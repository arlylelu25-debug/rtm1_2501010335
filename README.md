# AKUISISI DATA TEMPAT WISATA DI PROVINSI BALI MENGGUNAKAN OPENSTREETMAP

Nama: Maria Indriani Lelu

NIM: 2501010335

Mata Kuliah: Akuisisi dan Manajemen 
Data - BIFP-243

Program Studi: Teknik Informatika - MDA

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
- **Wilayah:** 9 kabupaten/kota di Provinsi Bali, yaitu Badung, Gianyar, Tabanan, Bangli, Klungkung, Karangasem, Buleleng, Jembrana, dan Kota Denpasar
- **Hasil:** 713 tempat wisata

## 4. Batasan etika
- **Ketentuan:** ODbL, wajib atribusi © OpenStreetMap contributors; jangan mengirim query berulang
- **Lisensi:** Open Database License (ODbL); atribusi dicantumkan di atas
- **Data pribadi:** tidak diambil. Nama orang, nomor telepon, email, foto, dan akun media sosial perorangan tidak menjadi target pengumpulan, walaupun terlihat di sumber
- **Keterbatasan:** data bergantung pada kelengkapan kontribusi OpenStreetMap; alamat yang kosong di sumber dibiarkan kosong dan tidak dibuat-buat; cakupan hanya objek yang memiliki tag tourism di Bali

## 5. Penjelasan kolom (data/raw/openstreetmap_bali_20261115.csv)

<table>
<tr><th>Kolom</th><th>Tipe</th><th>Arti</th><th>Satuan</th></tr>
<tr><td>nama_wisata</td><td>teks</td><td>Nama tempat wisata</td><td>-</td></tr>
<tr><td>kategori</td><td>teks</td><td>Kategori objek wisata dari tag tourism</td><td>-</td></tr>
<tr><td>kabupaten_kota</td><td>teks</td><td>Kabupaten atau kota lokasi objek</td><td>-</td></tr>
<tr><td>latitude</td><td>desimal</td><td>Garis lintang lokasi objek</td><td>derajat</td></tr>
<tr><td>longitude</td><td>desimal</td><td>Garis bujur lokasi objek</td><td>derajat</td></tr>
<tr><td>alamat</td><td>teks</td><td>Informasi alamat jika tersedia di sumber</td><td>-</td></tr>
<tr><td>osm_id</td><td>bilangan bulat</td><td>Identitas objek di OpenStreetMap</td><td>-</td></tr>
</table>

Jumlah record: 713 baris.

## 6. Cara menjalankan ulang
1. pip install pandas requests
2. Buka notebooks/akuisisi_openstreetmap_bali.ipynb, pilih Restart & Run All.
3. Berkas baru tersimpan di data/raw/ dengan tanggal hari itu; berkas lama tidak ditimpa.
