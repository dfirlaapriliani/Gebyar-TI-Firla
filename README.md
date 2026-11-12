# Tugas Web Profile - Teknik Informatika UIKA

Halo, ini adalah proyek website Major Profile untuk Program Studi Teknik Informatika UIKA Bogor. Website ini aku buat untuk keperluan lomba.

## Identitas Pembuat
- **Nama:** D Firla Apriliani
- **NIM:** 261106040002
- **Universitas:** Universitas Ibn Khaldun Bogor
- **Program Studi:** Teknik Informatika
- **Kelas:** TI REG 1A

## Konsep Pembuatan Website
Konsep utama website ini adalah *single-file approach* atau menggabungkan semuanya ke dalam satu file. Aku sengaja nggak pakai file CSS dan JS terpisah (seperti `style.css` atau `script.js`). 

Semua kode CSS kustom aku taruh di dalam tag `<style>` di bagian `<head>`, dan semua logika JavaScript aku taruh di dalam tag `<script>` di bagian paling bawah sebelum `</body>`.

### Kenapa Dibuat Seperti Itu?
1. **Biar Aman Pas Dinilai:** Pas juri buka filenya atau pas di-hosting, nggak bakal ada error kayak *styling* ilang atau *script* nggak jalan gara-gara salah path.
2. **Praktis:** Cuma butuh satu file HTML buat jalanin semuanya. Tinggal dobel klik, langsung kebuka di browser tanpa perlu setting *local server*.
3. **Gampang Dicek:** Juri tinggal *scroll* ke bawah atau pencet *inspect element* buat lihat langsung kode HTML, CSS, sama JS-nya tanpa harus pindah-pindah file.
4. **Tampilan Tetap Terjaga:** Karena layout dan desainnya aku kunci pake CSS, tampilannya nggak bakal berubah atau berantakan walaupun dibuka di device atau browser yang beda-beda.

## Struktur Folder
Meskipun CSS dan JS digabung ke dalam HTML, file gambar tetap aku pisahin ke dalam folder `assets` biar rapi. Struktur foldernya seperti ini:

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