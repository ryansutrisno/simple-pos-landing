# Simpel POS Landing Page

Halaman landing (landing page) edukatif dan interaktif untuk memasarkan produk **Simpel POS** – sebuah sistem Point of Sale (POS) yang dirancang khusus untuk mempermudah operasional toko kecil dan UMKM.

Proyek ini dibuat menggunakan kerangka kerja [Astro](https://astro.build) yang super ringan dengan pendekatan Vanilla CSS untuk memastikan performa yang sangat cepat, SEO yang baik, dan kemudahan dalam maintenance.

## 🚀 Fitur Utama

- **Cepat & Ringan:** Dibangun menggunakan Astro tanpa JavaScript framework berat (Zero JS by default) untuk Load Time yang optimal (Core Web Vitals).
- **Responsive Design:** Tampilan fleksibel dan optimal di seluruh ukuran layar (Mobile, Tablet, Desktop) menggunakan CSS Grid dan Flexbox.
- **Interaktif:** Menggunakan video preview ringan yang diputar otomatis (autoplay, muted) untuk memberikan demonstrasi langsung produk kepada calon pelanggan tanpa memberatkan load halaman.
- **SEO Optimized:** Telah dilengkapi dengan meta tag Open Graph (OG), Twitter Cards, struktur semantic HTML, dan JSON-LD Schema (FAQ) yang disukai mesin pencari Google.
- **Komponen Modular:** Basis kode HTML dan CSS dipilah ke dalam sistem komponen (Hero, Fitur, FAQ, dll) untuk mempermudah perawatan (maintenance) dan skalabilitas.

## 📁 Struktur Direktori

```text
/
├── public/                 # Aset statis seperti video, thumbnail Open Graph, favicon
├── src/
│   ├── assets/             # Aset gambar yang dioptimasi oleh Astro
│   ├── components/         # Komponen-komponen penyusun halaman (Hero, Header, Footer, dll)
│   ├── pages/              # Halaman utama routing (contoh: index.astro)
│   ├── styles/             # Global CSS dan reset
│   └── utils/              # Skrip helper dan variabel konstanta (contoh: constants.ts)
└── LANDING_PAGE_DESIGN.md  # Log dokumen keputusan arsitektur dan desain
```

## 🛠️ Panduan Pengembangan (Development)

Pastikan Anda telah menginstal [Node.js](https://nodejs.org/) di sistem Anda.

1. **Instalasi Dependencies:**
   ```bash
   npm install
   ```

2. **Menjalankan Local Server:**
   ```bash
   npm run dev
   ```
   Aplikasi akan berjalan di `http://localhost:4321/`.

3. **Membangun untuk Produksi (Build):**
   ```bash
   npm run build
   ```
   Astro akan meng-compile proyek menjadi file HTML/CSS statis ke dalam direktori `dist/` yang sangat ringan dan siap di-deploy (misalnya ke Netlify, Vercel, Cloudflare Pages, atau hosting manapun).

## 🎨 Konfigurasi SEO & Open Graph

Proyek ini telah dikonfigurasi untuk menampilkan *rich snippet* jika tautannya dibagikan di media sosial (WhatsApp, Facebook, Twitter, LinkedIn).
- Konfigurasi meta tag diletakkan pada komponen *wrapper* di `src/components/Layout.astro`.
- Gambar utama (thumbnail) untuk tautan yang dibagikan telah disambungkan ke file statis `public/Simple-Pos-Thumbnail.png`.

---

© 2026 Dibuat dengan ❤️ oleh [Trazmedia.com](https://trazmedia.com)
