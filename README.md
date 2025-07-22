# 📘 User Manual – Aplikasi Inventori Bengkel Motor
## 1. Deskripsi Program
Aplikasi ini adalah program berbasis Python yang digunakan untuk mengelola data sparepart bengkel motor secara efisien. Pengguna dapat menambahkan, melihat, mengedit, menghapus, dan menampilkan laporan stok sparepart.
Semua data disimpan secara permanen ke dalam file inventori_bengkel.json.

## 2. Persyaratan Sistem
Python versi 3.6 atau lebih tinggi

Dapat dijalankan melalui:

VS Code / Terminal (Windows/Linux/macOS)

Google Colab

## 3. Struktur File
Nama File	Keterangan
bengkel_motor.py	File utama berisi seluruh kode program
inventori_bengkel.json	File tempat penyimpanan data sparepart
user_manual.md	File dokumentasi penggunaan program

## 4. Cara Menjalankan Program
🔹 Di VS Code / Terminal

Pastikan Python sudah terinstall.

Buka terminal atau command prompt.

Jalankan perintah berikut:

bash
Salin
Edit
python bengkel_motor.py
🔹 Di Google Colab

Upload file bengkel_motor.py.

Jalankan sel yang berisi kode.

File inventori_bengkel.json akan dibuat otomatis di direktori kerja.

## 5. Panduan Menu Program
Saat program dijalankan, pengguna akan melihat menu berikut:

markdown
Salin
Edit
=== Menu Inventori Bengkel Motor ===
1. Tambah Sparepart
2. Lihat Semua Sparepart
3. Edit Stok Sparepart
4. Hapus Sparepart
5. Laporan Stok
6. Simpan & Keluar
No	Menu	Deskripsi
1	Tambah Sparepart	Menambahkan sparepart baru (kode, nama, stok). Kode harus unik.
2	Lihat Semua Sparepart	Menampilkan seluruh daftar sparepart dan stoknya.
3	Edit Stok Sparepart	Mengubah jumlah stok berdasarkan kode sparepart.
4	Hapus Sparepart	Menghapus sparepart berdasarkan kode.
5	Laporan Stok	Menampilkan laporan stok dari jumlah terbanyak ke terkecil.
6	Simpan & Keluar	Menyimpan data ke file JSON dan keluar dari program.

## 6. Format Input
Field	Format	Contoh
Kode Sparepart	String tanpa spasi	SPR001
Nama Sparepart	String bebas	Busi Motor
Jumlah Stok	Angka bulat positif (int)	50

## 7. Fitur Optimasi & Penanganan Error
✅ File Handling menggunakan with open dan error handling dengan try-except
✅ Pengukuran performa menggunakan time.time() untuk analisis kecepatan fungsi
✅ Komentar kode lengkap agar mudah dipahami dan dikembangkan
✅ Validasi kode sparepart unik saat menambah data
✅ Struktur data fleksibel menggunakan list of dictionary
✅ Data tetap aman walau file JSON belum tersedia sebelumnya

## 8. Catatan Tambahan
File inventori_bengkel.json akan otomatis diperbarui saat memilih menu Simpan & Keluar.

Jangan mengedit file JSON secara manual untuk menghindari kerusakan data.

Jika file belum ada, maka program akan otomatis memulai dari data kosong.

Gunakan format kode sparepart konsisten, misalnya: SPR001, SPR002, dll.

💡 Saran Pengembangan (Opsional)
Gunakan struktur dictionary dengan indexing kode sparepart untuk akses lebih cepat (O(1)).

Tambahkan validasi agar input stok harus bernilai positif.

Buat fitur ekspor laporan stok ke file .txt atau .csv.

Tambahkan kategori sparepart, seperti: kelistrikan, mesin, rem, dll.
