# Praktikum AR/VR - Pertemuan 1

- Nama : Tegar Raya Harahap
- NIM : 2409020069
- Link demo : https://tegarksp.github.io/arvr-prak-2409020069/

Project ini berisi scene WebXR perkenalan diri menggunakan A-Frame 1.7.1.

## Isi Scene

- Tiga objek primitif berbeda: kubus (a-box), bola (a-sphere), dan silinder (a-cylinder), ditambah kerucut (a-cone) dan torus (a-torus).
- Lantai (a-plane) berwarna krem dan langit (a-sky) berwarna biru muda.
- Teks nama dan NIM menggunakan a-text.
- Bola berputar terus-menerus menggunakan atribut animation.

## Jawaban Refleksi

**1. Mengapa posisi objek yang terlihat pertama kali oleh pengguna memakai nilai z negatif?**
Pada A-Frame, sumbu Z mengarah ke pengguna, sehingga arah pandang awal kamera adalah Z negatif. Objek yang berada di depan pengguna saat scene pertama dibuka harus memiliki nilai z negatif, sedangkan objek dengan z positif berada di belakang kamera dan tidak terlihat.

**2. Mengapa WebXR hanya aktif pada HTTPS atau localhost?**
WebXR dapat mengakses perangkat sensitif seperti sensor gerak dan kontroler, sehingga peramban hanya mengizinkannya pada koneksi yang aman. Localhost dianggap aman karena hanya bisa diakses dari komputer itu sendiri, sedangkan alamat IP jaringan lokal menggunakan HTTP biasa dan tidak memenuhi syarat tersebut.

**3. Jelaskan perbedaan peran WebXR Device API, three.js, dan A-Frame dengan bahasa Anda sendiri.**
WebXR Device API adalah standar yang menghubungkan peramban dengan perangkat VR dan AR. three.js adalah pustaka grafik 3D yang mengelola scene, kamera, dan rendering di atas WebGL. A-Frame berada di atas three.js dan menyajikannya sebagai tag HTML, sehingga scene 3D bisa dibuat tanpa menulis kode tingkat rendah.