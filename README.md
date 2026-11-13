# Tugas Web Profile - Teknik Informatika UIKA

Proyek ini merupakan website *Major Profile* untuk Program Studi Teknik Informatika, Universitas Ibn Khaldun Bogor. Website dikembangkan sebagai karya untuk keperluan kompetisi.

## Identitas Pembuat
- **Nama:** D Firla Apriliani
- **NIM:** 261106040002
- **Universitas:** Universitas Ibn Khaldun Bogor
- **Program Studi:** Teknik Informatika
- **Kelas:** TI REG 1A

## Konsep Pembuatan Website
Konsep utama arsitektur website ini adalah *single-file approach*, yaitu menggabungkan seluruh struktur HTML, *styling* CSS, dan logika JavaScript ke dalam satu file utama tanpa memisahkannya ke dalam file eksternal (seperti `style.css` atau `script.js`).

Seluruh kode CSS kustom diletakkan di dalam tag `<style>` pada bagian `<head>`, dan seluruh logika JavaScript ditempatkan di dalam tag `<script>` pada bagian akhir sebelum penutup tag `</body>`.

### Alasan Penerapan Konsep Single-File:
1. **Zero Dependency (Tanpa Ketergantungan Eksternal):** Meminimalisir risiko kegagalan pemuatan aset (*file not found* atau *404 error*) yang sering terjadi akibat kesalahan penulisan *path* direktori saat proses *deployment*.
2. **Portabilitas Tinggi:** Website dapat dijalankan secara instan hanya dengan membuka file HTML melalui *web browser*, tanpa memerlukan konfigurasi *local server* tambahan.
3. **Kemudahan Audit Kode:** Mempermudah proses peninjauan struktur kode karena HTML, CSS, dan JavaScript dapat dilihat secara langsung pada satu file yang sama.
4. **Konsistensi Tampilan:** Desain dan tata letak (*layout*) dikunci menggunakan CSS internal sehingga konsistensi visual tetap terjaga di berbagai ukuran layar dan *browser*.

## Struktur Folder
Meskipun CSS dan JS digabung ke dalam HTML, aset berupa gambar tetap dipisahkan ke dalam folder `assets` untuk menjaga kerapian struktur proyek. Struktur foldernya adalah sebagai berikut:

```text
proyek-ti-uika/
│
├── index.html           (Halaman Landing Page)
├── lab-se.html          (Halaman Peminatan Software Engineering)
├── lab-csn.html         (Halaman Peminatan Computer System & Network)
├── lab-git.html         (Halaman Peminatan Geospatial Info. Tech.)
├── lab-keris.html       (Halaman Peminatan Knowledge Engineering)
├── README.md            (File dokumentasi ini)
│
└── assets/
    ├── img/
    │   ├── bg/          (Gambar background hero)
    │   ├── dosen/       (Foto-foto dosen)
    │   ├── lab/         (Foto fasilitas lab)
    │   ├── logo/        (Logo UIKA, Prodi, HIMA)
    │   ├── organisasi/  (Gambar struktur organisasi lab)
    │   └── ... (foto prestasi, galeri, dll)
    └── ...
