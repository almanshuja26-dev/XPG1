# KAS X PG 1 VILLA

Website pembayaran kas kelas:
- 26 siswa
- Rp5.000 / minggu
- QRIS dari file `qris.jpeg`
- Upload bukti pembayaran
- Login Admin OKTA
- Dashboard verifikasi Terima / Tolak
- Rekap CSV

## Login demo
- Username: `OKTA`
- Password: `OKTA2026`

## Cara pasang di GitHub Pages
1. Buat repository baru di GitHub.
2. Upload `index.html` dan `qris.jpeg`.
3. Masuk **Settings → Pages**.
4. Pilih **Deploy from a branch**, branch `main`, folder `/root`.
5. Simpan dan tunggu GitHub Pages menerbitkan situs.

## Catatan penting
Versi ini sengaja dibuat sebagai **website statis GitHub Pages**. Data pembayaran dan bukti upload disimpan di `localStorage` browser.

Artinya:
- data yang dikirim dari HP/laptop siswa TIDAK otomatis masuk ke laptop admin;
- admin hanya melihat data yang tersimpan pada browser/perangkat yang sama;
- login admin di file HTML bukan keamanan sungguhan karena kode JavaScript bisa dilihat pengguna.

Kalau website ini akan dipakai sungguhan oleh 26 siswa dari perangkat berbeda, perlu backend/database (misalnya Firebase atau Supabase) untuk akun, upload bukti, dan verifikasi admin.
