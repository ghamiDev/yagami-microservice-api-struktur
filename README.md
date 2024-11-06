# yagami-microservice-api-struktur
Mikroservices stuktrur dengan node js

Langkah Menjalankan Docker Compose
Pastikan Docker dan Docker Compose Terinstal
Jika belum, instal Docker terlebih dahulu di sistem Anda. Untuk menginstal Docker dan Docker Compose, ikuti petunjuk di docker.com.

Arahkan ke Direktori Project
Buka terminal atau command prompt, lalu navigasikan ke direktori project Anda di mana file docker-compose.yml berada.

bash
cd path/to/your/project
Jalankan Docker Compose
Untuk memulai semua layanan secara bersamaan, gunakan perintah berikut:

bash
docker-compose up
Catatan: Perintah di atas akan menampilkan log dari setiap kontainer ke terminal. Ini berguna untuk melihat apakah ada masalah saat layanan dimulai.

Jalankan Docker Compose di Background (Opsional)
Jika Anda ingin menjalankan Docker Compose di background tanpa menampilkan log di terminal, tambahkan opsi -d (detached mode):

bash
docker-compose up -d
Perintah ini memungkinkan Anda melanjutkan kerja di terminal tanpa terpengaruh oleh log Docker Compose.

Cek Layanan yang Berjalan
Anda bisa memeriksa kontainer yang sedang berjalan dengan perintah:

bash
docker ps
Ini akan menampilkan daftar kontainer yang berjalan, bersama dengan nama dan port yang dipetakan.

Menghentikan Semua Layanan
Untuk menghentikan semua layanan, gunakan perintah berikut:

bash
docker-compose down
Perintah ini akan menghentikan dan menghapus semua kontainer yang dibuat oleh docker-compose up.

Menghapus Volume dan Jaringan (Opsional)
Jika Anda ingin menghapus semua volume dan jaringan yang dibuat oleh Docker Compose untuk project ini, gunakan:

bash
docker-compose down -v
Troubleshooting
Jika ada error saat build, pastikan setiap service memiliki Dockerfile yang benar.
Pastikan juga port yang digunakan setiap service tidak bentrok dengan aplikasi lain yang berjalan di sistem Anda.
Dengan perintah docker-compose up dan docker-compose down, Anda dapat dengan mudah mengelola layanan-layanan mikroservice di dalam lingkungan terisolasi.