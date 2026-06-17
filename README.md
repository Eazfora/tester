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

### 3. Penyiapan Frontend (frontend-client)
```bash
cd ../frontend-client
npm install

### 4. Penyiapan AI Service (ai_service)
Sangat disarankan untuk menggunakan virtual environment agar dependensi Python tidak bentrok dengan proyek lain.
```bash
cd ../ai_service
python -m venv venv

# Aktivasi virtual environment (Windows)
venv\Scripts\activate

# Install dependensi
pip install -r requirements.txt

