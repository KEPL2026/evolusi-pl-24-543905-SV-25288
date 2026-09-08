# Portfolio

Aplikasi web sederhana berbasis Laravel yang digunakan untuk menampilkan portofolio dan informasi profil.

## Fitur

* Menampilkan halaman Home
* Menampilkan informasi profil melalui halaman About
* Menampilkan navigasi antarbagian halaman
* Menggunakan Laravel sebagai framework aplikasi web
* Menggunakan Vue.js untuk bagian frontend
* Menggunakan Vite untuk proses build frontend
* Continuous Integration menggunakan GitHub Actions

## Struktur Branch

Repository ini menggunakan tiga jenis branch utama dalam proses pengembangan:

* `main` — branch utama yang digunakan untuk versi final aplikasi
* `dev` — branch pengembangan dan integrasi fitur
* `feature/*` — branch yang digunakan untuk mengembangkan fitur tertentu

Alur pengembangan:

```text
feature/* → dev
dev → main
```

Setiap perubahan dilakukan melalui Pull Request dan tidak dilakukan push langsung ke branch `main`.

## Testing

Project ini menggunakan PHPUnit melalui Laravel untuk melakukan pengujian aplikasi.

Untuk menjalankan test:

```bash
php artisan test
```

Testing juga dijalankan secara otomatis melalui GitHub Actions setiap kali terjadi push atau Pull Request pada branch yang telah ditentukan.

## CI/CD

Project ini menggunakan GitHub Actions dengan workflow `CI`.

Workflow memiliki dua job:

* **Laravel Test** — melakukan instalasi dependency, build frontend, menyiapkan environment Laravel, kemudian menjalankan `php artisan test`.
* **Frontend Build** — melakukan instalasi dependency frontend dan menjalankan `npm run build` untuk memastikan proses build frontend berhasil.

Hasil workflow dapat dilihat pada bagian **Actions** di repository GitHub.

## Pull Request

Proses pengembangan menggunakan Pull Request untuk menjaga perubahan tetap terkontrol.

Pull Request yang digunakan:

1. `feature/about → dev` — penambahan halaman About.
2. `feature/ci → dev` — penambahan GitHub Actions CI.
3. `dev → main` — integrasi seluruh perubahan ke branch utama.

## Branch Protection

Branch `main` dan `dev` diberikan branch protection untuk mencegah perubahan langsung dan memastikan perubahan melalui proses Pull Request.

## Repository

Repository project:

https://github.com/KEPL2026/evolusi-pl-24-543905-SV-25288
