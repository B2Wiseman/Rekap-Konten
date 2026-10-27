# Rekap Konten EV — Glass Dashboard v2

Dashboard HTML statis dengan ikon kamera, background animasi, glassmorphism blur, dan tiga progres utama:
- **Selesai** — hijau, jika kolom Diupload terisi.
- **Disetor** — kuning, jika belum diupload dan kolom Disetor terisi tanpa tanggal revisi.
- **Direvisi** — merah, jika belum diupload dan kolom Revisi terisi.
- **Belum disetor** — abu-abu jika belum ada tanggal setoran, revisi, atau upload.

## Google Sheets
Spreadsheet ID sudah disetel di `index.html`. Nama tab yang dibaca: `Oktober`, `November`, `Desember`. Urutan kolom 9 pertama pada tiap tab: Periode, Konten, Dibuat, Disetor, Revisi, Diupload, Talent, Caption, Link. Publikasikan setiap tab melalui File → Share → Publish to web. Data yang dipublikasikan dapat diakses publik.

Untuk menambahkan bulan, ubah `const SHEET_NAMES=['Oktober','November','Desember'];` di `index.html`, lalu tambahkan nama tab yang sama persis.

## Upload GitHub Pages
1. Buat repository GitHub.
2. Upload `index.html` langsung ke root repository lalu Commit changes.
3. Settings → Pages → Deploy from a branch → `main` → `/(root)` → Save.
4. Buka URL yang ditampilkan pada Settings → Pages setelah deploy selesai.

Koneksi perlu diuji dari URL GitHub Pages setelah tab dipublikasikan.
