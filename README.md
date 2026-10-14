# 🌊 WebGIS Hotspot Pengawasan Dit. PSDKP

Aplikasi *Web Geographic Information System* (WebGIS) interaktif yang dirancang untuk memvisualisasikan, memantau, dan menganalisis titik-titik hotspot pengawasan serta indikasi pelanggaran pelaku usaha di bawah wilayah kerja Direktorat Pengawasan Sumber Daya Kelautan (Dit. PSDK).

---

## ✨ Fitur Utama

- **🗺️ Multi-BaseMap Terintegrasi:** Mendukung berbagai pilihan tampilan peta dasar (*Esri Dark, Satellite, OpenStreetMap, Light, dan Topografi*).
- **🔥 Heatmap Kepadatan Wilayah:** Visualisasi konsentrasi titik pelanggaran berbasis gradasi warna (Rendah, Sedang, Tinggi) dengan efek *solid blur* dinamis yang menyesuaikan tingkat *zoom*.
- **📍 Klasterisasi Titik (*Marker Cluster*):** Pengelompokan titik secara otomatis untuk menjaga performa peta tetap ringan dan mudah dibaca pada tingkat skala nasional.
- **🏢 Batas Wilayah UPT & Garis Pantai:** Integrasi data spasial GeoJSON untuk menampilkan wilayah kerja UPT PSDKP (Stasiun & Pangkalan) serta Garis Pantai Indonesia.
- **🔍 Pencarian & Filter Komprehensif:** 
  - Pencarian real-time berdasarkan nama pelaku usaha, lokasi, atau indikasi pelanggaran.
  - Filter berdasarkan UPT PSDKP penanggung jawab.
  - Filter status pengawasan (*Sudah diawasi* vs *Belum diawasi*).
- **📱 Desain Responsif & Modern:** Antarmuka berbasis *Dark Theme* menggunakan *Plus Jakarta Sans*, dirancang optimal untuk layar *desktop* maupun perangkat *mobile*.

---

## 📁 Struktur Berkas Proyek

Proyek ini telah dipisahkan menjadi beberapa modul modular agar bersih dan mudah dikelola:

```text
├── index.html                  # Struktur utama halaman antarmuka WebGIS
├── style.css                   # Berkas penataan gaya, tema gelap, dan responsivitas UI
├── script.js                   # Logika utama aplikasi, interaksi peta, dan manajemen filter
├── data.js                     # Berkas basis data terpusat (Array objek JSON titik hotspot & perusahaan)
├── garpan_web_simplified_05.geojson # Berkas spasial GeoJSON Garis Pantai Indonesia
└── upt_psdkp_web.geojson       # Berkas spasial GeoJSON wilayah kerja UPT PSDKP
