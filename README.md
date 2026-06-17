# 📊 OmniSight BI - Capstone Project (PJK-GM017)

> **OmniSight BI** adalah aplikasi *Business Intelligence* yang dirancang untuk membantu pengelolaan bisnis dengan dukungan AI secara cerdas dan efisien.

![Frontend](https://img.shields.io/badge/Frontend-React%20%7C%20Vite-blue?style=flat-square&logo=react)
![Backend](https://img.shields.io/badge/Backend-Nest.JS%20%7C%20Prisma-red?style=flat-square&logo=nestjs)
![AI Service](https://img.shields.io/badge/AI-Python%20%7C%20FastAPI-green?style=flat-square&logo=python)

Proyek ini mengintegrasikan tiga komponen utama untuk memberikan visualisasi data dan wawasan prediktif:
- 🌐 **Frontend Client** (React / Vite)
- ⚙️ **Backend Service** (Nest.JS & Prisma)
- 🤖 **AI Service** (Python / FastAPI)

---

## 🛠️ Persyaratan Sistem

Sebelum menjalankan proyek ini, pastikan mesin Anda telah terinstal:
* **[Node.js](https://nodejs.org/en/download/)** (Disarankan versi LTS)
* **[Python](https://www.python.org/downloads/)** (Versi 3.8 atau lebih baru)
* **[Git](https://git-scm.com/downloads)** (Opsional, untuk kloning repositori)

---

## 🚀 Cara Instalasi dan Penyiapan Proyek

### 1. Kloning Repositori
Buka terminal Anda, lalu arahkan ke folder tempat Anda ingin menyimpan proyek ini.
```bash
git clone https://github.com/ZaxkyyOfficial/Capstone_Project-PJK-GM017.git
cd omnisight-bi
```

### 2. Penyiapan Backend (`backend-service`)
```bash
cd backend-service
npm install
```

### 3. Penyiapan Frontend (frontend-client)
```bash
cd ../frontend-client
npm install
```

### 4. Penyiapan AI Service (ai_service)
Sangat disarankan untuk menggunakan virtual environment agar dependensi Python tidak bentrok dengan proyek lain.
```bash
cd ../ai_service
python -m venv venv

# Aktivasi virtual environment (Windows)
venv\Scripts\activate

# Install dependensi
pip install -r requirements.txt
```

### 💻 Petunjuk Penggunaan

Cara paling mudah dan praktis untuk menjalankan keseluruhan proyek ini di Windows adalah dengan menggunakan script otomatis yang telah disediakan.

1. Pastikan Anda berada di *root folder* proyek.
2. Klik ganda (*double click*) file `start_all.bat`.

Script `start_all.bat` akan secara otomatis melakukan:
* 🧹 Membersihkan port 3000 dan 8000 (jika sedang digunakan).
* 🗄️ Melakukan sinkronisasi database Prisma dan *seeding* data awal.
* 🧠 Melatih ulang (*training*) model Machine Learning dengan data *dummy*.
* 🚀 Menjalankan Backend Service (Port 3000).
* 🚀 Menjalankan AI Service (Port 8000).
* 🚀 Menjalankan Frontend Client (Port 5173).

---

### 🌐 Akses Aplikasi

Setelah terminal menunjukkan semua servis berhasil dijalankan, Anda dapat mengakses:

| Layanan | URL Akses |
| :--- | :--- |
| **Frontend / UI Dashboard** | http://localhost:5173 |
| **Backend API** | http://localhost:3000 |
| **AI API** | http://localhost:8000 |

---

### 🔐 Kredensial Login (Default)

Untuk masuk ke dalam dashboard sebagai administrator, gunakan akses berikut:
* **Email:** `admin@omnisight.com`
* **Password:** `admin123`

---

### 📌 Informasi Penting Lainnya

⚠️ Harap perhatikan beberapa hal berikut saat mengembangkan atau menjalankan proyek:

* **Database (Prisma ORM):** Script `start_all.bat` mengeksekusi perintah dengan flag `--accept-data-loss` saat melakukan *push* skema. Berhati-hatilah jika Anda memiliki data penting di *environment* lokal Anda, karena data tersebut mungkin akan tertimpa dan hilang.
* **Konflik Port:** Jika ada layanan yang gagal berjalan, pastikan port 3000, 5173, dan 8000 dalam keadaan kosong dan tidak diblokir oleh Firewall atau aplikasi lain (seperti antivirus).
* **Model Machine Learning:** Saat pertama kali dijalankan oleh script, AI Service akan memakan waktu sejenak untuk memproses dan melatih model menggunakan sekitar 20.000 baris data *dummy*. Mohon tunggu hingga proses selesai.


