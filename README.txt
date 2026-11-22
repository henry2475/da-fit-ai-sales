DA FIT AI Sales Assistant — Weather Assistant V1.0

Isi:
- index.html: aplikasi cuaca responsif
- manifest.webmanifest: metadata PWA
- sw.js: cache dasar agar app shell dapat dibuka kembali
- icon.svg: ikon aplikasi

Fitur:
- Lokasi awal Koja, Jakarta Utara
- Deteksi GPS melalui browser (izin lokasi diperlukan)
- Pencarian kota/wilayah
- Cuaca saat ini, prakiraan per jam 12 jam, dan prakiraan 3 hari
- Peluang hujan dan rekomendasi aktivitas sales
- Bagikan ringkasan cuaca
- Permintaan izin notifikasi browser

Sumber:
- Open-Meteo Forecast API dan Geocoding API. Periksa ketentuan penggunaan terbaru di https://open-meteo.com/en/terms
- Untuk penggunaan nonkomersial, akses tanpa API key tersedia dengan ketentuan atribusi Open-Meteo.

Cara menjalankan:
1. Ekstrak ZIP.
2. Unggah isi folder ke hosting statis HTTPS (misalnya GitHub Pages atau layanan static hosting lain).
3. Buka URL HTTPS di Chrome Android.
4. Pilih menu Chrome > Tambahkan ke layar utama / Install app.
5. Izinkan lokasi dan notifikasi bila diminta.

Catatan:
- PWA memerlukan HTTPS (atau localhost) untuk service worker dan instalasi.
- GPS tidak berfungsi pada file://; jalankan melalui HTTPS.
- Notifikasi browser tidak menjamin otomatis tampil di smartwatch. Agar diteruskan, aktifkan notifikasi Chrome pada Android dan izin notifikasi aplikasi di DA FIT.
- Aplikasi ini belum memiliki integrasi Bluetooth langsung dengan ZL50J dan tidak mengganti Bixby.
- Data cuaca memerlukan internet. Data lokasi tidak dikirim ke server aplikasi; koordinat dikirim ke API cuaca untuk memperoleh prakiraan.
