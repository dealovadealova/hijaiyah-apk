# Cara membuat APK tanpa install apa-apa di laptop (pakai GitHub)

GitHub akan membuatkan APK di server mereka. Laptop Anda hanya dipakai untuk membuka website.

## Langkah
1. Buat akun gratis di https://github.com (lewati jika sudah punya).
2. Klik **+ > New repository**. Beri nama `hijaiyah-apk`, pilih **Public**, lalu klik **Create repository**.
3. Di halaman repository, klik **uploading an existing file**.
4. Buka folder `hijaiyah-apk` dari zip ini, lalu **pilih semua isinya** (termasuk folder `.github`, `android`, `www`, dan file `package.json`) dan tarik ke halaman GitHub.
   - Jika tidak muncul folder `.github`, itu wajar karena nama diawali titik. Tetap pilih semuanya, atau lihat catatan di bawah.
   - Jika upload dibatasi jumlah file, lakukan dalam beberapa kali.
5. Klik **Commit changes**.
6. Buka tab **Actions** di repository. Tunggu workflow **Build APK** sampai ada tanda centang hijau (sekitar 5–10 menit).
7. Klik workflow tersebut, lalu di bagian **Artifacts** unduh **cocokkan-huruf-hijaiyah-apk**. Unzip, dan di dalamnya ada `app-debug.apk`.
8. Kirim file APK ke HP, lalu install. Izinkan "Install dari sumber tidak dikenal" jika diminta.

## Kalau game diubah
Ganti file `www/index.html` di repository (klik file > ikon pensil > Commit), lalu workflow otomatis berjalan lagi dan APK baru bisa diunduh.

## Catatan
- Ini APK debug, cukup untuk dipakai sendiri dan dibagikan ke keluarga.
- Untuk Play Store perlu APK rilis yang ditandatangani, bisa dibantu nanti.
