# Mengatur Laravel pada Xampp
Ini perngaturan bertujuan agar kita dapat menjalankan laravel ketika sudah dijalankan apache tanpa harus memakai di cli ini
```sh
php artisan serve
```
## Step-stepnya 
  - Pada direktori root (instalasi laravel) cari server.php
  - server.php ganti namanya menjadi index.php
  - Masuk ke folder public pindahkan .htdocs ke luar direktori public/ pada folder public
  - Done

Sekarang sudah bisa dibuka langsung tanpa mengunakan artisan atau membuka folder public