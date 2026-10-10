# MEMORY STATE: PENGEMBANGAN SISTEM USI MODIST

> **Dokumen ini adalah "Shared Memory" untuk Agen AI. Jika Anda membaca dokumen ini, gunakan informasi di bawah ini sebagai konteks utama untuk membantu USER mengembangkan sistem aplikasinya (Coding).**

## 1. Konteks & Spesifikasi Teknis
*   **Lokasi Proyek:** `c:\laragon\www\usi-modist`
*   **Environment:** Laragon (Windows)
*   **Tech Stack (Rekomendasi):** Laravel 11 (PHP), MySQL, dan TailwindCSS/Bootstrap (Frontend).
*   **Integrasi Pihak Ketiga:** Midtrans (Snap API) untuk Payment Gateway (QRIS, E-Wallet, VA).

## 2. Arsitektur Fitur Utama (Dual Mode)
Sistem ini memfasilitasi 2 jenis transaksi yang alurnya berbeda:
1.  **Ready Stock:** Pelanggan -> Masuk Keranjang -> Checkout -> Bayar Midtrans -> Pesanan Diproses (Otomatis potong stok).
2.  **Custom Order (Pre-Order):** Pelanggan -> Form Request Custom (Upload referensi) -> Review Admin/Desainer -> Penentuan Harga (Quotation) -> Disetujui Pelanggan -> Bayar DP/Full via Midtrans -> Proses Produksi -> Pelunasan -> Pengiriman.

## 3. Hak Akses (Role Base)
*   **Owner:** Memantau laporan keuangan harian/bulanan, dashboard analitik.
*   **Admin:** Mengelola produk, stok, menyetujui pesanan *custom*, memberikan notifikasi WA (semi-otomatis/template).
*   **Pelanggan:** Pendaftaran, login, melihat katalog *e-commerce*, melacak status pesanan.

## 4. Progres Pengembangan (Status Tracker)
- [ ] **Fase 1: Setup Lingkungan** (Instalasi Laravel, Konfigurasi `.env` & Laragon Database).
- [ ] **Fase 2: Database & Migrasi** (Pembuatan ERD dan file *migration* untuk entitas Produk, User, Transaksi, Detail Transaksi).
- [ ] **Fase 3: Autentikasi** (Multi-role login: Owner, Admin, Pelanggan).
- [ ] **Fase 4: Core Features Internal** (CRUD Produk, Stok, Manajemen Pesanan oleh Admin).
- [ ] **Fase 5: Core Features Eksternal** (Katalog e-commerce, Keranjang, Form Pesanan Custom).
- [ ] **Fase 6: Integrasi Midtrans** (Setup API Key, Webhook, Simulasi Pembayaran).
- [ ] **Fase 7: Testing & Debugging** (Black Box Testing sesuai metode Prototype).

## 5. Instruksi Khusus untuk AI
Selalu verifikasi perubahan kode sebelum mengeksekusi perintah terminal. Jika terdapat error, segera periksa log Laravel (`storage/logs/laravel.log`) secara otomatis untuk membantu USER melakukan debugging.
