# Jarkom_modul2_praktikum_C12

## Kelompok C12
* 05111840000146 - [I Kadek Ricky Suirta](https://github.com/riclown)
* 05111840000162 - [Fransiskus Xaverius Kevin Koesnadi](https://github.com/fxkevink)

## Daftar Isi
* [Soal DNS](#dns-soal-1---7)
* [Soal 1](#soal-1)
* [Soal 2](#soal-2)
* [Soal 3](#soal-3)
* [Soal 4](#soal-4)
* [Soal 5](#soal-5)
* [Soal 6](#soal-6)
* [Soal 7](#soal-7)
* [Soal Web Server](#web-server-soal-8---17)
* [Soal 8](#soal-8)
* [Soal 9](#soal-9)
* [Soal 10](#soal-10)
* [Soal 11](#soal-11)
* [Soal 12](#soal-12)
* [Soal 13](#soal-13)
* [Soal 14](#soal-14)
* [Soal 15](#soal-15)
* [Soal 16](#soal-16)
* [Soal 17](#soal-17)

## DNS (Soal 1 - 7)

## Soal 1
Buka uml *MALANG* dan update package list `apt-get update` dan lakukan proses instalasi bind9 dengan perintah `apt-get install bind9 -y`.

Lakukan perintah pada uml *MALANG* `nano /etc/bind/named.conf.local` dan isi konfigurasi pada **semeruc12.pw** dengan syntax
```
zone "semeruc12.pw" {
	type master;
	file "/etc/bind/jarkom/semeruc12.pw";
};
```
![Img 1](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/1.0.jpg)

Buat folder **jarkom** di dalam /etc/bind `mkdir /etc/bind/jarkom`

Copykan file db.local pada path /etc/bind ke dalam folder jarkom yang baru saja dibuat dan ubah namanya menjadi **semeruc12.pw** `cp /etc/bind/db.local /etc/bind/jarkom/jarkom2020.com`

Kemudian buka file `semeruc12.pw` dan edit

![Img 2](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/1.1.jpg)

Lalu restart bind9 `service bind9 restart`. Pada client *GRESIK* dan *SIDOARJO* edit file **resolv.conf** dengan mengetikkan perintah `nano /etc/resolv.conf`

![Img 3](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/1.2.jpg)
![Img 4](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/1.4.jpg)

Lakukan `ping semeruc12.pw`

![Img 5](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/1.3.jpg)
![Img 6](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/1.5.jpg)


## Soal 2

Buka file `semeruc12.pw` pada uml MALANG, dan masukan konfigurasi

![Img 7](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/2.0.jpg)

Lakukan `service bind9 restart` dan cek **ping www.semeruc12.pw** atau **host -t CNAME www.semeruc12.pw** dari uml *GRESIK*

![Img 8](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/2.1.jpg)
![Img 9](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/2.2.jpg)


## Soal 3

Edit file **/etc/bind/jarkom/semeruc12.pw** dengan
```
nano /etc/bind/jarkom/semeruc12.pw
```
Serta lakukan konfigurasi pada file tersebut

![Img 10](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/3.0.jpg)

Setelah itu lakukan `service bind9 restart` dan ping dari *GRESIK* yaitu `ping penanjakan.semeruc12.pw` atau `host -t CNAME penanajakan.semeruc12.pw`

![Img 11](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/3.1.jpg)
![Img 12](https://github.com/riclown/Jarkom_modul2_praktikum_C12/blob/main/img/3.2.jpg)

## Soal 4

## Soal 5

## Soal 6

## Soal 7

## Web Server (Soal 8 - 17)

## Soal 8


## Soal 9

## Soal 10


## Soal 11


## Soal 12


## Soal 13


## Soal 14


## Soal 15

## Soal 16

## Soal 17

### Kendala yang  dihadapi saat pengerjaan
