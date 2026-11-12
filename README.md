# MONDIS Web — Static Frontend Demo

Frontend HTML/CSS/JavaScript untuk MONDIS UP3 Jayapura. Tidak memerlukan instalasi Python, Docker, Render, atau build tools.

## Jalankan

Buka `index.html` dengan browser. Untuk pengujian melalui server lokal: `python -m http.server 8000`, lalu buka http://localhost:8000.

## Deploy via GitHub Pages

1. Upload `index.html`, `styles.css`, dan `app.js` ke repository **khusus demo frontend** (disarankan terpisah dari aplikasi Streamlit utama).
2. Di GitHub pilih **Settings → Pages → Build and deployment → Deploy from a branch**.
3. Pilih branch `main`, folder `/ (root)`, lalu Save.
4. Buka URL yang ditampilkan GitHub Pages.

**Catatan:** GitHub Pages pada umumnya memublikasikan situs secara terbuka, termasuk bila repository bersifat private sesuai dukungan paket. Jangan masukkan data PLN sebenarnya atau informasi kontrak sensitif.

## Data dan keamanan

- Data demo tersimpan hanya pada `localStorage` browser yang digunakan, tidak tersinkronisasi antar perangkat atau pengguna.
- Gunakan menu Backup Data untuk ekspor/impor JSON.
- Tidak ada login, otorisasi, enkripsi data, atau database server.
- Jangan gunakan untuk produksi. Untuk multiuser, diperlukan backend, database persisten, autentikasi dan otorisasi, serta audit trail.
- File-file ini tidak menggantikan aplikasi Streamlit `app.py` yang sudah ada.
