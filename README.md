# OmniSight BI - Capstone Project (PJK-GM017)


OmniSight BI adalah aplikasi *Business Intelligence* *Full Stack* yang dirancang untuk membantu pengelolaan bisnis dengan dukungan AI. Proyek ini terdiri dari tiga komponen utama:
- **Frontend Client** (React/Vite)
- **Backend Service** (NestJS & Prisma)
- **AI Service** (Python/FastAPI)


---


## 🛠️ Persyaratan Sistem
Sebelum menjalankan proyek ini, pastikan Anda telah menginstal:
- **Node.js** (Versi LTS disarankan)
- **Python** (Versi 3.8 atau lebih baru)
- **Git** (opsional)


---


## 🚀 Cara Instalasi dan Penyiapan Proyek


1. **Kloning atau Unduh Repositori**
   Buka terminal, lalu arahkan ke folder proyek ini.


2. **Penyiapan Backend (`backend-service`)**
   ```bash
   cd backend-service
   npm install
   ```


3. **Penyiapan Frontend (`frontend-client`)**
   ```bash
   cd ../frontend-client
   npm install
   ```


4. **Penyiapan AI Service (`ai_service`)**
   Sangat disarankan untuk menggunakan *virtual environment*.
   ```bash
   cd ../ai_service
   python -m venv venv
   venv\Scripts\activate
   pip install -r requirements.txt
   ```


---


## 💻 Petunjuk Penggunaan


Cara paling mudah untuk menjalankan keseluruhan proyek ini di sistem operasi Windows adalah dengan menggunakan script `start_all.bat`.


1. Klik ganda (double click) file `start_all.bat` yang ada di root folder proyek ini.
2. Script ini secara otomatis akan:
   - Membersihkan port `3000` dan `8000` jika sedang digunakan.
   - Melakukan sinkronisasi *database* Prisma dan proses *seeding* data awal.
   - Melatih ulang (*training*) model Machine Learning.
   - Menjalankan **Backend Service** (Port 3000).
   - Menjalankan **AI Service** (Port 8000).
   - Menjalankan **Frontend Client** (Port 5173).


### Akses Aplikasi
Setelah semua servis berhasil dijalankan, Anda dapat mengakses:
- **Frontend / UI:** `http://localhost:5173`
- **Backend API:** `http://localhost:3000`
- **AI API:** `http://localhost:8000`


### Kredensial Login (Default)
Gunakan kredensial berikut untuk masuk sebagai administrator:
- **Email:** `admin@omnisight.com`
- **Password:** `admin123`


---


## 📌 Informasi Penting Lainnya


- **Database:** Proyek ini menggunakan Prisma ORM. Script `start_all.bat` menggunakan perintah `--accept-data-loss` saat melakukan push skema. Berhati-hatilah jika ada data penting di environment lokal Anda.
- **Port Bentrok:** Jika servis gagal berjalan, pastikan port `3000`, `5173`, dan `8000` tidak diblokir oleh antivirus atau aplikasi lain.
- **Model Machine Learning:** AI Service akan secara otomatis memproses dan melatih model dengan sekitar 20.000 baris data dummy saat pertama kali dijalankan oleh script.


