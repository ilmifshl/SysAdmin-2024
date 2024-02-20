# Perintah `su` dan `su -` pada Debian

## Perintah su:

**Penjelasan:**

Perintah su adalah singkatan dari "switch user" atau "substitute user". Perintah ini digunakan untuk beralih ke pengguna lain, biasanya pengguna root, dengan memasukkan kata sandi pengguna yang dituju. Ketika menggunakan su, Anda akan menjalankan shell dengan hak akses dan lingkungan pengguna baru tanpa mengatur ulang beberapa variabel lingkungan.

**Perbedaan:**

Saat menggunakan su, shell tidak dimuat ulang sepenuhnya dengan lingkungan baru. Variabel lingkungan dan direktori kerja saat ini dari pengguna yang sedang aktif mungkin tetap sama setelah beralih ke pengguna baru. Ini berguna ketika Anda hanya perlu melaksanakan beberapa tugas sebagai pengguna lain tanpa perlu sepenuhnya beralih ke lingkungan pengguna tersebut.

## Perintah su -:

**Penjelasan:**

Perintah su - atau su -l adalah singkatan dari "switch user with login shell" atau "substitute user with login shell". Ini melakukan hal yang sama seperti su, yaitu beralih ke pengguna lain, biasanya pengguna root, tetapi juga memuat ulang shell dengan lingkungan pengguna baru sepenuhnya.

**Perbedaan:**

Saat menggunakan su -, shell dimuat ulang sepenuhnya dengan lingkungan baru, termasuk variabel lingkungan, direktori kerja, dan hak akses yang sesuai dengan pengguna baru. Variabel lingkungan, direktori kerja, dan hak akses baru sepenuhnya diberikan kepada pengguna baru yang dituju. Ini berguna ketika Anda perlu sepenuhnya bekerja dalam lingkungan pengguna baru, seperti saat bekerja sebagai pengguna root dengan hak akses penuh.

## Kesimpulan:

Jadi, perbedaan utama antara su dan su - terletak pada pembaruan lingkungan shell. Saat menggunakan su -, lingkungan shell sepenuhnya dimuat ulang dengan lingkungan pengguna baru, sementara su hanya beralih pengguna tanpa mengubah lingkungan shell sepenuhnya. Ini memberikan fleksibilitas dalam penggunaan, di mana Anda dapat memilih antara menjalankan perintah sebagai pengguna lain tanpa mengubah lingkungan shell atau sepenuhnya beralih ke lingkungan pengguna baru dengan hak akses dan variabel lingkungan yang sesuai.
