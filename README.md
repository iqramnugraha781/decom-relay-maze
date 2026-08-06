# 🧩 DecomRelay: Decomposition Relay Maze

> **Game Pembelajaran Interaktif Berpikir Komputasional (Materi Dekomposisi) untuk Papan Interaktif Digital (PID) & Web Browser.**

**DecomRelay** adalah media pembelajaran berbasis game PvP (*Player vs Player*) estafet yang dirancang khusus untuk membantu siswa SMP memahami konsep **Dekomposisi dalam Berpikir Komputasional (*Computational Thinking*)**.

Game ini mengajak siswa secara beregu untuk memecah masalah besar (menghafal rute jalan yang panjang) menjadi sub-masalah kecil yang dikerjakan secara bertahap oleh setiap anggota tim melalui bantuan sistem *Checkpoint*.

---

## 🌟 Fitur Utama

* 📺 **Optimasi Papan Interaktif Digital (PID)**: Tampilan *split-screen* dengan tombol kontrol sentuh besar yang responsif untuk dua tim bertanding secara bersamaan di layar sentuh besar.
* 🧩 **Simulasi Dekomposisi Nyata**: Rute panjang secara otomatis dipecah menjadi modul-modul pendek sesuai jumlah anggota kelompok.
* 🗺️ **Peta Grid 2D *Mystery Board***: Peta netral tanpa petunjuk visual langsung, memaksa siswa fokus pada urutan logika langkah (Atas, Bawah, Kiri, Kanan).
* 🚩 **Sistem Checkpoint & Modul**: Jika siswa salah melangkah, karakter hanya akan kembali ke *Checkpoint* terakhir (bukan ke awal), membuktikan secara langsung manfaat dekomposisi dan modularitas dalam efisiensi kerja.
* ⚡ **Tanpa Dependensi / Installation-Free**: File tunggal statis (`index.html`), langsung dapat dijalankan tanpa perlu `npm`, `node_modules`, atau proses *build*.
* 🔊 **Efek Audio Sintetis (Web Audio API)**: Dilengkapi efek suara interaktif bawaan tanpa memerlukan file audio eksternal.

---

## 🎯 Hubungan dengan Kurikulum & Berpikir Komputasional

| Konsep Game | Prinsip Berpikir Komputasional |
| --- | --- |
| Membagi rute 12–16 langkah menjadi 3–4 blok hafalan per anggota | **Dekomposisi (*Decomposition*)**: Memecah masalah kompleks menjadi bagian-bagian kecil yang mudah dikelola. |
| Setiap anggota hanya menghafal pola panah untuk blok tugasnya | **Abstraksi (*Abstraction*)**: Fokus hanya pada informasi/tugas yang relevan di tingkat modul masing-masing. |
| Penguncian progres di setiap benderanya (*Checkpoint*) | **Modularitas (*Modularity*)**: Memastikan kegagalan di satu komponen tidak merusak seluruh sistem dari awal. |

---

## 🎮 Cara Bermain di Kelas

1. **Pembentukan Tim**: Bagi kelas menjadi 2 tim bertanding (Tim Merah vs Tim Biru) dengan 3–4 siswa per tim.
2. **Fase Perencanaan & Hafalan**:
* Sistem akan menampilkan rute langkah satu per satu di layar.
* Anggota tim membagi tugas (misal: Anggota 1 menghafal langkah 1–4, Anggota 2 langkah 5–8, dst.).


3. **Fase Estafet (PvP Race)**:
* Anggota 1 dari masing-masing tim maju ke PID untuk mengeksekusi langkah 1–4.
* Setelah mencapai *Checkpoint*, ganti posisi (*high-five*) dengan Anggota 2 yang melanjutkan langkah berikutnya.
* Tim pertama yang mencapai garis *Finish* memenangkan pertandingan!



---

## 🚀 Cara Menjalankan & Deploy

### A. Jalankan Lokal

Cukup unduh atau kloning repositori ini, lalu klik dua kali pada file `index.html` untuk membuanya di browser apa pun (Google Chrome, Edge, Safari).

```bash
git clone https://github.com/username-anda/decom-relay-maze.git
cd decom-relay-maze
# Buka file index.html di browser

```

### B. Deploy Gratis ke GitHub Pages

1. *Fork* atau buat repositori baru di GitHub dengan nama `decom-relay-maze`.
2. Unggah file game dan pastikan diberi nama **`index.html`**.
3. Buka **Settings** > **Pages**.
4. Pada menu **Branch**, pilih `main` / `master` dan folder `/ (root)`, lalu klik **Save**.
5. Tautan publik siap digunakan di layar PID dalam waktu 1–2 menit!

---

## 🛠️ Teknologi yang Digunakan

* **HTML5**: Struktur UI dan tata letak *split-screen*.
* **Tailwind CSS (via CDN)**: Desain antarmuka modern yang responsif untuk berbagai ukuran layar PID.
* **Vanilla JavaScript (ES6+)**: Logika game, animasi grid 2D, pewaktu hafalan, dan sistem *checkpoint*.
* **Web Audio API**: Generator nada/suara sintetis *real-time*.

---

## 📄 Lisensi

Proyek ini dirilis di bawah lisensi [MIT License](https://www.google.com/search?q=LICENSE). Bebas digunakan, dimodifikasi, dan didistribusikan untuk kepentingan pendidikan.
