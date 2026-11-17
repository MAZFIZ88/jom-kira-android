# Jom Kira! V6 — Android APK Build Ready

Projek Android Java WebView yang membungkus permainan Jom Kira! V5 untuk dimainkan secara luar talian.

## Bina APK melalui GitHub Actions menggunakan telefon Android

1. Cipta **repositori GitHub baharu**, contohnya `jom-kira-android` (berasingan daripada repo GitHub Pages).
2. Ekstrak ZIP ini di telefon. Muat naik **semua fail dan folder** ke root repo, termasuk folder tersembunyi `.github/workflows/`. Jangan upload ZIP sahaja.
3. Pergi ke tab **Actions** > **Bina APK Jom Kira** > **Run workflow** (atau tunggu workflow berjalan automatik selepas push ke `main`).
4. Apabila tanda hijau dipaparkan, buka run tersebut > **Artifacts** > **JomKira-V6-Android-APK**. Muat turun ZIP artifact.
5. Ekstrak ZIP artifact, kemudian cari `app-debug.apk` dan pasang pada telefon Android. Android mungkin meminta kebenaran *Install unknown apps* untuk aplikasi yang membuka APK. Pasang hanya APK daripada workflow repositori anda sendiri.

**Penting:** GitHub Actions perlu diaktifkan untuk repositori. Memuat naik folder `.github` dari sesetengah aplikasi pengurus fail boleh menyembunyikan folder bertitik; pastikan ia benar-benar wujud dalam GitHub. GitHub web UI di telefon mungkin lebih mudah melalui pilihan 'Desktop site'.

## Status dan had

- Fail ini ialah **projek sedia bina**, **bukan APK yang telah diuji atau dibina**.
- Aplikasi menggunakan fail HTML V5 yang dibungkus secara setempat; tidak perlu hosting untuk bermain.
- Rekod dalam localStorage kekal pada peranti/aplikasi sahaja; **tiada penyegerakan awan aktif**.
- Permainan mini mengikut implementasi V5 asal; bukan permainan 3D penuh.
- Semak kandungan soalan terhadap DSKP KSSR Tahun 2 sebelum penggunaan rasmi.
- APK yang dijana ialah **debug APK**, sesuai untuk ujian peribadi; bukan pakej keluaran Play Store.
- Jika ingin terbitkan ke Play Store, perlu migrasi target SDK, konfigurasi release signing dan ujian keselamatan/keserasian.
