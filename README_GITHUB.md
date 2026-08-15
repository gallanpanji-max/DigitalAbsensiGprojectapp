# Digital Absensi Gprojectapp — Build APK tanpa Android Studio

Paket ini sudah berisi project Android dan workflow GitHub Actions. GitHub akan membangun APK di server cloud, jadi Anda tidak perlu Android Studio di HP/PC.

## Cara paling cepat dari HP

1. Buat akun/login di GitHub.
2. Buat repository baru, misalnya `DigitalAbsensiGprojectapp`.
3. Upload **seluruh isi folder project ini** ke repository (termasuk folder `.github`).
4. Pastikan branch bernama `main`.
5. Buka tab **Actions**.
6. Pilih **Build Digital Absensi APK**.
7. Tekan **Run workflow**.
8. Tunggu sampai status hijau/Success.
9. Buka hasil workflow tersebut, cari bagian **Artifacts**, lalu download `Digital-Absensi-Gprojectapp-APK`.
10. Ekstrak ZIP artifact dan install `app-debug.apk` di HP Android.

Workflow ini menggunakan GitHub Actions untuk menjalankan build Gradle dan menyimpan APK sebagai artifact. GitHub mendokumentasikan workflow sebagai proses otomatis yang disimpan di `.github/workflows`, dan artifact dapat dipakai untuk menyimpan file hasil build. Android Gradle Plugin adalah sistem build resmi Android.

## Catatan Voice Absen

Jangan membuka `index.html` dari browser/file Download untuk mengetes Voice Absen. Voice Absen native aktif setelah APK terpasang. Saat pertama kali menekan **Voice Absen**, izinkan akses mikrofon.
