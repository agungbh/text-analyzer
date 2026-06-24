AI Text Analyzer & PR Generator Pro
Aplikasi web single-file berbasis PHP Native yang dirancang secara elegan dan modern untuk memproses, menganalisis, dan mentransformasi dokumen teks. Aplikasi ini mampu mendeteksi kesalahan tata bahasa (typo), plagiarisme, dan jejak buatan AI (AI-generated text), lalu menyempurnakannya menjadi dua format profesional: Artikel Ilmiah (Vancouver Style) dan Rilis Berita (Press Release) standar jurnalistik.

🌟 Fitur Utama
Aplikasi ini membagi antarmuka pengguna menjadi 5 Kolom Terintegrasi yang responsif di segala perangkat (Desktop, Laptop, Tablet, maupun Smartphone):

1. Kolom Input Dokumen (Ekstraksi Sisi Klien)
Mendukung pengetikan langsung (copy-paste) ke dalam text area.

Mendukung Upload File .docx dan .pdf. File tidak diunggah ke server, melainkan diekstrak secara langsung di browser pengguna (Client-Side) demi privasi dan kecepatan.

Menghitung statistik jumlah kata secara aktual.

2. Kolom Hasil Analisis Teks
Sistem akan memecah teks input per kalimat dan memberikan highlight warna yang informatif:

🔴 Merah (Typo): Kesalahan ejaan atau tata bahasa dasar.

🟣 Ungu (Plagiarisme AI): Teks yang terdeteksi dihasilkan oleh mesin/AI (seperti ChatGPT, Gemini, dll).

🟠 Oranye (Plagiarisme): Kalimat yang teridentifikasi menyalin persis dari literatur digital publik.

🟢 Hijau (Paraphrase): Teks yang unik, mengalir natural, dan lolos deteksi.

3. Kolom Saran Perbaikan
Menyajikan umpan balik komprehensif atas setiap temuan di Kolom 2. Memberikan rekomendasi perbaikan kata baku, restrukturisasi kalimat, hingga saran penyematan sitasi.

4. Kolom Artikel Ilmiah Final
Mentransformasi input yang cacat menjadi draf karya ilmiah yang sempurna:

Bahasa diubah menjadi format baku akademik yang objektif.

Otomatis menyematkan Sitasi Angka (Vancouver Style) pada kalimat yang terkait literatur dunia nyata (misal: Revolusi Industri atau Kecerdasan Buatan).

Membangun struktur Daftar Pustaka secara otomatis di bagian bawah teks.

5. Kolom Rilis Berita (Press Release)
Membangun Press Release sesuai Standar Operasional Prosedur (SOP) korporasi:

Kategori Otomatis: Deteksi pintar apakah teks masuk ke ranah Berita (Event), Peristiwa (Insiden), atau Opini.

Headline: Dibuat otomatis menggunakan kalimat aktif (SPOK), tidak clickbait, dan dibatasi maksimal 12 kata.

Dateline: Menggunakan format waktu dan lokasi yang tepat (contoh: TASIKMALAYA, 24 Juni 2026).

Kutipan Pejabat: Opini berbobot yang relevan dan tidak mengulang isi berita (memberikan sentuhan manusiawi).

Boilerplate & Media Contact: Secara otomatis menyertakan profil institusi dan narahubung resmi Humas Agung Media Corp.

🛠️ Fitur Ekspor Microsoft Word (.doc) Tingkat Lanjut
Setiap kolom hasil (Analisis, Saran, Ilmiah, PR) dilengkapi dengan tombol Download Word yang sudah dimodifikasi menggunakan struktur Microsoft Office XML. Ekspor ini akan secara paksa mengunci format dokumen hasil unduhan dengan aturan baku:

Ukuran Kertas: A4

Orientasi: Portrait

Margin Halaman: 3 cm (Atas, Bawah, Kanan, Kiri)

Perataan Teks: Rata Kanan & Kiri (Justify)

Spasi Baris: 2 (Double Space)

Jenis Font: Times New Roman (Ukuran 12pt)

Metadata Footer: Otomatis menyematkan "Copyright: Agung Baitul Hikmah - 0815-466-0328" di bagian bawah halaman Word.

💻 Teknologi yang Digunakan
Proyek ini dibangun tanpa kerangka kerja (framework) backend yang berat, mengutamakan kecepatan, dan portabilitas:

Backend: PHP 7.4+ / 8.0+ (Pemrosesan logika dinamis via POST).

Frontend UI/UX: HTML5 & Tailwind CSS (via CDN) untuk desain grid responsif dan tipografi yang elegan.

Ikonografi: FontAwesome 6 (via CDN).

Ekstraksi DOCX: Mammoth.js (Client-Side).

Ekstraksi PDF: PDF.js (Client-Side).

🚀 Cara Instalasi & Menjalankan Aplikasi
Aplikasi ini menggunakan pendekatan Single-File Application sehingga proses instalasinya sangat ringkas:

Pastikan Anda telah menginstal Local Web Server seperti XAMPP, Laragon, atau MAMP.

Aktifkan modul Apache pada Control Panel server lokal Anda.

Buat sebuah folder baru (misal: text-analyzer) di dalam direktori root server lokal Anda:

Untuk XAMPP: C:\xampp\htdocs\text-analyzer\

Untuk Laragon: C:\laragon\www\text-analyzer\

Buat file bernama index.php di dalam folder tersebut dan paste seluruh baris kode aplikasi ke dalamnya.

Buka browser (Chrome, Edge, Firefox, atau Safari).

Akses URL berikut: http://localhost/text-analyzer/

📝 Catatan Pengembang (Developer Notes)
Aplikasi ini saat ini mengimplementasikan Mock API (Simulasi Logika Pemrosesan) di dalam backend PHP menggunakan Regular Expressions (preg_split, preg_match, str_ireplace) untuk keperluan demonstrasi fungsionalitas UI/UX dan alur data secara real-time.

Untuk membawa aplikasi ini ke level produksi nyata, blok logika simulasi di bagian atas index.php (// --- LOGIKA SUMBER REAL ---) perlu diganti dengan permintaan cURL (cURL requests) yang terhubung langsung ke titik akhir API pihak ketiga (seperti OpenAI API untuk parafrase, ZeroGPT API untuk deteksi AI, dan Grammarly API untuk tata bahasa). Kredensial rahasia (API Keys) harus ditangani dengan hati-hati jika fitur tersebut diaktifkan.

https://gemini.google.com/u/3/app/886846371d621705?pageId=none
Hak Cipta © 2026 Agung Baitul Hikmah
Kontak Pengembang: WA 0815-466-0328
