# I. PENDAHULUAN 

# 1.1 Latar Belakang 

Perkembangan teknologi informasi mendorong pelaku usaha, termasuk Usaha Mikro, Kecil, dan Menengah (UMKM), untuk memanfaatkan teknologi digital dalam berbagai aktivitas bisnis. Pemanfaatan tersebut mencakup proses e-procurement, Point of Sales (POS), e-marketing, e-commerce, hingga pembayaran digital, dan penelitian pada UMKM di Indonesia menunjukkan adanya hubungan positif antara adopsi digital dan kinerja bisnis (Affandi et al., 2024). Namun demikian, tingkat adopsi teknologi digital di kalangan UMKM belum merata. Kementerian Komunikasi dan Digital RI (2024) mencatat bahwa dari sekitar 64 juta UMKM di Indonesia, baru sekitar 26% yang telah beralih ke platform digital. Penelitian terhadap 2.222 usaha mikro dan kecil di Indonesia juga menunjukkan bahwa pemanfaatan teknologi berbasis digital, termasuk teknologi keuangan digital dan penjualan daring, belum diterapkan secara seragam pada pelaku usaha (Trinugroho et al., 2022). Kondisi tersebut menunjukkan masih adanya ruang bagi UMKM untuk mengoptimalkan pemanfaatan teknologi digital dalam mendukung aktivitas operasional dan penjualan. 

Pada bidang usaha fashion, kebutuhan terhadap pemanfaatan teknologi digital menjadi semakin relevan karena subsektor ini memiliki kontribusi yang besar terhadap ekonomi kreatif Indonesia. Penelitian Arifin (2025) menunjukkan bahwa subsektor fesyen memiliki hubungan positif yang kuat terhadap peningkatan nilai tambah ekonomi kreatif nasional dengan koefisien jalur sebesar 0,880. Selain itu, fesyen merupakan salah satu kontributor utama ekspor ekonomi kreatif Indonesia dengan kontribusi sebesar 61,5% (Nasution, 2023). Dalam aktivitas penjualannya, usaha fashion dapat menangani produk ready stock maupun pesanan custom atau pre-order yang memiliki karakteristik proses transaksi berbeda. Sawitri et al. (2023) 

menunjukkan bahwa proses penjualan ready stock dan pre-order pada UMKM fashion memerlukan pengelolaan transaksi yang berbeda, termasuk pada proses permintaan dan pemrosesan pesanan. Kondisi tersebut menunjukkan bahwa pengelolaan penjualan usaha fashion memerlukan sistem yang mampu menyesuaikan proses transaksi dengan karakteristik pesanan. 

USI Modist merupakan usaha fesyen ecoprint yang berlokasi di Kota Jambi dan bergerak pada pengembangan produk fesyen berbasis ecoprint (Simatupang et al., 2024). Berdasarkan hasil pra-penelitian, aktivitas penjualan USI Modist mencakup produk ready stock dan pesanan custom. Pengelolaan operasional melibatkan peran Admin dalam menjalankan aktivitas penjualan dan pengelolaan data usaha, sedangkan Owner membutuhkan informasi yang dapat digunakan untuk memantau aktivitas penjualan dan kondisi usaha. 

Berdasarkan hasil observasi dan wawancara awal, pengelolaan transaksi ready stock maupun pesanan custom di USI Modist masih dilakukan secara manual menggunakan pencatatan buku. Kondisi serupa juga ditemukan pada penelitian Pratama et al. (2025), yang mengidentifikasi permasalahan berupa pencatatan transaksi manual, keterbatasan metode pembayaran, dan pengelolaan stok yang belum efisien pada UMKM. Pada USI Modist, kondisi tersebut terlihat dari hasil pencocokan catatan buku dengan stok fisik pada [tanggal], yang menunjukkan selisih pada [X] dari [Y] jenis produk _ready stock_ . Menurut Admin, dalam [3] bulan terakhir terdapat sekitar [X] pesanan _custom_ yang terlewat dari proses tindak lanjut, dan Owner membutuhkan sekitar [X jam/hari] untuk merekap penjualan bulanan secara manual dari catatan buku (hasil observasi dan wawancara, [tanggal]). Selain permasalahan internal, USI Modist telah memiliki _website_ berbasis [platform] yang pemanfaatannya masih terbatas sebagai media informasi. Sistem eksternal yang dikembangkan pada penelitian ini melengkapi 

