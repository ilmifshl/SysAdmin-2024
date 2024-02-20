# Penjelasan File /etc/group pada Debian

## Fungsi
File `/etc/group` pada Debian adalah file konfigurasi yang menyimpan informasi tentang grup-grup pengguna di sistem. Ini memungkinkan administrator untuk mengelola grup-grup pengguna dengan memberikan akses tertentu ke berbagai sumber daya dan layanan di sistem.

## Format
Setiap baris dalam file `/etc/group` memiliki format yang terdiri dari empat bidang yang dipisahkan oleh titik dua (`:`), seperti berikut:

`nama_grup:kata_sandi:ID_grup:anggota_grup`

- **nama_grup**: Nama grup yang diberikan.
- **kata_sandi**: Kata sandi grup, biasanya terenkripsi (ditandai dengan "x") karena sandi sebenarnya disimpan di `/etc/gshadow`.
- **ID_grup**: ID numerik unik yang terkait dengan grup.
- **anggota_grup**: Daftar pengguna yang menjadi anggota grup tersebut, dipisahkan oleh koma.

## Penggunaan
Perintah `less /etc/group` digunakan untuk melihat isi dari file `/etc/group` secara bertahap. Ini memungkinkan administrator untuk memeriksa konfigurasi grup, menambahkan atau menghapus grup, serta mengelola anggota grup di sistem Debian.

