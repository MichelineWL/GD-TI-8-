# Laporan Tutorial 8 - Game Polishing & Balancing

**Nama:** Micheline Wijaya Limbergh
**NPM:** 2306207013

## 1. Opini Mengenai Polishing
Penambahan percepatan (acceleration) dan perlambatan (deceleration) menggunakan fungsi `lerp()` sangat meningkatkan **Game Feel**. Karakter tidak lagi terasa kaku atau bergerak secara instan, melainkan memiliki "bobot" dan momentum yang membuat kontrol terasa lebih natural dan responsif. 

Selain itu, partikel lari memberikan *feedback* visual yang sangat memuaskan. Partikel ini membantu pemain mengetahui kapan karakter telah mencapai kecepatan maksimum (`speed`), sehingga interaksi lari terasa lebih dinamis dan memberikan kepuasan visual (juice) saat melakukan eksplorasi di dalam level.

## 2. Game Balancing: Spawn Rate
Setelah melakukan beberapa percobaan, saya memilih nilai Spawn Rate yang memberikan tantangan yang adil namun tetap bisa dilewati.
- **Spawn Rate Terpilih:** 2.0 detik
- **Alasan:** Nilai 2.0 detik memberikan jeda yang cukup bagi pemain untuk bereaksi dan melompati musuh yang muncul, namun tetap mempertahankan ritme permainan. Jika terlalu cepat (seperti 0.3 detik), pemain akan merasa kewalahan (*rage quit*), dan jika terlalu lambat (seperti 5.0 detik), tantangan menjadi hilang. Nilai 2.0 detik menciptakan kondisi **flow** di mana pemain harus tetap fokus tanpa merasa frustrasi.

## 3. Referensi
- [Godot Documentation: Interpolation](https://docs.godotengine.org/en/stable/tutorials/math/interpolation.html)
- [Godot Documentation: GPUParticles2D](https://docs.godotengine.org/en/stable/classes/class_gpuparticles2d.html)
- Kenney Platformer Pack Assets