_website_ tersebut dengan katalog produk dan fasilitas transaksi mandiri, tanpa menggantikan fungsi _company profile_ yang telah ada. 

Berdasarkan permasalahan tersebut, diperlukan sistem informasi penjualan yang mampu mengintegrasikan pengelolaan operasional internal dengan akses transaksi pelanggan pada sisi eksternal. Sistem yang dikembangkan diharapkan dapat mendukung pengelolaan produk, transaksi, dan pesanan oleh Admin, menyediakan informasi penjualan bagi Owner, menampilkan katalog produk kepada pelanggan, serta memungkinkan pelanggan melakukan pemesanan secara mandiri. Sistem juga perlu menyesuaikan alur transaksi untuk produk ready stock dan pesanan custom serta menghubungkan transaksi dengan pencatatan pemasukan secara konsisten. Pada sisi pembayaran, integrasi payment gateway dapat digunakan untuk mendukung transaksi non-tunai dan sinkronisasi status pembayaran dengan data pesanan. 

Beberapa penelitian terdahulu menunjukkan bahwa digitalisasi pada UMKM telah diterapkan melalui berbagai bentuk sistem dan pendekatan. Affandi et al. (2024) mengidentifikasi lima proses bisnis yang dapat didigitalisasi pada UMSE di Indonesia, yaitu e-procurement, POS, e-marketing, e-commerce, dan digital payment. Pada konteks UMKM fashion, Febriani et al. (2025) menunjukkan pentingnya integrasi kanal penjualan dengan dukungan pengelolaan persediaan secara real-time dan keterlibatan pelanggan. Sementara itu, Sawitri et al. (2023) menunjukkan bahwa penjualan ready stock dan pre-order pada UMKM fashion memiliki alur proses yang berbeda. Dari sisi implementasi sistem penjualan, Pratama et al. (2025) mengembangkan POS berbasis web yang terintegrasi Midtrans, sedangkan Maulana dan Widiono (2024) mengembangkan POS berbasis web dengan integrasi Xendit untuk mendukung pengelolaan stok, transaksi penjualan, dan pembelian secara real-time.  Buwono et al. (2024)  juga mengimplementasikan 

payment gateway Midtrans pada sistem penjualan UMKM Batik Lurik untuk mendukung transaksi digital dan pembaruan status pesanan. 

Berdasarkan penelitian-penelitian tersebut, dapat dilihat bahwa penelitian terdahulu memiliki fokus yang berbeda, mulai dari pengukuran adopsi digital UMKM, transformasi omnichannel pada sektor fashion, pemodelan proses ready stock dan pre-order, hingga pengembangan POS dan integrasi payment gateway. Berdasarkan studi yang ditinjau, masih terdapat peluang untuk mengembangkan sistem yang secara khusus menggabungkan pengelolaan operasional internal, akses transaksi pelanggan, penanganan ready stock dan pesanan custom, integrasi payment gateway, serta keterhubungan transaksi dengan pencatatan keuangan dalam satu sistem yang disesuaikan dengan kebutuhan UMKM fashion ecoprint USI Modist. 

Dalam pengembangannya, penelitian ini menggunakan metode Prototyping yang terdiri atas tahapan communication, quick plan, modeling quick design, construction of prototype, serta deployment, delivery & feedback (Alawiyah & Cahyana, 2025). Metode ini dipilih karena memungkinkan rancangan sistem dikembangkan secara iteratif melalui evaluasi dan umpan balik pengguna sehingga kebutuhan sistem dapat disempurnakan secara bertahap (Kholis & Zaky, 2025). Pendekatan tersebut sesuai dengan kondisi USI Modist yang kebutuhan sistemnya masih terus digali melalui proses pra-penelitian dan penyempurnaan rancangan antarmuka. 

Penelitian ini dilaksanakan secara paralel dengan penelitian [Nama Partner] (NIM [..]) berjudul “[judul final]”, yang berfokus pada analisis kebutuhan pengguna dan perancangan UI/UX dengan pendekatan _Design Thinking_ pada objek yang sama. Hasil penelitian tersebut digunakan sebagai acuan pada tahap _communication_ (kebutuhan pengguna) dan _modeling quick design_ (rancangan antarmuka), sedangkan penelitian ini berfokus pada implementasi sistem 

berdasarkan rancangan tersebut. Kendala teknis yang ditemukan pada tahap _construction of prototype_ dan _deployment, delivery & feedback_ dikomunikasikan kepada peneliti UI/UX untuk penyempurnaan rancangan pada iterasi berikutnya. 

