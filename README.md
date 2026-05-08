# **Sovereign Tetris**

Sovereign Tetris adalah implementasi modern dari permainan arcade klasik Tetris yang dibangun menggunakan teknologi web murni. Proyek ini menggabungkan estetika minimalis dengan fungsionalitas canggih seperti sistem audio prosedural dan fitur Real-time Multiplayer berbasis Peer-to-Peer (P2P).

## Abstraksi
Proyek ini bermula dari keinginan untuk menciptakan lingkungan permainan yang ringan namun memiliki performa tinggi tanpa ketergantungan pada game engine pihak ketiga yang berat. Fokus utama pengembangan terletak pada manipulasi matriks untuk logika blok, sinkronisasi data antar pemain secara langsung, dan penggunaan Web Audio API untuk menghasilkan efek suara secara dinamis melalui kode (tanpa file aset eksternal).

### Fitur Utama
- Classic Mechanics: Pergerakan blok, rotasi, dan sistem pembersihan baris yang presisi.
- P2P Multiplayer: Bertanding dengan teman secara real-time menggunakan sistem ID unik tanpa memerlukan server perantara yang kompleks.
- Procedural SFX: Efek suara yang dihasilkan secara sintetis menggunakan Web Audio API.
- Minimalist UI: Antarmuka berbasis glassmorphism yang bersih dan modern, dirancang menggunakan variabel CSS.
- Ada 4 level yang bisa di pilih di solo mode, yaitu Easy, Medium, Hard, dan WNI.

### Teknologi yang Digunakan
> Proyek ini dibangun sepenuhnya menggunakan Vanilla Web Stack untuk memastikan kecepatan dan portabilitas maksimal:

- HTML5 Canvas: Untuk perenderan grafis 2D berkecepatan tinggi.
- CSS3: Menggunakan Flexbox, CSS Grid, dan kustomisasi variabel untuk desain responsif.
-  JavaScript (ES6+): Logika permainan inti, mesin audio, dan manajemen state.
-  PeerJS: Library pembungkus WebRTC untuk menangani koneksi multiplayer langsung antar browser.

### Cara Menjalankan Proyek
> Sovereign Tetris dirancang untuk berjalan langsung di browser tanpa perlu instalasi tambahan.

1. Clone Repositori:
```
git clone https://github.com/username/sovereign-tetris.git
```

2. Buka File:
Cukup klik dua kali pada file index.html di browser pilihan Anda (Chrome, Firefox, atau Edge sangat direkomendasikan).

3. Mulai Bermain:
Gunakan tombol panah pada keyboard untuk mengontrol blok (Kiri/Kanan untuk geser, Atas untuk rotasi, dan Bawah untuk soft drop).

### Cara Menggunakan Fitur Multiplayer
> Sistem multiplayer menggunakan protokol P2P. Ikuti langkah berikut untuk bermain bersama teman:

1. Buka Game: Pastikan Anda dan teman Anda sama-sama membuka aplikasi.

2. Dapatkan ID: Klik tombol Pair Player. Anda akan melihat ID unik yang dihasilkan (misalnya: X9Z2K).

3. Hubungkan:

   - Minta teman Anda memberikan ID mereka kepada Anda.

   - Masukkan ID tersebut ke dalam kolom input di layar Anda.

   - Klik Establish Connection.

4. Sinkronisasi: Setelah status berubah menjadi Connected, data permainan akan dikirimkan secara langsung antar perangkat. Anda hanya perlu melakukan proses pairing ini satu kali selama sesi browser tidak ditutup.

## Pengembangan Mendatang (Roadmap)
> Karena proyek ini masih dalam tahap pengembangan awal, berikut adalah rencana fitur selanjutnya:

- Integrasi papan skor global (Leaderboard).

- Sistem level dan peningkatan kecepatan otomatis.

- Mode permainan tambahan seperti Timed Challenge.

- Optimasi kontrol sentuh untuk perangkat mobile.

**Dibuat oleh Juna.**
Proyek ini merupakan bagian dari eksplorasi pemrograman Informatika di Universitas Ciputra Surabaya.
