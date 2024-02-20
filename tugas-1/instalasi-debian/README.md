# Instalasi Debian

1. Install file .iso dari Debian [di sini](https://www.debian.org/download).
2. Install VirtualBox [di sini](https://www.virtualbox.org/wiki/Downloads) dan jalankan setup-nya.
3. Buka VirtualBox, berikut adalah tampilannya.
   ![alt](./assets/1.png)
   Kemudian, klik "Add".
4. Kemudian, akan muncul pop-up seperti berikut.
   ![alt](./assets/2.png)
   Isi kolom "Name" dengan "Debian" dan pilih file .iso yang telah di-install sebelumnya. Kemudian, klik "Next".
5. Setelah itu, lakukan konfigurasi RAM dan CPU yang akan digunakan pada engine. Pada kasus ini, saya menggunakan RAM sebanyak 2 GB (2048 MB) dan CPU sebanyak 1. Kemudian, klik "Next".
   ![alt](./assets/3.png)
6. Selanjutnya, lakukan konfigurasi Hard Disk. Isi ukuran Hard Disk dengan 25 GB.
   ![alt](./assets/4.png)
7. Setelah seluruh konfigurasi selesai, maka akan muncul summary sebagai berikut.
   ![alt](./assets/5.png)
8. Berikut adalah tampilan home dari VirtualBox Anda setelah engine berhasil ditambahkan. Kemudian, klik tombol "Start".
   ![alt](./assets/6.png)
9. Setelah proses booting selesai, maka akan muncul tampilan berikut.
   ![alt](./assets/7.png)
   Select opsi "Graphical Install".
10. Pilih bahasa yang akan digunakan.
    ![alt](./assets/12.png)
11. Pilih lokasi.
    ![alt](./assets/13.png)
12. Pilih konfigurasi keyboard yang ingin digunakan.
    ![alt](./assets/14.png)
13. Kemudian, isi hostname untuk system. Pada kasus ini, saya mengisinya dengan "sysadmin-3122600014".
    ![alt](./assets/15.png)
14. Selanjutnya, isi domain name. Jika tidak ada, Anda dapat mengosonginya.
    ![alt](./assets/16.png)
15. Lakukan setup users dan password untuk root.
    ![alt](./assets/17.png)
16. Lakukan konfigurasi untuk user.
    ![alt](./assets/18.png)
    ![alt](./assets/19.png)
    ![alt](./assets/20.png)
17. Lakukan konfigurasi jam untuk sistem.
    ![alt](./assets/21.png)
18. Pada bagian ini, karena konfigurasi partisi akan dilakukan secara manual, maka pilih opsi "Manual".
    ![alt](./assets/22.png)
    Selanjutnya klik "Continue".
19. Selanjutnya, klik opsi berikut.
    ![alt](./assets/23.png)
20. Pilih opsi "Yes" karena kita akan membuat partisi baru.
    ![alt](./assets/24.png)
21. Selanjutnya akan muncul tampilan sebagai berikut.
    ![alt](./assets/25.png)
    Pilih opsi pri/log.
22. Pertama-pertama, kita akan membuat partisi root. Pilih opsi "Create a new partition".
    ![alt](./assets/26.png)
23. Masukkan size partisi sebesar 20 GB.
    ![alt](./assets/27.png)
24. Pada tipe partisi, pilih "Primary".
    ![alt](./assets/28.png)
25. Pilih opsi "Beginning".
    ![alt](./assets/29.png)
26. Karena partisi root diperlukan untuk booting, maka set bootable flagnya menjadi "On".
    ![alt](./assets/40.png)
27. Berikut adalah summary dari partisi root yang telah dikonfigurasi.
    ![alt](./assets/30.png)
    Jika seluruhnya summary-nya dirasa benar, pilih opsi "Done setting up the partition".
28. Selanjutnya akan diarahkan kembali pada halaman ini.
    ![alt](./assets/31.png)
    Dapat dilihat bahwa root partition yang telah dikonfigurasi sebelumnya telah berhasil dibuat.
29. Karena kita akan membuat partisi /storage, maka pilih kembali partisi yang berlabel "FREE SPACE".
30. Masukkan size dari partisi, yaitu 5 GB.
    ![alt](./assets/32.png)
31. Pilih opsi "Beginning".
    ![alt](./assets/33.png)
32. Karena kita akan menggunakan nama /storage pada mount points, maka pilih opsi "Enter Manually".
    ![alt](./assets/34.png)
    ![alt](./assets/35.png)
33. Berikut adalah summary dari partisi /storage.
    ![alt](./assets/36.png)
    Jika dirasa sudah benar, pilih opsi "Done setting up the partition".
34. Karena kita akan membuat partisi untuk swap, maka pilih kembali partisi yang berlabel "FREE SPACE".
35. Masukkan size dari partisi, yaitu 1,6 GB.
    ![alt](./assets/37.png)
36. Karena partisi ini digunakan untuk swap, ubah kolom "Use as" menjadi "Swap area".
    ![alt](./assets/38.png)
37. Berikut adalah summary dari konfigurasi partisi yang telah dilakukan.
    ![alt](./assets/39.png)
    Selanjutnya, pilih opsi "Finish partitioning and write changes to disk".
38. Tunggu proses hingga selesai.
    ![alt](./assets/41.png)
39. Kemudian, akan muncul tampilan sebagai berikut. Pilih opsi "No".
    ![alt](./assets/42.png)
40. Selanjutnya adalah melakukan konfigurasi package manager.
    ![alt](./assets/43.png)
    Pilih negara yang terdekat dengan network Anda. Pada kasus ini, saya memilih opsi "Indonesia".
41. Kemudian, pilih mirror yang terdekat dengan network dengan network Anda.
    ![alt](./assets/44.png)
    Pada kasus ini, saya memilih opsi [kebo.pens.ac.id](https://kebo.pens.ac.id).
42. Masukkan informasi proxy. Jika tidak ada, Anda dapat mengosonginya dan klik "Continue".
    ![alt](./assets/45.png)
43. Pada bagian berikut, pilih opsi "No.
    ![alt](./assets/46.png)
44. Pilih software-software yang ingin Anda install.
    ![alt](./assets/47.png)
45. Tunggu instalasi software hingga selesai.
    ![alt](./assets/48.png)