Selain aspek fungsional sistem, penelitian ini juga mempertimbangkan pemanfaatan AI agent dalam proses pembangunan prototipe untuk mendukung efisiensi pengembangan, sebuah pendekatan yang belakangan dikenal sebagai vibe coding (Meske et al., 2025). Mengingat sistem yang dibangun menangani transaksi dan data keuangan, penerapan pendekatan ini tetap disertai proses validasi dan pengujian terstruktur, khususnya pada modul-modul kritis, guna memastikan kualitas dan keandalan hasil implementasi. 

# 1.2 Rumusan Masalah 

Berdasarkan latar belakang yang telah diuraikan, maka rumusan masalah dalam penelitian ini adalah sebagai berikut: 

   1. Bagaimana merancang dan mengimplementasikan sistem informasi penjualan pada USI Modist yang mengintegrasikan pengelolaan operasional internal (oleh Admin dan Owner) dengan akses transaksi mandiri bagi pelanggan pada sisi eksternal, serta mampu menyesuaikan alur transaksi untuk produk _ready stock_ dan pesanan _custom_ ? 

   2. Bagaimana mengintegrasikan _payment gateway_ pada sistem tersebut agar transaksi penjualan tercatat secara otomatis dan konsisten sebagai data operasional dan keuangan? 

   3. Bagaimana pendekatan _AI-Assisted Development_ diterapkan dalam proses pembangunan sistem dengan tetap memastikan kualitas dan keandalan pada modul-modul kritis seperti transaksi dan pembayaran? 

- 1.3 Tujuan Penelitian 

Berdasarkan rumusan masalah di atas, tujuan dari penelitian ini adalah sebagai berikut: 

   1. Merancang dan mengimplementasikan sistem informasi penjualan pada USI Modist yang mengintegrasikan pengelolaan operasional internal (oleh Admin dan Owner) dengan akses transaksi mandiri bagi pelanggan pada sisi eksternal, serta mampu menyesuaikan alur transaksi untuk produk _ready stock_ dan pesanan _custom_ . 

   2. Mengintegrasikan _payment gateway_ pada sistem yang dibangun agar transaksi penjualan tercatat secara otomatis dan konsisten sebagai data operasional dan keuangan. 

   3. Menerapkan pendekatan _AI-Assisted Development_ dalam proses pembangunan sistem dengan tetap memastikan kualitas dan keandalan pada modul-modul kritis seperti transaksi dan pembayaran. 

- 1.4 Batasan Penelitian 

Penelitian ini memiliki batasan sebagai berikut: 

1. Penelitian ini berfokus pada implementasi sistem informasi penjualan USI Modist. Analisis kebutuhan pengguna dan perancangan UI/UX, termasuk pengujian _usability_ dan evaluasi pengalaman pengguna, tidak termasuk dalam cakupan penelitian ini dan dilakukan pada penelitian [Nama Partner] berjudul “[judul final]” yang dilaksanakan secara paralel dengan pendekatan _Design Thinking_ . Hasil penelitian tersebut digunakan sebagai acuan perancangan antarmuka, sedangkan penyesuaian antarmuka selama implementasi dibatasi pada kendala teknis dan dikonsultasikan kepada peneliti UI/UX. 

2. Sistem yang dibangun terdiri atas sub-sistem internal (pengelolaan produk, transaksi, pesanan, serta laporan penjualan dan 

keuangan untuk Admin dan Owner) dan sub-sistem eksternal (registrasi, _login_ , katalog produk, serta transaksi mandiri bagi pelanggan). 

3. Penelitian ini tidak mencakup pengelolaan bahan baku maupun proses produksi (seperti pencatatan stok kain, bahan pewarna, atau tahapan produksi _ecoprint_ ), dan hanya berfokus pada pengelolaan produk _ready stock_ yang telah selesai diproduksi. 

4. Pengujian pada sub-sistem internal dilakukan melalui _Black Box Testing_ dan _User Acceptance Testing_ (UAT) yang melibatkan Owner, Admin, dan karyawan USI Modist. Pengujian pada sub-sistem eksternal dibatasi pada _Black Box Testing_ menggunakan akun uji coba oleh peneliti, tanpa melibatkan pengujian penerimaan pengguna (UAT) oleh pelanggan aktual. 

