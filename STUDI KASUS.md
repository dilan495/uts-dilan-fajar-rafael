# 📚 Studi Kasus: Sistem Data Pembayaran Sederhana

## 🎯 Latar Belakang

Dalam dunia digital saat ini, pencatatan pembayaran secara manual sangat tidak efisien. Banyak organisasi atau instansi memerlukan sistem yang mampu mencatat, mengelola, dan melacak pembayaran dari pelanggan secara terstruktur. Oleh karena itu, dibutuhkan sistem **Data Pembayaran** sederhana yang mampu menangani hal tersebut secara otomatis, cepat, dan akurat.

---

## 🧩 Tujuan Sistem

Membangun aplikasi manajemen pembayaran menggunakan Laravel 12 dan Filament Admin Panel yang dapat:

- Mencatat data pelanggan.
- Mencatat detail pembayaran beserta metode yang digunakan.
- Menampilkan statistik pembayaran secara visual (grafik).
- Menerapkan konsep struktur data seperti Array, Stack, Queue, Tree, dan Graph dalam studi sistem.

---

## 🏛️ Struktur Database

Sistem ini hanya memiliki 3 tabel utama:

1. **customers** – Menyimpan data pelanggan.
2. **payment_methods** – Menyimpan jenis metode pembayaran (cash, transfer, e-wallet, dll).
3. **payments** – Menyimpan data pembayaran yang dilakukan oleh pelanggan.

Relasi:

- `payments` memiliki relasi **belongsTo** ke `customers`.
- `payments` memiliki relasi **belongsTo** ke `payment_methods`.
- `customers` dan `payment_methods` memiliki relasi **hasMany** ke `payments`.

---

## 🧠 Analisis Struktur Data

| Struktur Data | Implementasi dalam Sistem |
|---------------|---------------------------|
| **Array**     | Menyimpan list metode pembayaran di dropdown form. |
| **Stack**     | Log aktivitas terakhir dimasukkan ke dalam array stack. |
| **Queue**     | Antrian verifikasi pembayaran jika sistem online. |
| **Tree**      | Hirarki laporan bulanan → mingguan → harian. |
| **Graph**     | Koneksi antar customer dan pembayaran (jika dihubungkan sebagai node). |

---

## 🔍 Fitur Pencarian

Sistem ini menyediakan fitur pencarian data pelanggan dan riwayat pembayaran berdasarkan:

- Nama pelanggan
- Nomor referensi pembayaran
- Tanggal pembayaran
- Metode pembayaran

---

## 📊 Visualisasi Data

Disediakan Widget seperti **PaymentChart** di dashboard untuk menampilkan statistik jumlah pembayaran per metode atau per bulan.

---

## ✅ Teknologi Digunakan

- Laravel 12
- Filament v3
- MySQL/MariaDB
- PHP 8.3+
- TailwindCSS (dari Filament)
- Eloquent ORM

---

## 💡 Kesimpulan

Sistem ini cocok digunakan sebagai pembelajaran implementasi struktur data dalam dunia nyata. Meski sederhana, namun sudah mampu merepresentasikan proses bisnis dengan pendekatan MVC serta penerapan konsep-konsep penting dalam struktur data.

