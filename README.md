# UTS Praktikum UDB
NIM: 240104010

## Deskripsi
Project ini merupakan UTS praktikum yang mengintegrasikan Git, Docker, MySQL,
PostgreSQL, Adminer, dan ZeroTier dengan fokus pada isolasi network Docker
dan kontrol akses database menggunakan ZeroTier.

## Konfigurasi Network
- Custom bridge network: 172.30.10.0/24
- Static IP untuk setiap container
- Database tidak diekspos ke publik
- Adminer diakses melalui ZeroTier

## Service
- MySQL (uts_mysql) → 172.30.10.10
- PostgreSQL (uts_postgres) → 172.30.10.20
- Adminer (uts_adminer) → Port 8010

## Kesimpulan
Dengan penggunaan Docker network dan ZeroTier, akses database dapat
dikontrol secara aman dan terisolasi.
