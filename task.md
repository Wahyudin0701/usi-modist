# Task Tracker: USI Modist POS & E-Commerce

Gunakan file ini untuk melacak status pengerjaan sistem. Ubah tanda `[ ]` menjadi `[/]` saat sedang dikerjakan, dan `[x]` jika sudah selesai.

## Fase 1: Setup & Inisiasi
- [x] Inisiasi repositori Git
- [x] Merapikan struktur folder dokumen (`docs/`)
- [x] Pembuatan aturan main AI (SOP) & Shared Memory
- [ ] Instalasi Laravel 11
- [ ] Konfigurasi `.env` dan pembuatan database `usi_modist` di MySQL
- [ ] Desain arsitektur database (ERD)

## Fase 2: Database & Migrasi (Backend)
- [ ] Pembuatan Model & Migration `Users` (Role: Owner, Admin, Customer)
- [ ] Pembuatan Model & Migration `Products` dan `Categories`
- [ ] Pembuatan Model & Migration `Transactions` (Ready Stock & Pre-Order)
- [ ] Pembuatan Model & Migration `Order_Details`

## Fase 3: Autentikasi & Authorization
- [ ] Setup Laravel Breeze / UI Auth
- [ ] Konfigurasi Middleware untuk Role Akses

## Fase 4: Core Features (Internal - Admin & Owner)
- [ ] CRUD Kategori & Produk
- [ ] Manajemen Stok Otomatis
- [ ] Modul Verifikasi Pesanan Custom (Pre-Order Quotation)
- [ ] Dashboard Analitik & Laporan Penjualan (Owner)

## Fase 5: Core Features (Eksternal - Pelanggan)
- [ ] Halaman Utama & Katalog Produk (E-Commerce)
- [ ] Fitur Keranjang Belanja (Cart)
- [ ] Fitur Checkout & Hitung Ongkir
- [ ] Form Pemesanan Custom (Upload Referensi Desain)

## Fase 6: Integrasi Payment Gateway
- [ ] Registrasi & Setup API Key Midtrans (Sandbox)
- [ ] Integrasi Midtrans Snap API (QRIS, VA, E-Wallet)
- [ ] Pembuatan Webhook untuk auto-update status pembayaran

## Fase 7: Pengujian & Deployment
- [ ] Black Box Testing (Admin, Owner, Pelanggan)
- [ ] Evaluasi Prototype
- [ ] Persiapan Produksi (Live)
