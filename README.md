# 🗺️ MALANG.HIDDEN

> Peta interaktif untuk mengeksplorasi kafe, restoran, bar, dan tempat-tempat tersembunyi di Malang, Jawa Timur.

![Static Badge](https://img.shields.io/badge/status-live-00ff9d?style=flat-square)
![Static Badge](https://img.shields.io/badge/data-OpenStreetMap-blue?style=flat-square)
![Static Badge](https://img.shields.io/badge/dibuat%20dengan-HTML%20%2F%20CSS%20%2F%20JS-orange?style=flat-square)
![Static Badge](https://img.shields.io/badge/deploy-GitHub%20Pages-181717?style=flat-square&logo=github)

---
- https://agusadhitama.github.io/malang-hidden/
---

## ✨ Fitur

- **Data Langsung** Mengambil data lokasi secara real-time dari OpenStreetMap via Overpass API. Tanpa database.
- **Peta Interaktif** Dibangun dengan Leaflet.js, bertema gelap dengan filter tile cyberpunk. Marker berwarna sesuai kategori.
- **Mode Gelap / Terang** Toggle tema dengan animasi smooth, preferensi tersimpan di localStorage.
- **Filter Kategori** Filter berdasarkan Kafe, Restoran, Bar, Tempat Wisata, atau Taman.
- **Pencarian** Cari nama lokasi dan alamat secara real-time.
- **Panel Detail Lokasi** Klik marker atau kartu untuk melihat koordinat, kategori, info WiFi, jam buka, dan tautan langsung ke Google Maps.
- **Lokasi Saya** Loncat ke posisi GPS kamu saat ini di peta.
- **Pelacak Koordinat** Tampilan lat/lng live saat kursor bergerak di atas peta.
- **Tanpa Backend** Murni static site. Tidak perlu server, database, atau maintenance rutin.

---

## 🖥️ Tampilan

| Mode Gelap | Mode Terang |
|------------|-------------|
| Peta gelap cyberpunk dengan marker bercahaya | Palet krem hangat dengan tile peta natural |

---

## 🚀 Cara Menjalankan

### Jalankan Secara Lokal

```bash
# Clone repositori
git clone https://github.com/agusadhitama/malang-hidden.git

# Buka di browser, tidak perlu proses build
cd malang-hidden
open index.html
```

Atau cukup drag file `index.html` ke browser.

---

## 🛠️ Teknologi yang Digunakan

| Teknologi | Kegunaan |
|-----------|----------|
| HTML / CSS / JS | Inti aplikasi tanpa framework, tanpa build tools |
| [Leaflet.js](https://leafletjs.com/) | Rendering peta interaktif |
| [OpenStreetMap](https://www.openstreetmap.org/) | Penyedia tile peta |
| [Overpass API](https://overpass-api.de/) | Data lokasi langsung untuk wilayah Malang |
| [Google Fonts](https://fonts.google.com/) | Syne (display) + Space Mono (UI) |
| GitHub Pages | Hosting gratis |

---

## 📁 Struktur Proyek

```
malang-hidden/
└── index.html      # Seluruh aplikasi satu file, tanpa instalasi dependency
```

---

## 🗂️ Sumber Data

Semua data lokasi diambil langsung dari **OpenStreetMap** menggunakan Overpass API. Query mencakup area bounding box Malang dan mengambil:

- `amenity = cafe`
- `amenity = restaurant`
- `amenity = bar / pub`
- `tourism = attraction / viewpoint`
- `leisure = park`

Hanya node yang memiliki tag `name` yang ditampilkan. Data diperbarui otomatis seiring kontribusi komunitas OSM.

---

## 🎨 Desain

- **Mode gelap**: Navy/hitam pekat dengan aksen `#00ff9d` estetika terminal cyberpunk
- **Mode terang**: Krem hangat `#f0ede8` dengan aksen `#00915a` bersih dan nyaman dibaca
- **Tipografi**: [Syne](https://fonts.google.com/specimen/Syne) untuk judul + [Space Mono](https://fonts.google.com/specimen/Space+Mono) untuk UI
- **Peta**: Mode gelap menerapkan filter CSS `invert + hue-rotate` pada tile OSM untuk tampilan peta malam

---

## 📌 Rencana Pengembangan

- [ ] Simpan / bookmark lokasi favorit
- [ ] Bagikan lokasi via URL
- [ ] Kirim lokasi tersembunyi baru (via GitHub Issues sebagai backend)
- [ ] Tampilan responsif untuk perangkat mobile
- [ ] Jarak dari lokasi saat ini

---

## 📄 Lisensi

MIT License bebas digunakan, dimodifikasi, dan didistribusikan.

---

<div align="center">

Dibuat dengan teliti oleh **Agus Satria Adhitama**  
Malang, Jawa Timur 🌋

</div>
