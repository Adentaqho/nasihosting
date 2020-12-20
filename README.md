# nasihosting

Nasihosting v2.5
--------------------
![alt text](http://xcode.or.id/04_small-logo.png)

Script untuk mendukung otomatisasi akun hosting dengan apache server di Ubuntu Server

Nasihosting ini menggunakan PHP 7.4
-------------------------
Semua instalasi sudah dilakukan otomatis dalam program.

File manager
------------
File manager yang digunakan adalah Tiny File Manager dengan sumber dari https://github.com/prasathmani/tinyfilemanager

Penggantian password cukup pada config.php

Untuk generate password pada sistem lama sebelum versi 1.2 :
https://tinyfilemanager.github.io/docs/pwd.html

Cara menggunakan
----------------
1. git clone https://github.com/kurniawandata/nasihosting
2. cd nasihosting
3. chmod -R 777 *
4. ./nasihosting.sh (Mendukung https tapi harus sudah mempunyai sertifikat SSL, mendukung Ubuntu Server 16.04 dan Ubuntu 18.04)

   ./nasihosting-httponly.sh (Hanya mendukung http, mendukung Ubuntu Server 16.04 dan Ubuntu 18.04) 
   
   ./nasihosting-ubuntu20.04.sh (Mendukung https tapi harus sudah mempunyai sertifikat SSL, mendukung Ubuntu Server 20.04)
   
   ./nasihosting-httponly-ubuntu20.04.sh (Hanya mendukung http, mendukung Ubuntu Server 20.04) 
   
5. Jalankan perintah 1,2,3 dan 15 lalu masuk ke fastmode atau install nasihosting-extensionpack jika ingin otomatis menambah dari website dan storage-nya share.

   ./fastmode.sh (Mendukung https tapi harus sudah mempunyai sertifikat SSL, mendukung Ubuntu Server 16.04 dan Ubuntu 18.04, bisa custom nama user mysql dan database tapi tidak aman jika digabung dengan nasihosting extension-pack)

   ./fastmode-httponly.sh (Hanya mendukung http, mendukung Ubuntu Server 16.04 dan Ubuntu 18.04, bisa custom nama user mysql dan database tapi tidak aman jika digabung dengan nasihosting extension-pack)

   ./fastmode2.sh (Mendukung https tapi harus sudah mempunyai sertifikat SSL, bisa custom nama user mysql dan database dan aman jika digabung dengan nasihosting extension-pack) 

   ./fastmode2-httponly.sh (Hanya mendukung http, mendukung Ubuntu Server 16.04 dan Ubuntu 18.04, bisa custom nama user mysql dan database dan aman jika digabung dengan nasihosting extension-pack) 

   Jika ada tambahan ubuntu20.04 pada nama file maka support untuk ubuntu 20.04
   
Kompatibilitas
--------------
Nasihosting-extensionpack tidak mendukung MySQL Server dari Ubuntu Server 20.04 sehingga pilihan distro linux terbaik untuk nasihosting adalah Ubuntu Server 18.04.5 atau Ubuntu 16.04.7, karena support nasihosting-extensionpack.

Keamanan
--------
Jangan pernah menggabungkan fastmode dengan nasihosting-extensionpack, kecuali menggunakan fastmode2


Keterangan untuk non fastmode
----------
Non fastmode yaitu mode di mana semuanya semi manual hingga manual.
1. Di script ini default-nya membuat file ekstensi img 150 MB jika ingin mengubah, bisa edit scriptnya
2. Saat masuk di /etc/fstab, masukkan : /mnt/namafile.img /home/sample ext4 loop 1 2 (namafile.img bisa diganti bebas namanya asal ada ekstensi img)
3. Kata sample di atas bisa diganti dengan nama sub domain yang akan dibuat
4. Di virtualhost ganti sample dengan melakukan find dan replace all dengan nama sub domain yang akan dibuat (Jika di linux pakai nano bisa menggunakan ctrl + backslash)

Script ini telah diimplementasi
-------------------------------
Anda bisa mengakses nasihosting di https://nasihosting.com

Licensi
-------
GNU General Public License v3

Program ini dibuat oleh :
--------------------------------------------
Kurniawan. kurniawan@xcodetraining.com.
xcode.or.id


Donasi :
--------
Jika ingin donasi untuk Kurniawan

Gopay :

![alt text](http://xcodeserver.my.id/gofood.png)

![alt text](http://xcodeserver.my.id/gopay.png)

Ovo :

![alt text](http://xcodeserver.my.id/ovo3.png)

![alt text](http://xcodeserver.my.id/ovo2.png)
