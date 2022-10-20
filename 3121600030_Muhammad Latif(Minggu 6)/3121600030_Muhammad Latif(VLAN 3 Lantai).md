# VLAN 3 LANTAI
## Muhammad Latif/3121600030
## 2 D4 IT A

## Topologi
Pengunaan VLAN untuk 3 VLAN yang berbeda. Untuk skema yang saya berikan merupakan skema 3 lantai dengan 3 switch dan 1 router dan 3 vlan sehinga setiap vlan dapat menghubungi satu vlan dan tidak dengan vlan yang lain. Di bawah ini merupakan contoh skema topologi yang saya gunakan.
![](https://i.ibb.co/qCbHbxs/Whats-App-Image-2022-10-01-at-11-24-29.jpg)

## Konfigurasi Router
Router 1 Fungsi router pada komunikasi antar vlan ialah, menyambungkan user client satu dengan user client yg lain dengan mengunakan gateway dan proses ecapsulation.

![](https://i.ibb.co/5Rx8K3v/Whats-App-Image-2022-10-01-at-11-35-34.jpg)

## Konfigurasi Switch
Selanjutnya kita setting pada pada Switch. untuk setting nya kita perlu setting pada Switch untuk mendaftarkan vlan dan mendaftarkan setiap port untuk di daftarkan pada setiap port seperti gambar dibawah

![](https://i.ibb.co/VxN0g3m/Whats-App-Image-2022-10-01-at-14-11-48.jpg)
![](https://i.ibb.co/StX4zy8/Whats-App-Image-2022-10-01-at-11-31-07.jpg)

Untuk port 4 pada switch1 dan 3 menggunakan trunk agar bisa mengakses switch lainnya. Sedangkan untuk switch2 port 4,5,6 menggunakan trunk agar bisa mengakses ke2 switch lainnya

![](https://i.ibb.co/QbxrSVs/Whats-App-Image-2022-10-01-at-11-32-08.jpg)

## Konfigurasi IP PC
Saya menggunakan VLAN10 untuk PC admin, VLAN20 untuk PC Developer, dan VLAN30 untuk PC Management dengan konfigurasi IP : 
192.168.10.1 - VLAN10
172.17.20.1 - VLAN20
118.18.30.1 - VLAN30
Sebagai contoh seperti gambar dibawah
![](https://i.ibb.co/5RtfwRg/Whats-App-Image-2022-10-01-at-11-27-35.jpg)
![](https://i.ibb.co/VYbpgr8/Whats-App-Image-2022-10-01-at-11-29-04.jpg)
![](https://i.ibb.co/NNVdy2W/Whats-App-Image-2022-10-01-at-11-29-59.jpg)

## Test Ping
percobaan melakukan test ping dari PC Admin1 ke Admin2

![](https://i.ibb.co/QkWk0qC/Whats-App-Image-2022-10-01-at-11-33-35.jpg)