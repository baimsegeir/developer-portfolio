# Final Project: Cloud Full-Stack Deployment
## Cara Menjalankan (Local & Docker)
## CI/CD Pipeline
## Deployment
## Author
# Cloud Full-Stack Deployment – Developer Portfolio

## 📖 Deskripsi Project
Project ini merupakan implementasi **Full-Stack Application** yang dideploy ke **Google Cloud Platform (GCP)** menggunakan **Docker** dan **CI/CD GitHub Actions**.

Project dibuat untuk memenuhi **Final Project Cloud / DevOps**, dengan fokus pada:
- Deployment aplikasi ke cloud
- Otomatisasi build menggunakan CI/CD
- Penerapan best practice DevOps
- Dokumentasi teknis yang rapi

---

## 🛠️ Teknologi yang Digunakan
- **Node.js 20**
- **Next.js**
- **Docker & Docker Compose**
- **GitHub Actions (CI/CD)**
- **Google Cloud Platform (Compute Engine VM)**
- **Linux (Red Hat-based OS)**

---

## 🏗️ Arsitektur Singkat
Developer → GitHub Repository
↓
GitHub Actions (CI/CD)
↓
Docker Build Image
↓
GCP VM (Docker Container)
↓
Public Access (IP)

---

## ▶️ Cara Menjalankan Aplikasi

### 1️⃣ Menjalankan Secara Local (Non-Docker)
npm install
npm run dev
akses : http://localhost:3000
2️⃣ Menjalankan Menggunakan Docker
docker-compose up -d --build
Akses aplikasi: http://<IP_VM_GCP>
🔁 CI/CD Pipeline (GitHub Actions)
Pipeline otomatis dijalankan setiap kali terjadi push ke branch main.
Tahapan pipeline:
Checkout source code
Setup Node.js 20
Install dependency
Build aplikasi
Build Docker image
File pipeline: .github/workflows/ci-cd.yml
Link pipeline: https://github.com/baimsegeir/developer-portfolio/actions
☁️ Deployment
Aplikasi dideploy ke Google Cloud Compute Engine VM menggunakan Docker Container.
OS VM: Red Hat-based Linux
Container exposed via port 80
Firewall GCP dikonfigurasi untuk akses publik
Akses aplikasi: http://<IP_VM_GCP>


👤 Author
Ibrahim Segeir
GitHub: https://github.com/baimsegeir
