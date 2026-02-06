# Privacy Policy / Kebijakan Privasi

**FTTH Schematic Topology**  
*Terakhir diperbarui / Last updated: Februari 2026*

---

# BAHASA INDONESIA

## 1. Ringkasan

Aplikasi **FTTH Schematic Topology** tidak memerlukan **registrasi**, **akun**, atau **login**. Semua data Anda disimpan **hanya di perangkat** Anda. Tidak ada data yang dikirim ke server kami (aplikasi ini tidak memiliki server backend).

## 2. Cara Aplikasi Berjalan (Khususnya di Android)

### 2.1 Tanpa Registrasi dan Tanpa Akun

- Aplikasi **tidak memiliki fitur daftar, masuk, atau keluar**.
- Tidak ada email, nomor telepon, atau kata sandi yang diminta.
- Anda langsung menggunakan aplikasi setelah membukanya.

### 2.2 Penyimpanan Data (Hanya di Perangkat)

- **Data yang Anda buat** (asset jaringan, kabel, koordinat, nama, catatan) disimpan **hanya di penyimpanan lokal** perangkat:
  - **Di browser (PC):** menggunakan **localStorage** browser.
  - **Di Android (APK):** menggunakan penyimpanan **WebView** (setara localStorage) yang **hanya dapat diakses oleh aplikasi ini**.
- Data **tidak** dikirim ke cloud, server, atau pihak ketiga untuk disimpan.
- Hanya perangkat Anda yang menyimpan data. Jika Anda menghapus data aplikasi atau uninstall, data tersebut hilang dari perangkat.

### 2.3 Akses Jaringan (Internet)

Aplikasi membutuhkan internet **hanya** untuk:

| Tujuan | Layanan | Data yang dikirim | Keterangan |
|--------|---------|-------------------|------------|
| Menampilkan peta | OpenStreetMap (tile) | Alamat IP, zoom level, koordinat area peta | Standar untuk menampilkan peta; tidak berisi data asset Anda |
| Routing "Ikuti Jalan" | OSRM (router.project-osrm.org) | Hanya koordinat titik awal dan akhir (2 pasang lat/lng) | Hanya saat Anda memilih "Ikuti Jalan" dan membuat kabel; tidak ada nama atau identitas |
| Memuat library (CSS/JS) | unpkg.com, cdnjs.cloudflare.com | Permintaan unduh file statis | Tidak berisi data pribadi atau data jaringan Anda |

Tidak ada data **nama asset, pelanggan, atau catatan** Anda yang dikirim ke server manapun.

### 2.4 Lokasi (GPS)

- **GPS digunakan hanya jika Anda menekan tombol** untuk mengambil lokasi (misalnya "Ambil dari GPS" atau ikon lokasi).
- Aplikasi **tidak** merekam atau melacak lokasi Anda secara terus-menerus.
- Koordinat yang diambil **hanya dipakai di perangkat** (misalnya untuk mengisi form tambah asset) dan disimpan di penyimpanan lokal seperti dijelaskan di atas.
- Di Android, izin lokasi ditanyakan oleh sistem; Anda bisa menolak dan tetap menggunakan aplikasi (tanpa fitur isi-otomatis koordinat dari GPS).

### 2.5 Export dan Import KML

- **Export KML:** Aplikasi membuat file KML dari data yang ada di perangkat dan menawarkan **unduh** ke perangkat Anda. File tidak di-upload ke server kami (tidak ada server).
- **Import KML:** File KML yang Anda pilih **hanya dibaca di perangkat** dan datanya dimasukkan ke penyimpanan lokal. Tidak ada upload ke server.

## 3. Data yang Tidak Dikumpulkan

Aplikasi **tidak**:

- Membuat atau mengelola akun pengguna.
- Mengumpulkan nama, email, nomor telepon, atau data profil.
- Mengirim data asset atau data jaringan Anda ke server kami atau pihak lain untuk disimpan atau dianalisis.
- Melacak lokasi secara diam-diam atau berkelanjutan.

## 4. Pihak Ketiga

- **OpenStreetMap** (peta): Kebijakan privasi mereka berlaku untuk penggunaan tile peta.
- **OSRM** (routing): Hanya menerima koordinat untuk menghitung rute; tidak menyimpan data Anda secara permanen untuk keperluan kami.
- **unpkg / Cloudflare (cdnjs):** Penyedia file statis (CSS/JS); tidak menerima data jaringan atau data pribadi Anda.