5. Penerapan pendekatan _AI-Assisted Development_ pada penelitian ini tidak dimaksudkan sebagai penelitian eksperimental yang membandingkan proses _coding_ manual dengan _coding_ berbantuan AI. Evaluasi dilakukan melalui perbandingan tingkat intervensi manual, _acceptance rate_ , dan _defect density_ antara modul kritis dan modul non-kritis dalam satu proses pengembangan yang sama. 

6. Notifikasi status pesanan kepada pelanggan disampaikan melalui WhatsApp secara semi-otomatis, yaitu sistem menyediakan template pesan sesuai status pesanan yang selanjutnya dikirimkan secara manual oleh Admin, bukan melalui integrasi API pengiriman pesan otomatis. 

7. Metode pembayaran yang didukung sistem mengikuti metode yang disediakan oleh _payment gateway_ Midtrans (Virtual Account, _ewallet_ , QRIS, dan/atau kartu kredit), dengan mekanisme 

pembayaran (uang muka/DP atau pembayaran penuh) untuk pesanan _custom_ mengikuti kebijakan yang berlaku di USI Modist. 

8. Penelitian ini menghasilkan produk sistem yang siap diserahterimakan kepada USI Modist, dengan pengujian penerimaan pengguna pada sisi eksternal (pelanggan) direkomendasikan sebagai tindak lanjut pasca-penelitian. 

9. Penelitian ini tidak mencakup migrasi atau pengembangan ulang konten website company profile yang telah ada. 

# 1.5 Manfaat Penelitian 

1. Manfaat Teoritis 

Penelitian ini diharapkan dapat memberikan kontribusi terhadap pengembangan ilmu pengetahuan di bidang sistem informasi, khususnya terkait perancangan dan implementasi sistem informasi penjualan yang mengintegrasikan pengelolaan operasional internal dengan akses transaksi mandiri pelanggan pada sisi eksternal, serta keterhubungan antara proses transaksi dengan pencatatan keuangan pada konteks UMKM fashion berbasis _ecoprint_ . Selain itu, penelitian ini juga diharapkan dapat menjadi referensi awal mengenai penerapan pendekatan _AIAssisted Development_ dalam proses pembangunan sistem yang memiliki modul kritis, khususnya pada transaksi dan integrasi pembayaran. 

2. Manfaat Praktis 

   - a. Bagi USI Modist 

Sistem yang dihasilkan diharapkan dapat membantu Admin dalam mengelola transaksi _ready stock_ dan pesanan _custom_ secara lebih terpusat dan akurat, membantu Owner dalam memantau kondisi penjualan dan keuangan usaha secara _real-time_ , serta memungkinkan pelanggan untuk melihat katalog produk dan melakukan transaksi secara 

mandiri melalui platform digital tanpa harus melakukan kontak manual terlebih dahulu. 

- b. Bagi Peneliti 

Penelitian ini menjadi sarana penerapan ilmu yang telah dipelajari selama masa perkuliahan, khususnya dalam merancang dan membangun sistem informasi penjualan yang mengintegrasikan sisi internal dan eksternal menggunakan metode _Prototyping_ , sekaligus menjadi pengalaman langsung dalam menerapkan pendekatan _AIAssisted Development_ secara terstruktur dan terukur pada bagian pengembangan sistem. 

- c. Bagi Akademik 

Hasil penelitian ini diharapkan dapat menjadi bahan referensi tambahan bagi mahasiswa lain yang akan melakukan penelitian sejenis, khususnya yang berkaitan dengan pengembangan sistem informasi penjualan yang mengintegrasikan sisi internal dan eksternal, integrasi _payment gateway_ , maupun penerapan kecerdasan buatan dalam proses pengembangan perangkat lunak. 

# DAFTAR PUSTAKA 

- Affandi, Y., Ridhwan, M. M., Trinugroho, I., & Hermawan, D. (2024). Digital Adoption, Business Performance, and Financial Literacy in Ultra-Macro, Micro, and Small Enterprises in Indonesia. _Research in International Business and Finance (RIBAF)_ , _7_ (10), 881–885. https://doi.org/10.1016/j.ribaf.2024.102376 

- Alawiyah, D., & Cahyana, R. (2025). Rancang Bangun Sistem Monitoring Kinerja Karyawan dan Penggajian Karyawan Konveksi berbasis web. _Jurnal Algoritma_ , _22_ (1), 592–600. https://doi.org/10.33364/algoritma/v.22-1.1818 

