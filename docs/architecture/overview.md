# Gambaran Arsitektur

## Prinsip
Gunakan satu backend dan satu sumber data untuk semua klien. Website, desktop, dan mobile tidak boleh memelihara salinan database transaksi yang terpisah.

## Komponen yang direncanakan
- Web client: katalog dan antarmuka pengguna.
- Desktop client: antarmuka petugas bila diperlukan.
- Mobile client: akses katalog dan layanan anggota.
- API service: autentikasi, otorisasi, validasi, pencarian, transaksi, dan laporan.
- Database: metadata buku, eksemplar, anggota, pengguna, dan transaksi.
- AI integration: menafsirkan permintaan lalu memanggil fungsi pencarian terkontrol pada backend.

## Pilihan deployment yang masih terbuka
1. Server lokal di sekolah: perlu jaringan lokal, backup, pemantauan, dan rencana akses dari luar.
2. Server online: perlu anggaran, koneksi internet, pengamanan, serta pengelolaan hosting.
3. Pendekatan campuran hanya dipertimbangkan bila kebutuhan offline benar-benar terbukti.

## Keamanan dasar
- Otorisasi ditegakkan di backend, bukan hanya dengan menyembunyikan tombol.
- Gunakan HTTPS untuk komunikasi melalui jaringan yang tidak dipercaya.
- Validasi semua input dan gunakan query database yang aman.
- Lindungi sesi/token dan batasi percobaan login.
- Jangan mengirim data pribadi yang tidak diperlukan ke penyedia AI.
- Catat aktivitas administratif tanpa menyimpan rahasia dalam log.

## Keputusan teknologi
Belum ditetapkan. Evaluasi kandidat berdasarkan kemampuan pengembang, kemudahan pemeliharaan, kebutuhan perangkat, hosting, dan biaya operasional.
