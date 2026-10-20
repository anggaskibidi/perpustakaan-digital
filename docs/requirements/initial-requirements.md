# Kebutuhan Awal

Status: draft untuk divalidasi bersama petugas perpustakaan.

## Fungsional

### Katalog
- Pengguna dapat mencari berdasarkan judul, penulis, ISBN/kode, atau kata kunci.
- Hasil dapat difilter menurut kategori dan ketersediaan.
- Hasil dapat diurutkan menurut judul A–Z/Z–A, terbaru, dan popularitas.
- Halaman detail menampilkan metadata dan ketersediaan yang berasal dari backend.
- Definisi "populer" harus ditentukan, misalnya berdasarkan jumlah peminjaman dalam periode tertentu.

### Administrasi
- Pengguna berwenang dapat mengelola data bibliografi, kategori, dan eksemplar.
- Petugas dapat mencatat peminjaman dan pengembalian.
- Stok dan status eksemplar diperbarui secara konsisten saat transaksi.
- Sistem menyimpan riwayat transaksi dan menyediakan laporan.
- Perubahan penting dapat dicatat dalam audit log.

### Akun dan akses
- Hak akses dibedakan untuk admin, petugas, guru, dan siswa.
- Pengguna hanya dapat melihat data pribadi dan riwayat yang menjadi haknya.
- Operasi administratif memerlukan autentikasi dan otorisasi backend.

### Asisten AI
- Memahami permintaan pencarian dalam bahasa sehari-hari.
- Mengubah permintaan menjadi filter katalog yang terstruktur.
- Menampilkan hasil yang diverifikasi melalui layanan pencarian.
- Tidak mengarang buku, stok, atau aturan perpustakaan.
- Tetap menyediakan pencarian biasa saat layanan AI tidak tersedia.
- Tidak dapat mengubah data atau melakukan transaksi tanpa otorisasi dan konfirmasi yang sesuai.

## Nonfungsional
- Antarmuka responsif dan dapat digunakan pada perangkat umum.
- Validasi input dan penanganan error konsisten.
- Kata sandi tidak disimpan dalam bentuk plaintext.
- Rahasia disimpan di environment/configuration yang tidak masuk Git.
- Backup, pemulihan, logging, dan kebijakan retensi data dirancang sebelum penggunaan nyata.
- Data pribadi siswa dan guru dilindungi sesuai kebijakan sekolah dan peraturan yang berlaku.

## Di luar MVP
- Aplikasi iOS native.
- Rekomendasi personal yang kompleks.
- Peminjaman mandiri atau reservasi sebelum alur utama tervalidasi.
- Integrasi layanan eksternal yang belum disetujui sekolah.

## Kriteria MVP
MVP baru dapat diuji jika petugas dapat mengelola katalog dan transaksi dengan benar, pencarian serta ketersediaan konsisten, akses dibatasi berdasarkan role, dan data uji dapat dicadangkan serta dipulihkan.
