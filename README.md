# Generator QR Code Modern

![Lisensi MIT](https://img.shields.io/badge/License-MIT-blue.svg)

Sebuah aplikasi web front-end yang simpel, modern, dan indah untuk membuat QR Code. Proyek ini dibuat untuk mendemonstrasikan penggunaan teknologi front-end modern seperti Tailwind CSS dan Alpine.js untuk menciptakan antarmuka pengguna yang fungsional dan estetis.

Aplikasi ini memungkinkan pengguna untuk mengubah teks atau URL apa pun menjadi QR Code yang dapat diunduh, dengan kustomisasi visual seperti sudut membulat dan efek timbul.

### Tampilan Aplikasi
![Tampilan Aplikasi Generator QR Code](https://i.imgur.com/uU2wT8I.png)

---

## ✨ Fitur Utama

- **Generasi QR Code Instan**: QR Code dibuat langsung di sisi klien (browser) tanpa perlu menunggu respon dari server.
- **Desain Modern & Responsif**: Menggunakan efek *glassmorphism* (latar belakang blur transparan) dengan warna gradien yang elegan. Tampilan optimal di berbagai ukuran layar, dari desktop hingga mobile.
- **Kustomisasi Tampilan QR Code**:
  - Titik dan sudut QR Code dibuat membulat (*rounded*) untuk tampilan yang lebih lembut.
  - Efek timbul (*emboss*) dengan bayangan halus untuk memberikan kesan 3D.
  - Border putih tebal yang jelas di sekeliling QR Code.
- **Fitur Unduh**: Pengguna dapat mengunduh QR Code yang telah dibuat sebagai file gambar `.png`.
- **Slider Interaktif**: Terdapat komponen slider (dibuat dengan Swiper.js) untuk menampilkan fitur-fitur unggulan aplikasi.
- **Ringan & Cepat**: Tidak memerlukan proses *build* atau instalasi dependensi yang rumit. Semua aset dimuat melalui CDN.

---

## 🛠️ Teknologi yang Digunakan

Proyek ini dibangun menggunakan kombinasi framework dan library modern:

- **Struktur**: HTML5
- **Styling**: **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS framework untuk desain kustom yang cepat.
- **Interaktivitas & State Management**: **[Alpine.js](https://alpinejs.dev/)** - Framework JavaScript yang ringan dan deklaratif untuk menambahkan perilaku dinamis pada markup.
- **Engine Generator QR Code**: **[QR-Code-Styling](https://github.com/kozakdenys/qr-code-styling)** - Library canggih untuk membuat dan menata tampilan QR Code dengan berbagai opsi kustomisasi.
- **Slider/Carousel**: **[Swiper.js](https://swiperjs.com/)** - Library slider sentuh yang modern dan powerful.
- **Font**: **[Google Fonts (Poppins)](https://fonts.google.com/specimen/Poppins)**

---

## 🚀 Cara Menjalankan

Proyek ini sangat mudah untuk dijalankan karena tidak memerlukan server atau proses kompilasi.

1.  **Clone repository ini:**
    ```bash
    git clone [https://github.com/NAMA-USERNAME-ANDA/NAMA-REPO-ANDA.git](https://github.com/NAMA-USERNAME-ANDA/NAMA-REPO-ANDA.git)
    ```

2.  **Masuk ke direktori proyek:**
    ```bash
    cd NAMA-REPO-ANDA
    ```

3.  **Buka file `index.html`:**
    Cukup buka file `index.html` di browser favorit Anda (misalnya Google Chrome, Firefox, atau Edge).

Selesai! Aplikasi akan langsung berjalan.

---

## 📂 Struktur Kode

Seluruh kode proyek ini terdapat dalam satu file, yaitu `index.html`.

- **`<head>`**: Bagian ini berisi semua tautan CDN ke library yang dibutuhkan (Tailwind, Alpine, Swiper, QR-Code-Styling) dan Google Fonts.
- **`<style>`**: Berisi beberapa CSS kustom untuk memberikan efek timbul (*box-shadow*) pada canvas QR Code dan menata *placeholder*.
- **`<body>`**: Berisi seluruh struktur layout yang dibangun dengan kelas-kelas utilitas dari Tailwind CSS.
- **`<script>`**:
  - **Logika Alpine.js**: Ditandai dengan `x-data="qrGenerator()"`. Di sinilah semua state (seperti teks input) dan fungsi (seperti `generate()` dan `download()`) dikelola.
  - **Inisialisasi Swiper.js**: Script singkat untuk mengaktifkan komponen slider.
  - **Inisialisasi QR-Code-Styling**: Instance QR Code dibuat di dalam fungsi `generate()` dengan berbagai opsi konfigurasi (`dotsOptions`, `cornersSquareOptions`) untuk mendapatkan tampilan yang diinginkan.

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah **Lisensi MIT**. Lihat file `LICENSE` untuk detail lebih lanjut.
