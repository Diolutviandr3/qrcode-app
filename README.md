# QR Dipo 📱✨

**QR Dipo** adalah aplikasi Flutter modern yang menggabungkan fitur **Pembuatan (Generator) QR Code** dan **Pemindaian (Scanner) QR Code** secara langsung (real-time) ke dalam satu aplikasi yang elegan dan interaktif.

Aplikasi ini dirancang dengan estetika modern menggunakan tema gelap Slate premium, aksen gradasi biru muda dan biru gelap, serta animasi transisi yang mulus untuk memberikan pengalaman pengguna yang luar biasa.

---

## ✨ Fitur Utama

- **🎨 Desain Premium & Elegan**: Menggunakan tema gelap modern dengan palet warna Slate (`#0F172A`) dan gradasi aksen biru dinamis (`#38BDF8` hingga `#2563EB`).
- **⚡ Pembuat QR Code Instan (Real-time)**: Kode QR dibuat secara langsung saat pengguna mengetik teks atau menempelkan tautan (URL) di kolom input, lengkap dengan animasi transisi memantul yang halus.
- **📸 Pemindai QR Responsif**:
  - Integrasi kamera pemindai live menggunakan `mobile_scanner`.
  - Animasi garis laser pemindai neon biru yang bergerak naik-turun.
  - Bingkai bidik (viewfinder) bergaya HUD modern dengan braket sudut kustom (`CustomPainter`).
  - Pengendali lampu kilat (flash/torch) dan tombol peralihan kamera depan/belakang.
- **🛡️ Penanganan Izin Kamera yang Ramah**: Jika izin kamera dinonaktifkan di ponsel, aplikasi akan menampilkan panduan instruksi visual yang ramah agar pengguna dapat mengaktifkannya di pengaturan.
- **🔄 Navigasi Beranimasi**: Beralih antar tab menggunakan animasi slide & fade yang mulus dan mempertahankan input data sebelumnya.
- **📋 Salin Satu Kali Klik**: Tombol salin hasil pindaian atau data QR langsung ke clipboard dengan notifikasi Snackbar yang informatif.

---

## 🛠️ Pustaka & Teknologi yang Digunakan

Aplikasi ini dibangun menggunakan teknologi terbaru:
- **Flutter SDK**: `v3.41.6` (Dart `v3.11.4`)
- **qr_flutter**: `^4.1.0` (Untuk menjabarkan data teks ke gambar QR)
- **mobile_scanner**: `^3.2.0` (Untuk mendeteksi QR Code melalui kamera ponsel)

---

## 🚀 Cara Memulai & Instalasi

### 1. Prasyarat
Pastikan Anda telah menginstal Flutter SDK di komputer Anda. Cek kesiapan lingkungan dengan menjalankan:
```bash
flutter doctor
```

### 2. Kloning dan Masuk ke Proyek
Buka terminal dan navigasikan ke direktori proyek Anda:
```bash
cd c:\FlutterProjects\qrcode-app
```

### 3. Ambil Dependencies
Unduh pustaka yang diperlukan untuk proyek ini:
```bash
flutter pub get
```

### 4. Jalankan Aplikasi
Hubungkan ponsel fisik (dengan mode debugging aktif) atau aktifkan emulator, lalu jalankan perintah:
```bash
flutter run
```

### 5. Kompilasi APK (Android)
Untuk membuat file instalasi APK Debug, jalankan perintah:
```bash
flutter build apk --debug
```
Hasil file APK dapat ditemukan di direktori:
`build/app/outputs/flutter-apk/app-debug.apk`

---

## ⚙️ Konfigurasi Penting Platform

### Android
Aplikasi ini memerlukan SDK minimal versi 21 dan izin kamera. Konfigurasi ini sudah diterapkan pada berkas berikut:
1. **Izin Kamera** di `android/app/src/main/AndroidManifest.xml`:
   ```xml
   <uses-permission android:name="android.permission.CAMERA" />
   ```
2. **Min SDK 21** di `android/app/build.gradle.kts`:
   ```kotlin
   defaultConfig {
       minSdk = 21
   }
   ```

---

## 📜 Hak Cipta
© 2026 **Dipo Corp**. Hak Cipta Dilindungi.