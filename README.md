# Website Profil Usaha Mie Ayam & Bakso Sakti

Website profil bisnis kuliner statis untuk menampilkan informasi usaha warung mie ayam, daftar menu dan harga, galeri foto dengan lightbox, jam operasional, lokasi Google Maps, serta pemesanan langsung melalui WhatsApp.

## Fitur Utama

- **Navigasi Sticky & Responsif**: Indikator bagian aktif otomatis saat digulir serta menu mobile (hamburger).
- **Hero & Keunggulan Usaha**: Tampilan editorial modern dengan foto produk utama dan 4 kartu keunggulan.
- **Tentang Kami**: Cerita usaha dilengkapi foto warung dan ringkasan layanan.
- **Menu Pilihan Kami**: Daftar menu mie ayam (Original, Bakso, Ceker, Spesial) serta menu pendamping lainnya dengan tombol pesan langsung ke WhatsApp.
- **Galeri Foto & Lightbox**: Grid asimetris dengan modal lightbox (mendukung tombol `Escape`, `ArrowLeft`, `ArrowRight`, dan klik area luar).
- **Lokasi, Jam Operasional & Pesan Cepat**: Informasi lengkap usaha, tautan Google Maps, dan formulir pembuat pesan WhatsApp otomatis.

## Cara Mengubah Data Usaha

Seluruh informasi usaha terpusat pada satu file:

- `src/data/businessConfig.ts`

Anda dapat dengan mudah mengubah:
- Nama usaha, monogram, dan deskripsi singkat
- Alamat lengkap dan tautan Google Maps
- Nomor WhatsApp (`whatsappNumber` dan `whatsappDisplay`)
- Jam operasional dan hari buka
- Daftar menu, harga, deskripsi, dan foto produk
- Foto galeri

## Menjalankan di Komputer Lokal

```bash
npm install
npm run dev
```

Aplikasi akan berjalan di `http://localhost:3000`.

## Build Produksi

```bash
npm run build
```

Hasil build statis tersimpan di folder `dist/`.

## Deploy ke Vercel

Proyek ini adalah aplikasi frontend statis tanpa database, tanpa server backend, dan tanpa API key:

1. Unggah seluruh proyek ke repository GitHub.
2. Buka [Vercel](https://vercel.com) dan pilih **Add New Project**.
3. Import repository GitHub Anda.
4. Vercel otomatis mendeteksi preset **Vite** (`Build Command: npm run build`, `Output Directory: dist`) berdasarkan `vercel.json`.
5. Klik **Deploy**.
