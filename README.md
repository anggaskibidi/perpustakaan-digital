# Perpustakaan Digital

Sistem perpustakaan digital yang dirancang untuk menghubungkan katalog buku, layanan anggota, pengelolaan perpustakaan, dan asisten AI dalam satu ekosistem.

> **Status:** Perencanaan awal. Belum siap digunakan untuk operasional perpustakaan.

## Tujuan

- Menyediakan katalog buku yang mudah dicari oleh siswa dan guru.
- Mendukung filter dan pengurutan, seperti kategori, ketersediaan, populer, terbaru, dan alfabetis.
- Membantu petugas mengelola koleksi, anggota, peminjaman, pengembalian, dan laporan.
- Menyediakan asisten AI yang membantu pencarian berdasarkan data katalog yang sebenarnya.
- Menyiapkan fondasi lintas platform: web, komputer admin, Android, dan kemungkinan iOS.

## Prinsip desain

1. **Satu sumber data.** Semua klien menggunakan backend dan database yang sama.
2. **AI bukan sumber kebenaran.** Ketersediaan dan detail buku harus diverifikasi oleh backend.
3. **Mulai dari MVP.** Katalog dan alur administrasi dasar lebih dahulu; fitur lanjutan menyusul.
4. **Keamanan sejak awal.** Hak akses, validasi, pencatatan aktivitas, dan perlindungan data pribadi harus dirancang sebelum deployment.
5. **Dibangun bertahap.** Proyek dikerjakan sesuai waktu yang tersedia dan hasil analisis kebutuhan nyata.

## Rencana platform

| Platform | Sasaran awal |
| --- | --- |
| Web | Katalog untuk siswa dan guru serta antarmuka petugas |
| Desktop | Antarmuka admin khusus komputer perpustakaan jika memang dibutuhkan |
| Android | Akses katalog dan layanan anggota |
| iOS | Tahap lanjutan setelah kebutuhan dan pendekatan teknis dikonfirmasi |
| AI assistant | Pencarian bahasa alami dan rekomendasi berbasis katalog |

## Rencana fitur

- [ ] Analisis proses perpustakaan yang berjalan saat ini
- [ ] Katalog buku, kategori, filter, dan pengurutan
- [ ] Manajemen anggota dan akun
- [ ] Peminjaman, pengembalian, dan stok eksemplar
- [ ] Riwayat transaksi dan laporan
- [ ] Hak akses admin, petugas, guru, dan siswa
- [ ] Asisten AI untuk pencarian katalog
- [ ] Antarmuka desktop dan mobile
- [ ] Pengujian keamanan, pencadangan, dan pemulihan data

## Struktur repository

```text
apps/
  web/                 # Website katalog dan antarmuka web
  desktop/             # Aplikasi desktop admin (rencana)
  mobile/              # Aplikasi Android/iOS (rencana)
services/
  api/                 # Backend dan API (rencana)
  ai-assistant/        # Integrasi asisten AI (rencana)
packages/
  shared/              # Tipe dan utilitas bersama
database/
  migrations/          # Perubahan skema database
  seeders/             # Data contoh untuk pengembangan
  diagrams/            # ERD dan diagram data
docs/
  planning/            # Tujuan, ruang lingkup, dan roadmap
  requirements/        # Kebutuhan fungsional dan nonfungsional
  architecture/        # Keputusan dan diagram arsitektur
  api/                 # Kontrak API
tests/                 # Strategi dan pengujian lintas komponen
.github/
  ISSUE_TEMPLATE/      # Template issue
```

Folder yang belum berisi implementasi hanya berfungsi sebagai tempat kerja awal; teknologi final belum diputuskan.

## Mulai berkontribusi

Baca [dokumen perencanaan](docs/planning/README.md), [kebutuhan awal](docs/requirements/initial-requirements.md), dan [arsitektur awal](docs/architecture/overview.md). Jangan masukkan data siswa sungguhan, kata sandi, token API, atau rahasia sekolah ke repository.

## Status keputusan

Stack teknologi, lokasi hosting, kebijakan peminjaman, lisensi, dan mekanisme login masih perlu dikonfirmasi. Repository yang bersifat publik tidak berarti data operasional atau data pribadi boleh dipublikasikan.

## Lisensi

Belum ditentukan. Lisensi perlu diputuskan setelah kepemilikan dan izin penggunaan kode untuk proyek sekolah dikonfirmasi.
