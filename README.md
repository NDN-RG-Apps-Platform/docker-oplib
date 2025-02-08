# User Service - Docker Setup

## Prerequisites

Sebelum memulai, pastikan kamu telah menginstal:

- [Docker Desktop](https://www.docker.com/)
- Git

## Cara Menjalankan Proyek

1. **Clone Repository**
   ```sh
   git clone https://github.com/NDN-RG-Apps-Platform/docker-oplib.git
   cd <repository-folder>
   ```

2. **Jalankan Docker Compose**
   ```sh
   docker compose up -d --build
   ```

   Opsi:
   - `-d` (detached mode): Menjalankan container di background.
   - `--build`: Membangun ulang image sebelum menjalankan container.

3. **Cek Container yang Berjalan**
   ```sh
   docker ps
   ```

4. **Menghentikan Container**
   ```sh
   docker compose down
   ```

5. **Menghapus Volume (Opsional, untuk menghapus data database)**
   ```sh
   docker compose down -v
   ```

## Notes
- Akses pgAdmin: `http://localhost:5051`
- PostgreSQL berjalan di port `5432`
- Pastikan konfigurasi database di `config.json` sesuai dengan yang ada di `docker-compose.yml`
