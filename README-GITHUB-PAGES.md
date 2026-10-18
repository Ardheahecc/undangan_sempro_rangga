# Undangan Seminar Proposal — GitHub Pages

Project undangan HTML statis yang disiapkan untuk repository:

- Repository: https://github.com/Ardheahecc/undangan_sempro_ronggo
- URL GitHub Pages: https://ardheahecc.github.io/undangan_sempro_ronggo/
- OG image: https://ardheahecc.github.io/undangan_sempro_ronggo/og-undangan-rangga-v4.jpg

## Deploy melalui GitHub Pages

1. Ekstrak ZIP ini di komputer Anda. **Unggah isi folder ini**, bukan file ZIP dan bukan folder induknya, ke root repository `undangan_sempro_ronggo`.
2. Pastikan `index.html`, `undangan.html`, `og-undangan-rangga-v4.jpg`, dan folder `asset/` berada di root repository.
3. Commit dan push semua file ke branch `main`.
4. Di GitHub buka **Settings → Pages**.
5. Pada **Build and deployment**, pilih **Deploy from a branch**.
6. Pilih branch **main** dan folder **/(root)**, lalu klik **Save**.
7. Tunggu proses deployment selesai di tab **Actions**. URL situs akan tersedia pada pengaturan Pages.

## Verifikasi Open Graph

Setelah deployment, buka kedua alamat berikut di browser:

- Halaman: https://ardheahecc.github.io/undangan_sempro_ronggo/
- Gambar OG langsung: https://ardheahecc.github.io/undangan_sempro_ronggo/og-undangan-rangga-v4.jpg

Gambar OG harus terbuka tanpa login. HTML menaruh `og:image` dan `twitter:image` secara langsung di bagian `<head>`, sehingga crawler tidak bergantung pada JavaScript. Semua URL OG/canonical menggunakan URL proyek GitHub Pages lengkap, termasuk nama repository `/undangan_sempro_ronggo/`.

## Uji WhatsApp

Setelah situs aktif dan URL gambar bisa dibuka, bagikan tautan ini untuk memicu pengambilan preview dengan URL baru:

`https://ardheahecc.github.io/undangan_sempro_ronggo/?ogv=4`

WhatsApp dapat menyimpan cache preview. Jika gambar belum tampil, pastikan deployment terbaru selesai dan URL gambar publik dapat dibuka dahulu; kode lokal saja tidak mengubah situs yang sudah online.

## Catatan

- Semua path aset dalam halaman dipertahankan relatif, sehingga tetap bekerja di bawah path proyek `/undangan_sempro_ronggo/`.
- Konfigurasi khusus Netlify sudah dihapus karena hosting target adalah GitHub Pages.
- Metadata `og:url` dan `canonical` mengarah ke URL dasar proyek yang stabil, tanpa query parameter.
