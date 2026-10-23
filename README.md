# Pojok Baca Kelas

Perpustakaan digital: koleksi Google Drive (PDF, DOCX, dan lainnya) + jutaan buku terbuka gratis.
memakai SOLID STATE dari HTML5 UP (CC BY 3.0).

## Struktur
- `index.html`: halaman struktur template, bagian koleksi, pembaca
- `assets/css/main.css`: CSS asli SOLID STATE
- `assets/css/app.css`: Komponen pada tampilan web
- `assets/js/main.js` dan pustaka: fungsi pustaka dan tampilan
- `assets/js/app.js`: logika Web, CFG api Keys
- `Code.gs`: backend Apps Script

## Mengubah tampilan
Warna dan sudut diatur template. Ubah warna aksen di `assets/css/app.css  dan gambar latar di `images/bg.jpg`.
Teks halaman ada di `index.html`. Ganti `images/pic01.jpg` sampai `pic08.jpg` dengan fotomu sendiri.

## Menghubungkan Google Drive
isi baris CFG '' pada app.js
- **Cara A (Apps Script):** pasang `Code.gs` (isi `FOLDER_ID`), deploy sebagai Web App (Akses: Siapa saja), isi `CFG.API` dengan URL `/exec`.
- **Cara B (langsung):** isi `CFG.FOLDER_ID` dan `CFG.API_KEY` (Google Drive API, batasi ke API keys ;Important).

Folder harus dibagikan "Siapa saja yang memiliki link". Subfolder menjadi kategori (awalan "Karya" = tipe Karya). Deskripsi file: `Penulis | Sinopsis`.

## Perpustakaan Terbuka
Tab ini mencari di Project Gutenberg, Internet Archive, dan Open Library (hanya buku domain publik atau akses terbuka). Tanpa kunci atau backen.

## Deploy
- **Deploy** (disarankan): unggah seluruh folder kecualikan code.gs

## Pembaca
Panah kiri/kanan pindah buku, `i` info, `Esc` tutup. Setiap buku punya tautan sendiri
