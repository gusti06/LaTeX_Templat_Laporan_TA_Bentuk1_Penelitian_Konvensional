# Templat LaTeX Laporan Tugas Akhir – Bentuk 1: Penelitian Konvensional
Prodi Teknik Informatika, Fakultas Teknologi Industri, Institut Teknologi Sumatera

## Cara pakai di Overleaf
1. Overleaf → New Project → Upload Project → pilih berkas ZIP ini.
2. Menu → Settings → Compiler: **pdfLaTeX**, Main document: **main.tex**.
3. Isi data diri di bagian "DATA TUGAS AKHIR" pada `main.tex`
   (judul, nama, NIM, pembimbing, penguji, koorprodi, tanggal, tahun).
4. Tulis isi tiap bab di folder `bab/`, referensi di `daftar-pustaka.bib`
   (ekspor BibTeX dari Mendeley/Zotero), sitasi dengan `\cite{kunci}`.

## Sakelar di main.tex
| Perintah | Fungsi |
|---|---|
| `\sidangakhirtrue` / `\sidangakhirfalse` | Sidang akhir (Bab I–V + Pernyataan AI) / Seminar proposal (Bab I–III) |
| `\petunjuktrue` / `\petunjukfalse` | Tampilkan / sembunyikan semua teks "Petunjuk:" |
| `\tampilpanduantrue` / `\tampilpanduanfalse` | Tampilkan / hapus halaman Petunjuk Pengisian & Peta Kewajiban |

## Struktur
- `itera-ta.sty` – format: kertas UNESCO 15,5×23 cm, Times 11 pt, spasi 1,5,
  margin cermin (atas 2, jilid 2,5, bawah 2, luar 2 cm), judul tabel di atas,
  judul gambar di bawah, IEEE.
- `halaman/` – sampul, pengesahan, orisinalitas, pernyataan AI, kata pengantar,
  abstract, abstrak, daftar singkatan.
- `bab/` – Bab I–V.
- `lampiran/lampiran.tex` – Daftar Lampiran + Lampiran 1–9.
  Simpan PDF (form bimbingan, Turnitin, dll.) di folder `lampiran/` dengan nama
  yang dirujuk di `\tempeldokumen{...}`; otomatis tersisip bila berkasnya ada.
- `gambar/` – logo ITERA; simpan gambar/diagram di sini.
  Pas foto: simpan `gambar/pasfoto.jpg` lalu isi `\newcommand{\pasfoto}{gambar/pasfoto.jpg}`.

## Makro bantu
- `\isian{...}` teks abu-abu dalam kurung siku (ganti dengan isi Anda).
- `\petunjuk{...}` petunjuk miring abu-abu.
- `\kotak` / `\kotakcentang` kotak centang pada Pernyataan AI & Daftar Lampiran.
