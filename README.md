# nasihosting

Nasihosting v1.8
--------------------
![alt text](http://xcode.or.id/04_small-logo.png)

Script untuk mendukung otomatisasi akun hosting dengan apache server di Ubuntu Server

Jangan menggunakan PHP di bawah versi 7.4
-------------------------
Jangan install PHP di bawah versi 7.4, jika punya server, pastikan install php 7.4, instalasi PHP 7.4 sudah disertakan dalam program,  jika anda sudah pakai PHP versi sebelumnya maka lakukan remove dan pastikan nanti PHP 7.4 yang berjalan.

File manager
------------
File manager yang digunakan adalah Tiny File Manager dengan sumber dari https://github.com/prasathmani/tinyfilemanager

Penggantian password cukup pada config.php

Untuk generate password pada sistem lama sebelum versi 1.2 :
https://tinyfilemanager.github.io/docs/pwd.html

Cara menggunakan
----------------
1. apt install apache2
2. apt install mysql-server
3. mysql lalu enter, lalu diisi : ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'passwordroot';
4. git clone https://github.com/kurniawandata/nasihosting
5. cd nasihosting
6. chmod -R 777 *
7. ./nasihosting.sh
8. Jika sudah tidak ada masalah dengan nasihosting.sh, seperti sudah menggunakan PHP 7.4 dan sebagainya yang diperlukan maka bisa menggunakan fast mode untuk membuat akun hosting, cara penggunaannya cukup ketik ./fastmode.sh lalu enter (Jangan lupa jika tidak ingin menggunakan default storage untuk client 125.62 MB (150 MB di program) maka edit programnya).


Keterangan
----------
1. Di script ini default-nya membuat file ekstensi img 150 MB jika ingin mengubah, bisa edit scriptnya
1. Saat masuk di /etc/fstab, masukkan : /mnt/namafile.img /home/sample ext4 loop 1 2 (namafile.img bisa diganti bebas namanya asal ada ekstensi img)
3. Kata sample di atas bisa diganti dengan nama sub domain yang akan dibuat
4. Di virtualhost ganti sample dengan melakukan find dan replace all dengan nama sub domain yang akan dibuat (Jika di linux pakai nano bisa menggunakan ctrl + backslash)

Script ini telah diimplementasi
-------------------------------
Anda bisa mengakses nasihosting di https://nasihosting.com

Demo video
----------
https://www.youtube.com/watch?v=sbM_NbdWWeg


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