- Arifin, Z. (2025). Kontribusi Subsektor Fesyen, Kuliner, dan Kriya terhadap Peningkatan Nilai Tambah Ekonomi Kreatif Nasional. _Jurnal Ekonomi Dan Kewirausahaan West Science_ , _3_ (01), 45–54. https://doi.org/10.58812/jekws.v3i01.1921 

- Buwono, R. C., Kartadie, R., & Ramadhan, M. K. (2024). Perancangan dan implementasi sistem payment gateway MIDTRANS untuk UMKM Batik Lurik. _INFOTECH : Jurnal Informatika & Teknologi_ , _5_ (2), 228– 238. https://doi.org/10.37373/infotech.v5i2.1334 

- Febriani, A., Sopha, B. M., & Arif Wibisono, M. (2025). Dynamic capabilities for omnichannel transformation in MSMEs: A comparative case study of fashion and furniture sectors. _Journal of Open Innovation: Technology, Market, and Complexity_ , _11_ (1), 100498. https://doi.org/10.1016/j.joitmc.2025.100498 

- Kementerian Komunikasi dan Digital RI. (2024). _Satu Dekade, Transformasi Digital UMKM Dorong Pertumbuhan Ekonomi Nasional_ Kementerian Komunikasi Dan Digital RI. https://www.komdigi.go.id/berita/siaran-pers/detail/satu-dekadetransformasi-digital-umkm-dorong-pertumbuhan-ekonomi-nasional 

- Kholis, M. Y., & Zaky, U. (2025). Implementasi Metode Prototype Pada Aplikasi Portal Lomba Informatika Berbasis Android Menggunakan Firebase. _Jurnal Informatika Teknologi Dan Sains (JINTEKS)_ , 667– 676. https://doi.org/10.51401/jinteks.v7i2.5628 

- Maulana, F. A., & Widiono, S. (2024). Inovasi Teknologi dalam Manajemen Penjualan: Aplikasi Point of Sales Berbasis Web untuk UMKM. _Infomatek_ , _26_ (2), 161–174. https://doi.org/10.23969/infomatek.v26i2.19007 

- Meske, C., Hermanns, T., Von der Weiden, E., Loser, K. U., & Berger, T. (2025). Vibe Coding as a Reconfiguration of Intent Mediation in Software Development: Definition, Implications, and Research Agenda. _IEEE Access_ , _13_ (December), 213242–213259. https://doi.org/10.1109/ACCESS.2025.3645466 

- Nasution, D. D. (2023). _Industri Fesyen jadi Andalan Ekspor Ekraf dengan Porsi 61,5 Persen_ . Republika.Co.Id. https://ekonomi.republika.co.id/berita/rqhk3b502/industrifesyen-jadi-andalan-ekspor-ekraf-dengan-porsi-615-persen 

- Pratama, M. I. S., Dermawan, B. A., & Carudin. (2025). Integrasi Payment Gateway Pada Aacplikasi Point of Sales Berbasis Website Menggunakan Framework Reactjs (Studi Kasus : Toko Adida Pratama). _Jurnal Informatika Dan Teknik Elektro Terapan_ , _13_ (3). https://doi.org/10.23960/jitet.v13i3.7099 

- Pratama, R. M. S. P., Alijoyo, F. A., & Sofiah, E. (2025). Optimalisasi Proses Bisnin UMKM Melalui User Interface Sistem Point of Sales (Studi Kasus: Cireng Asgard). _Jurnal Sistem Informasi_ , _7_ (2), 502–525. 

- Sawitri, R. A. D., Jaswadi, & Indrawan, A. K. (2023). The Business Process of Selling Ready Stock and Pre Order Items through E- Commerce System : an Indonesian SME Case Study. _Indonesian Journal of Business Analytics_ , _3_ (4), 1043–1066. 

https://doi.org/10.55927/ijba.v3i4.4850 

- Simatupang, Y. K., Mutia, A., Islam, U., Sulthan, N., & Saifuddin, T. (2024). Analisis manajemen strategi dalam meningkatkan ekonomi kreatif pada industri halal fesyen ecoprint usi modist kota jambi. _Penelitian Ilmiah Multidisplin_ , _8_ (12), 487–507. 

- Trinugroho, I., Pamungkas, P., Wiwoho, J., Damayanti, S. M., & Pramono, T. (2022). Adoption of digital technologies for micro and small business in Indonesia. _Finance Research Letters_ , _45_ (May), 102156. https://doi.org/10.1016/j.frl.2021.102156 

