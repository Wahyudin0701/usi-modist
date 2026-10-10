# 📜 SOP & ATURAN MAIN KOLABORASI AI - PROYEK USI MODIST

> **PERINGATAN UNTUK AGEN AI:** Dokumen ini adalah Undang-Undang Tertinggi dalam proyek ini. Anda WAJIB mematuhi seluruh aturan di bawah ini tanpa terkecuali setiap kali berinteraksi dengan USER atau memodifikasi file di dalam direktori ini.

---

## 1. MANAJEMEN PERCAKAPAN & MEMORI (STATE MANAGEMENT)
1. **Pemisahan Konteks:** Proyek ini dibagi menjadi percakapan yang berbeda (Cabang Skripsi, Cabang Coding, Cabang Random) menggunakan fitur **`Split`**.
2. **Kewajiban Sinkronisasi:** Sebelum memulai pekerjaan di percakapan baru, AI wajib membaca *Shared Memory* yang relevan:
   - Baca `MEMORY_SKRIPSI.md` untuk pengerjaan dokumen akademik/skripsi.
   - Baca `MEMORY_SISTEM.md` untuk pengerjaan kode (*programming*).

## 2. MANAJEMEN REFERENSI AKADEMIK (ANTI-HALUSINASI)
1. **Single Source of Truth:** Seluruh landasan teori dan kutipan akademik HANYA boleh diambil dari folder `C:\laragon\www\usi-modist\docs/Jurnal-Referensi-Udin\`. AI dilarang keras mengarang (berhalusinasi) referensi fiktif.
2. **Hierarki Pembacaan Referensi (Efisiensi Token):** 
   - AI **WAJIB** membaca ringkasan berformat `.md` (misal: `Analisis_Sawitri_2023.md`) terlebih dahulu.
   - AI **BARU DIIZINKAN** membaca file asli `.pdf` HANYA JIKA informasi di file `.md` dirasa kurang (misalnya membutuhkan detail rumus, tabel kuesioner, atau *flowchart* spesifik).
3. **Alur Penambahan Referensi Baru (Gap Handling):**
   - Jika AI tidak menemukan teori yang dibutuhkan di dalam folder referensi, AI wajib mencari di internet menggunakan tool `search_web`.
   - AI melaporkan Judul dan Link kepada USER.
   - USER akan mengunduh file PDF tersebut dan memasukkannya ke folder `docs/Jurnal-Referensi-Udin`.
   - Setelah USER mengonfirmasi, AI baru boleh membuat file analisis `.md` baru dan melanjutkan penulisan.

## 3. PENGEMBANGAN SISTEM & CODING
1. **Eksekusi Otomatis:** AI harus bertindak secara *Agentic*. Jangan hanya memberikan *snippet code* untuk di-*copy-paste*. Gunakan tool eksekusi terminal (PowerShell) dan modifikasi file secara langsung di komputer USER.
2. **Proactive Debugging:** Jika perintah terminal atau *code* menghasilkan error, AI harus proaktif membaca file `storage/logs/laravel.log` atau pesan error terminal, menganalisis masalahnya, dan langsung memperbaikinya tanpa harus menunggu instruksi berlapis dari USER.
3. **Environment:** Semua pengembangan dilakukan di lingkungan **Laragon** (Windows) menggunakan *stack* Laravel 11, MySQL, Midtrans Snap API, dan metode pengembangan *Prototyping*.

---
*Ditetapkan dan disepakati oleh USER dan Agen AI Antigravity.*
