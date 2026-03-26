# Progress 1: Simple LMS - Docker & Django Foundation

## Langkah-langkah Menjalankan Project
## 1. Clone Repository

- git clone (https://github.com/Nazla44/simple-lms.git)

## 2. Jalankan Docker 

- docker-compose up -d --build

<img width="1339" height="942" alt="Screenshot 2026-03-26 120425" src="https://github.com/user-attachments/assets/bdf1305d-ab95-4ad8-b819-12e8d2d5994d" />
<img width="1393" height="483" alt="Screenshot 2026-03-26 120432" src="https://github.com/user-attachments/assets/b140418a-d885-4b8f-88c1-655329c541d9" />

## 3. Verifikasi Container Berjalan

- docker ps 

<img width="1911" height="204" alt="Screenshot 2026-03-26 120632" src="https://github.com/user-attachments/assets/c33a310d-cac4-4a45-b01d-6aea067e4215" />

## 4. Akses Aplikasi

Buka browser dan akses: http://localhost:8000
<img width="1911" height="1018" alt="Screenshot 2026-03-26 120535" src="https://github.com/user-attachments/assets/77217aef-f63f-465d-abc3-0a07765dabb5" />

## 5. Stop Project
- docker compose down

# Environment Variables yang Digunakan

Berikut ini adalah konfigurasi yang digunakan dalam file .env :
<img width="723" height="163" alt="Screenshot 2026-03-26 134816" src="https://github.com/user-attachments/assets/81c0b238-aa76-434b-acd9-4cfdd13289cc" />

Penjelasan:
- Debug: untuk mengaktifkan mode debug pada Django. True digunakan untuk development.
- SECRET_KEY: Kunci rahasia Django yang digunakan untuk keamanan aplikasi seperti session dan CSRF.
- ALLOWED_HOSTS: Daftar host yang diizinkan untuk mengakses aplikasi.
- DATABASE_URL: Konfigurasi koneksi PostgreSQL dalam format URL dengan detail (username & password: postgres, hostname database, port PostgreSQL yaitu 5432, dan nama DB adalah lms_db)
- REDIS_URL: URL koneksi Redis

