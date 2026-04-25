# SIAM - Sistem Informasi Aspirasi Mahasiswa 🎓

**SIAM** adalah platform transparansi digital yang dirancang untuk menjembatani komunikasi antara mahasiswa dan pihak birokrasi kampus Universitas Muhammadiyah Malang. Proyek ini berfokus pada efisiensi penyampaian keluhan, saran, dan pemantauan solusi secara real-time.

---

## 🚀 Fitur Utama
Berdasarkan perancangan pada *Daily Project 6*, platform ini mengimplementasikan 5 pilar fungsional:

1.  **Status Tracking Real-Time**: Mahasiswa mendapatkan transparansi penuh atas progres aspirasi (Dikirim → Diverifikasi → Diproses → Selesai).
2.  **Voting & Prioritas**: Sistem dukungan publik untuk membantu Admin mengidentifikasi isu yang paling mendesak bagi massa mahasiswa.
3.  **Klasifikasi Otomatis (Rule-Based)**: Pengelompokan cerdas ke kategori Akademik atau Fasilitas berdasarkan deteksi kata kunci.
4.  **Dashboard Transparansi & Statistik**: Visualisasi data bagi pihak manajemen untuk memantau performa layanan.
5.  **Rating & Feedback Solusi**: Ruang evaluasi bagi mahasiswa untuk menilai kualitas penyelesaian masalah oleh staf.

---

## 📊 Perbandingan Uji Aplikasi (Aspek Kualitas)

Tabel berikut menunjukkan hasil pengujian fungsionalitas aplikasi dibandingkan dengan target desain awal:

| Aspek Kualitas / Fitur | Target Desain (Daily Project 6) | Hasil Pengujian (Uji Aplikasi) | Status |
| :--- | :--- | :--- | :--- |
| **Real-Time Tracking** | Sinkronisasi status aspirasi secara instan antar aktor. | Database Listener Firestore berhasil melakukan update status tanpa refresh halaman. | **PASS** |
| **Voting System** | Mekanisme dukungan publik untuk penentuan prioritas isu. | Fungsi *Asynchronous Increment* berhasil mengakomodasi akumulasi dukungan secara masif (High Engagement). | **PASS** |
| **Akurasi Klasifikasi** | Kategorisasi otomatis berbasis deteksi kata kunci teks. | Logika *Conditional Rule-Based* berhasil memetakan aspirasi ke kategori yang sesuai secara otomatis. | **PASS** |
| **Transparansi Data** | Visualisasi tren masalah melalui dashboard statistik terpusat. | Integrasi Chart.js berhasil merender grafik distribusi status berdasarkan data riil dari Firestore. | **PASS** |
| **Feedback Mechanism** | Pengumpulan rating kepuasan layanan setelah solusi diberikan. | Validasi *UI Conditional Rendering* berhasil menampilkan form rating hanya pada aspirasi berstatus "Selesai". | **PASS** |

---

## 🛠️ Arsitektur Teknologi
* **Frontend**: HTML5, Tailwind CSS (Modern & Responsive UI).
* **Backend & Auth**: Firebase Authentication (Institutional Email Validation).
* **Database**: Firebase Firestore (NoSQL Real-time Database).
* **Analytics**: Chart.js (Data Visualization).

## 👥 Aktor Sistem
* **Mahasiswa**: Mengirim aspirasi, memberikan voting dukungan, dan menilai solusi.
* **Staff**: Memberikan feedback jawaban dan melakukan eksekusi solusi.
* **Admin**: Mengelola seluruh data, memantau statistik, dan mengatur hak akses (CRUD data).

---

## 📦 Instalasi & Jalankan Lokal
1.  Clone repository ini:
    ```bash
    git clone https://github.com/ErkPH/SIAM-DAILY7.git
    ```
2.  Buka file `index.html` di browser (atau gunakan Live Server di VS Code).
3.  Pastikan koneksi internet aktif untuk memuat library Firebase dan Tailwind.

---

### 🔗 Tautan Terkait
* **Live Demo (Hosting)**: https://siam-kampus.web.app
* **Developer**: Erik Putra Hernanda (23-250) - Teknik Informatika Universitas Muhammadiyah Malang.