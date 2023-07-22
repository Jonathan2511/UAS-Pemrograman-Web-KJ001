# UAS-Pemrograman-Web-KJ001
Project Tugas Akhir untuk memenuhi UAS Mata Kuliah Pemrograman Web Semester 4

Anggota Kelompok:
1. Agustian Prakoso (20210801027)
2. Alfino Rizky Afandie (20210801275)
3. Fajar Mahardika (20210801112)
4. Jonathan Aditya Puryanto (20210801001)
5. Rifqi Adi Prasetya (20210801024)

Cara Menjalankan Aplikasi Secara Local:
Pastikan sudah melakukan instalasi git bash, composer, laravel, XAMPP, dan lain-lain
Buka git bash / terminal lainnya dan lakukan cd ke folder program ini, setelah itu jalankan
```bash
composer update
```
Buat database mysql dengan nama example_app
Lalu jalankan
```bash
cp .env.example .env
```
Setelah itu edit file .env yang ada di folder program dan lakukan konfigurasi seperti dibawah ini
```bash
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=example_app
DB_USERNAME=root
DB_PASSWORD=

APP_NAME=Laravel
APP_ENV=local
APP_KEY=base64:QGRW4K7UVzS2M5HE2ZCLlUuiCtOIzRSfb38iWApkphE=
APP_DEBUG=true
APP_URL=http://example-app.test
```
Selanjutnya kita bisa melakukan generate key
```bash
php artisan key:generate
```
Jika sudah, kita bisa melakukan migrate database untuk pembuatan table dan seed database untuk mengisi table user dan setting
```bash
php artisan migrate && php artisan db:seed
```
Selesai!!! tinggal menjalankan aplikasinya menggunakan artisan serve atau valet
```bash
php artisan serve
```


