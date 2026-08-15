# Digital Absensi Gprojectapp - Android V4

Perbaikan Voice Absen:
- Menggunakan Android native SpeechRecognizer melalui JavaScript bridge.
- Tidak lagi bergantung pada Web Speech API browser yang sering menghasilkan `not-allowed` pada file HTML lokal/WebView.
- Meminta izin RECORD_AUDIO.
- Bahasa Indonesia `id-ID`.
- Hasil suara dikirim ke HTML dan otomatis diproses sebagai Hadir.
- Tombol Stop menghentikan pengenalan suara.

PENTING:
Jangan mengetes Voice Absen dengan membuka file HTML dari folder Download/browser. Fitur native hanya berjalan setelah project ini dibuild menjadi APK dan aplikasi APK dibuka.

Build:
1. Buka folder project ini di Android Studio.
2. Sync Gradle.
3. Build > Build APK(s).
4. Install APK di HP.
5. Saat pertama kali menekan Voice Absen, pilih Izinkan untuk mikrofon.