Kami tidak mengontrol kebijakan privasi pihak ketiga tersebut. Penggunaan aplikasi berarti Anda juga menerima penggunaan layanan mereka sesuai kebijakan masing-masing.

## 5. Keamanan Data

- Data Anda **hanya berada di perangkat** Anda (dan di backup/export yang Anda buat sendiri, misalnya file KML).
- Kami tidak memiliki akses ke data yang disimpan di perangkat atau di file yang Anda export.
- Disarankan untuk secara berkala **Export KML** sebagai cadangan, karena penghapusan aplikasi atau data aplikasi akan menghapus data dari perangkat.

## 6. Perubahan Kebijakan

Perubahan kebijakan privasi akan dicantumkan di dokumen ini dengan memperbarui tanggal "Terakhir diperbarui". Penggunaan aplikasi setelah perubahan berarti penerimaan terhadap kebijakan yang diperbarui.

## 7. Kontak

Untuk pertanyaan tentang privasi aplikasi ini:  
**Support by Saputra Budi**

---

# ENGLISH

## 1. Summary

The **FTTH Schematic Topology** application does **not** require **registration**, **account**, or **login**. All your data is stored **only on your device**. No data is sent to our servers (this application has no backend server).

## 2. How the Application Works (In Particular on Android)

### 2.1 No Registration and No Account

- The app **does not have sign-up, sign-in, or sign-out**.
- No email, phone number, or password is ever requested.
- You use the app as soon as you open it.

### 2.2 Data Storage (On-Device Only)

- **Data you create** (network assets, cables, coordinates, names, notes) is stored **only in local storage** on the device:
  - **In a browser (PC):** using the browser’s **localStorage**.
  - **On Android (APK):** using **WebView** storage (equivalent to localStorage) that **only this app can access**.
- Data is **not** sent to any cloud, server, or third party for storage.
- Only your device holds the data. If you clear the app’s data or uninstall the app, that data is removed from the device.

### 2.3 Network (Internet) Access

The app uses the internet **only** for:

| Purpose | Service | Data sent | Notes |
|--------|---------|-----------|--------|
| Showing the map | OpenStreetMap (tiles) | IP address, zoom level, map area coordinates | Standard for map display; does not include your asset data |
| “Follow road” routing | OSRM (router.project-osrm.org) | Only start and end coordinates (2 lat/lng pairs) | Only when you choose “Ikuti Jalan” and create a cable; no names or identity |
| Loading libraries (CSS/JS) | unpkg.com, cdnjs.cloudflare.com | Requests for static files | No personal or network data |

No **asset names, customer names, or notes** are sent to any server.

### 2.4 Location (GPS)

- **GPS is used only when you press a button** to get your location (e.g. “Ambil dari GPS” or the location icon).
- The app **does not** record or track your location in the background.
- Coordinates are **used only on the device** (e.g. to fill the “add asset” form) and stored in local storage as described above.
- On Android, location permission is requested by the system; you can deny it and still use the app (without auto-filling coordinates from GPS).

### 2.5 KML Export and Import

- **Export KML:** The app generates a KML file from data on the device and offers a **download** to your device. The file is not uploaded to our servers (we have no server).
- **Import KML:** The KML file you select is **read only on the device** and its data is added to local storage. No upload to any server occurs.

## 3. Data We Do Not Collect

The app **does not**:

- Create or manage user accounts.
- Collect name, email, phone number, or profile data.
- Send your asset or network data to our servers or any other party for storage or analysis.
- Track your location in the background or continuously.

## 4. Third Parties

- **OpenStreetMap** (map): Their privacy policy applies to use of map tiles.
- **OSRM** (routing): Receives only coordinates to compute a route; does not store your data for our purposes.
- **unpkg / Cloudflare (cdnjs):** Provide static files (CSS/JS); they do not receive your network or personal data.

We do not control these third parties’ privacy policies. Using the app means you also accept use of their services in line with their respective policies.

## 5. Data Security

- Your data **exists only on your device** (and in any backup/export you make yourself, e.g. KML files).
- We do not have access to data stored on your device or to files you export.
- We recommend that you **export KML** periodically as a backup, since clearing or uninstalling the app will remove data from the device.

## 6. Changes to This Policy

Any changes to this privacy policy will be reflected in this document with an updated “Last updated” date. Continued use of the app after changes constitutes acceptance of the updated policy.

## 7. Contact

For questions about this app’s privacy practices:  
**Support by Saputra Budi**

---

*FTTH Schematic Topology – Privacy Policy v1.0*
