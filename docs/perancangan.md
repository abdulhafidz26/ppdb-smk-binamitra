# Dokumentasi Perancangan Sistem PPDB Online SMK Binamitra
**Tahun Ajaran:** 2026 / 2027  
**Pengembang:** Administrator SMK Binamitra  

---

## 1. Pendahuluan & Laporan Singkat
Portal PPDB (Penerimaan Peserta Didik Baru) Online SMK Binamitra dirancang untuk mendigitalisasi proses pendaftaran, manajemen data calon siswa, verifikasi berkas, hingga rekapitulasi kuota kompetensi keahlian secara *real-time* menggunakan penyimpanan berbasis *Client-Side* (`localStorage`).

---

## 2. Arsitektur & Struktur Menu Sistem
Sistem ini dirancang menggunakan Admin Panel terpusat dengan navigasi menu sebagai berikut:
1. **Dashboard (`index.html`):** Menampilkan ringkasan statistik pendaftar secara *real-time*, informasi jalur pendaftaran, serta grafik statistik.
2. **Data Calon Siswa (`data-siswa.html`):** Tabel master data pendaftar lengkap dengan fitur pencarian instan dan tombol aksi.
3. **Verifikasi Detail Siswa (`detail-siswa.html`):** Halaman khusus untuk memeriksa berkas persyaratan dan mengubah status verifikasi (*Terverifikasi*, *Revisi*, atau *Ditolak*).
4. **Data Jurusan & Kuota (`jurusan.html`):** Manajemen kapasitas daya tampung kompetensi keahlian (TKJ, AK, TSM, TKR) beserta persentase keterisiannya.
5. **Laporan Rekapitulasi (`laporan.html`):** Rekapitulasi data pendaftar harian dan cetak laporan resmi sekolah.
6. **Pengumuman & Pengaturan (`pengumuman.html` & `pengaturan.html`):** Broadcast informasi publik dan konfigurasi profil akun pengelola.

---

## 3. Teknologi yang Digunakan
- **HTML5:** Struktur semantik dokumen web.
- **Tailwind CSS (via CDN):** Kerangka kerja *utility-first* untuk desain antarmuka (*UI/UX*) yang modern dan responsif.
- **Font Awesome:** Pustaka ikon visual modern.
- **JavaScript (Vanilla) & LocalStorage:** Interaktivitas DOM, manipulasi data modal, validasi formulir, dan basis data lokal sisi klien.
