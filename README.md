# FTTH Schematic Topology - Network Topology Management

## 🚀 Fitur Utama

### 📍 Map View
- Peta interaktif
- Marker clustering untuk performa optimal
- GPS integration untuk lokasi real-time
- Klik marker untuk melihat detail asset

### 📊 Topology View
- Diagram topologi jaringan hierarkis (vis.js)
- Visualisasi koneksi antar equipment
- Toggle layout (hierarchical/force-directed)
- Interactive: klik node untuk detail

### 📋 List View
- Daftar semua asset dengan informasi lengkap
- Status indikator (Active/Maintenance/Inactive)
- Capacity monitoring
- Sorting dan filtering

### ⚙️ Fitur Lengkap
- ✅ **CRUD Operations** - Create, Read, Update, Delete asset
- ✅ **Search & Filter** - Cari berdasarkan nama, tipe, customer
- ✅ **GPS Integration** - Ambil koordinat dari GPS device
- ✅ **KML Export** - Export data ke format KML (Google Earth compatible)
- ✅ **KML Import** - Import existing KML files
- ✅ **localStorage** - Data tersimpan di browser (offline-capable)
- ✅ **Mobile-First Design** - Bottom navigation, responsive
- ✅ **Multiple Asset Types** - ODP, ODC, OLT, FAT, JC, Pole, Customer
- ✅ **Cable Management** - Backbone, Distribution, Drop cable

## 📦 Tipe Asset yang Didukung

| Tipe | Icon | Deskripsi |
|------|------|-----------|
| **OLT** | 🗄️ | Optical Line Terminal (Central Office) |
| **ODC** | 🖥️ | Optical Distribution Cabinet |
| **ODP** | 🟢 | Optical Distribution Point |
| **FAT** | 📦 | Fiber Access Terminal |
| **JC** | 🔗 | Joint Closure (Splicing Point) |
| **Pole** | ⚫ | Utility Pole |
| **Customer** | 🏠 | Customer Premises |
| **Cable** | ➖ | Fiber Optic Cable (Backbone/Distribution/Drop) |

## 🎯 Cara Penggunaan

### 1. Menambah Asset Baru

1. Klik tombol **+** (FAB) di tengah bottom navigation
2. Pilih tipe asset (ODP/ODC/OLT/dll)
3. Isi form:
   - **Nama** (wajib)
   - **Koordinat** (lat/lng) - bisa ambil dari GPS
   - **Kapasitas** (untuk equipment)
   - **Splitter & Ratio** (untuk ODP/ODC)
   - **Pelanggan** (satu nama per baris)
   - **Catatan** tambahan
4. Klik **Simpan**

### 2. Menambah Cable/Connection

**Metode A: Dari Asset Popup**
1. Klik **marker asset** di peta
2. Di popup, klik **"Add Cable"**
3. Pilih routing type:
   - **Garis Lurus** - koneksi langsung point-to-point
   - **Ikuti Jalan** - mengikuti jalur jalan (OSRM routing)
4. Klik **asset tujuan** di peta
5. Jarak **otomatis dihitung**
6. Form cable muncul dengan data pre-filled
7. Isi informasi tambahan (tipe, core, notes)
8. Klik **Simpan**

**Metode B: Manual**
1. Klik tombol **+** (FAB)
2. Pilih tipe **Cable**
3. **Klik 2 marker** di peta untuk memilih endpoint
4. Isi informasi cable:
   - Tipe (Backbone/Distribution/Drop)
   - Core (12/24/48/96/144)
   - Panjang (auto-calculated)
5. Klik **Simpan**

### 3. Edit/Delete Asset

1. Klik asset di **Map** atau **List**
2. Modal detail akan muncul
3. Pilih:
   - **Edit** untuk mengubah data
   - **Delete** untuk menghapus (konfirmasi required)

### 4. Search & Filter

1. Klik icon **🔍** di header
2. Ketik nama asset atau customer
3. Pilih filter:
   - **Semua** - tampilkan semua
   - **ODP** - hanya ODP
   - **ODC** - hanya ODC
   - dll.

### 5. Export KML

1. Klik **☰** menu
2. Pilih **Export KML**
3. File `ftth_network_YYYY-MM-DD.kml` akan terdownload
4. Bisa dibuka di:
   - Google Earth
   - Google Maps
   - QGIS
   - ArcGIS

### 6. Import KML

1. Klik **☰** menu
2. Pilih **Import KML**
3. Pilih file .kml
4. Konfirmasi import
5. Data akan dimuat ke aplikasi

### 7. GPS Features

**Mendapatkan Lokasi Saat Ini:**
1. Klik icon **📍** di header
2. Allow location access
3. Koordinat dan akurasi akan ditampilkan
4. Peta akan pan ke lokasi Anda

**Menggunakan GPS saat Add Asset:**
1. Di form, klik **Ambil dari GPS**
2. Koordinat otomatis terisi

## 💾 Data Storage

- Data disimpan di **localStorage** browser
- **Otomatis tersimpan** setiap kali ada perubahan
- **Offline-capable** - tetap bisa digunakan tanpa internet
- **Manual backup** dengan Export KML

### Kapasitas Storage
- localStorage: ~5-10 MB
- Cukup untuk ribuan asset

### Backup & Restore
1. **Backup**: Export KML secara berkala
2. **Restore**: Import KML saat pindah device

## 📞 Support

Untuk pertanyaan atau bug report, hubungi developer.

## 📝 License

© 2026 - By Saputra Budi

---

**Happy Mapping! 🗺️✨**
