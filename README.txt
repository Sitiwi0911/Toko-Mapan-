TOKO MAPAN 2 — versi online + login + sinkronisasi

Yang sudah disiapkan:
- PWA: bisa "Tambahkan ke Layar Utama" di HP sehingga tampil seperti aplikasi.
- Tampilan responsif untuk HP dan laptop.
- Login email/password via Supabase Auth.
- Database online Supabase.
- Data barang terpisah per akun.
- Cari nama/barcode.
- Tambah/edit/hapus barang.
- Harga beli, harga jual, stok, barcode.
- Scan barcode kamera pada browser yang mendukung BarcodeDetector.
- Ikon Toko Mapan 2.
- Service worker untuk cache tampilan aplikasi.

CARA MENYALAKAN:
1. Buat project di Supabase.
2. Buka SQL Editor, jalankan isi file supabase_schema.sql.
3. Ambil Project URL dan anon/public key dari Supabase.
4. Buka index.html, ganti:
   SUPABASE_URL = "GANTI_DENGAN_SUPABASE_URL"
   SUPABASE_ANON_KEY = "GANTI_DENGAN_SUPABASE_ANON_KEY"
5. Upload folder ini ke hosting HTTPS (misalnya hosting statis).
6. Buka alamatnya di HP/laptop.
7. Di Android Chrome pilih menu browser → "Tambahkan ke layar utama"/"Install app".

CATATAN:
- Karena memakai login + database online, internet diperlukan untuk sinkronisasi.
- Struktur sudah dibuat agar akun A tidak bisa melihat data akun B.
- Untuk pemakaian produksi, sebaiknya ditambah role pengguna/karyawan, reset password, audit perubahan harga, dan sinkronisasi offline penuh.
- Kamera biasanya mensyaratkan HTTPS dan izin kamera.
