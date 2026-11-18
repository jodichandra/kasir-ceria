# 🎈 Kasir Pintar - Market Day Anak SD

Aplikasi kasir sederhana satu halaman (*single page application*) berbasis **HTML, CSS, dan JavaScript murni**. Didesain khusus untuk kegiatan **Market Day sekolah dasar / stan bazar anak-anak**. 

Aplikasi ini **tidak memerlukan login** atau backend server dan **semua data tersimpan otomatis di browser (Local Storage)**. Jika browser tidak sengaja di-refresh atau tertutup, data menu, pesanan, kasir, dan riwayat transaksi tetap aman tersimpan.

---

## 🌟 Fitur Baru & Peningkatan

### 1. 🔢 Format Angka & Nominal Ramah Anak SD (Edukasi Matematika)
- **Format Ribuan Otomatis**: Saat mengetik harga menu baru (misal: `10000`) atau uang tunai di kasir, angka langsung otomatis terformat rapi dengan pemisah titik ribuan (`10.000` atau `Rp 10.000`). Anak-anak tidak akan lagi bingung menghitung jumlah angka nol!
- **Teks Terbilang Otomatis (Live)**: Di bawah kolom input harga dan uang kembalian, langsung keluar teks cara membaca uangnya:
  - `10.000` ➡️ *👉 Dibaca: Sepuluh Ribu Rupiah*
  - `5.000` ➡️ *👉 Dibaca: Lima Ribu Rupiah*
  - `2.500` ➡️ *👉 Dibaca: Dua Ribu Lima Ratus Rupiah*
- **Tombol Pintas Cepat**: Di form tambah menu tersedia tombol klik instan: `1.000`, `2.000`, `3.000`, `5.000`, `10.000`, dan `+500`.

### 2. 👤 Manajemen Petugas Kasir Jaga Stand (Shift Kasir)
- **Tombol Kasir di Header**: Menampilkan nama anak yang sedang bertugas jaga (misal: `👤 Kasir: Aisyah`).
- **Ganti / Tambah Petugas Kasir**:
  - Klik nama kasir di header untuk membuka pop-up pergantian kasir.
  - Tambah nama-nama anak yang piket jaga stand (misal: *Aisyah, Budi, Fatih, Zahra, Rian, Bu Guru Ani*).
  - Cukup sekali klik untuk memilih siapa yang sedang piket kasir saat itu.
- **Tercatat di Struk**: Setiap transaksi dan struk belanja otomatis merekam nama anak yang menjadi kasir.
- **Laporan Penjualan Per Kasir (Leaderboard Kasir)**:
  - Di menu **Rekap Penjualan**, terdapat kartu breakdown performa setiap kasir:
    - Nama kasir jaga
    - Berapa kali transaksi yang berhasil dilayani
    - Total pcs barang/makanan yang laku saat kasir tersebut bertugas
    - **Total Omset Penjualan yang dihasilkan oleh kasir tersebut**
  - **Filter Kasir**: Anda bisa memfilter seluruh riwayat dan tabel transaksi berdasarkan kasir tertentu.

---

## 🛒 Fitur Utama Lainnya

1. **Pop-up Nama Toko / Stan / Kelas**
   - Saat pertama kali aplikasi dibuka, otomatis muncul pop-up untuk mengisi **Nama Stan / Kelas** (misal: *Stand Ceria Kelas 4A*) dan slogan.
   - Nama stand ini bisa diubah kapan saja dengan mengklik tombol **"Ubah"** di header.
   - Tercetak otomatis di bagian atas struk belanja.

2. **Daftar Menu & Kategori**
   - Menampilkan kartu menu produk lengkap dengan harga dalam format Rupiah, nama, dan ikon emoji yang ceria.
   - Filter menu cepat: **Semua**, **Makanan**, **Minuman**, **Snack**, dan **Lainnya/Kerajinan**.
   - Kolom pencarian untuk mencari menu dengan cepat.
   - Disertai contoh menu bawaan khas Market Day (Es Teh, Sosis Bakar, Jasuke, Donat, dll).

3. **Daftar Pesanan / Keranjang Kasir**
   - Cukup **klik kartu menu** untuk langsung memasukkan ke daftar jual di sebelah kanan.
   - Jika diklik lagi (klik 2x), jumlah (**Qty**) langsung bertambah 2x secara otomatis.
   - Terdapat tombol `+` dan `−` untuk menyesuaikan jumlah porsi.
   - Menampilkan harga satuan dan subtotal secara otomatis.
   - Total banyak barang (*pcs*) dan **Total Yang Harus Dibayar** dihitung otomatis dengan angka yang besar dan jelas.

4. **Pop-up Kasir & Hitung Kembalian Otomatis**
   - Klik tombol **"PROSES BAYAR (KASIR)"**.
   - Menampilkan total tagihan belanjaan + teks terbilang.
   - Masukkan uang yang diberikan oleh pembeli (bisa ketik angka atau klik tombol pecahan cepat: *Uang Pas*, *Rp 2.000*, *Rp 5.000*, *Rp 10.000*, *Rp 20.000*, *Rp 50.000*).
   - **Nominal Kembalian dihitung langsung secara real-time**:
     - Warna **Biru**: Ada uang kembalian yang harus diberikan kepada pembeli (disertai teks terbilang).
     - Warna **Hijau**: Uang pas.
     - Warna **Merah & Berkedip**: Uang pembeli masih kurang.
   - Opsional: Bisa diisikan nama pembeli (misal: *Bu Guru Ani* / *Rian 3B*).

5. **Struk Belanja & Cetak Nota**
   - Efek perayaan suara kasir & animasi *confetti* saat transaksi berhasil.
   - Tampilan visual nota struk belanja yang rapi dan bisa dicetak (*Print*) ke printer nota atau kertas standar.

6. **Kalkulator Manual Terintegrasi**
   - Tombol **"Kalkulator"** di header untuk membuka kalkulator cepat langsung di dalam aplikasi.
   - Tidak perlu lagi membuka aplikasi kalkulator terpisah di HP atau komputer.
   - Mendukung klik mouse, layar sentuh, dan tombol keyboard fisik angka (`0-9`, `+`, `-`, `*`, `/`, `Enter`, `Backspace`, `C`).

7. **Efek Suara Kasir Ramah Anak (Web Audio API)**
   - Bunyi *beep* kasir saat klik menu dan bunyi *chime* saat transaksi selesai (bisa dimatikan dengan tombol ikon speaker di pojok kanan atas).
   - Menggunakan Web Audio API murni sehingga tidak membutuhkan file suara eksternal.

---

## 🚀 Cara Menjalankan

1. Cukup buka file **`index.html`** di browser apa saja:
   - **Google Chrome**
   - **Microsoft Edge**
   - **Mozilla Firefox**
   - Atau browser di **Tablet / iPad / HP Android**
2. Tidak perlu instalasi Node.js, PHP, ataupun database.
3. Langsung siap dipakai untuk jualan di acara Market Day!
