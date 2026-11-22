# Domino Tactical Assistant — Android APK

Prototipe Android offline berbasis WebView, berisi versi HTML yang telah diuji pengguna. Tidak membutuhkan izin internet.

## Membuat APK lewat GitHub Actions (HP atau PC)
1. Ekstrak ZIP ini di HP, pertahankan semua folder termasuk folder tersembunyi `.github`.
2. Buat repository GitHub baru, misalnya `domino-tactical-android` (Private boleh).
3. Di halaman repo, pilih **Add file > Upload files**, lalu unggah isi folder hasil ekstrak dengan mempertahankan struktur direktori; cara termudah untuk folder bersarang ialah menggunakan github.dev (tekan `.` di repo) atau unggah lewat Git. Folder `.github/workflows` wajib ada di repo.
4. Commit ke branch default. Workflow juga berjalan otomatis pada push.
5. Buka **Actions > Build Android APK**, lalu **Run workflow** bila diperlukan.
6. Sesudah berhasil, buka hasil job terbaru > **Artifacts > domino-tactical-apk**. Download ZIP hasil build lalu ekstrak `app-debug.apk`.
7. Di Android, buka APK untuk memasang. Aktifkan izin pemasangan dari sumber tersebut hanya ketika diperlukan dan dari hasil build milik Anda sendiri.

## Ketentuan
- Android 6.0+ (minSdk 23).
- Mode offline; semua data dicatat di penyimpanan WebView lokal.
- Aturan awal empat pemain, dua ujung; aturan lokal gaple masih perlu penyesuaian.
- Rekomendasi bersifat heuristik, bukan jaminan menang.
- Digunakan pada permainan tanpa taruhan dengan persetujuan peserta.
- Hasil APK belum dibangun atau dites dalam lingkungan ini: GitHub Actions yang akan mengompilasi.
