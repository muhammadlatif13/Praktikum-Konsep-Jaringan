---
## Muhammad Latif/3121600030
## 2 D4 IT A
---
# Post Test
### Topologi
Berikut ini adalah topologi dari sebuah jaringan yang memiliki 2 lantai.
![Topologi](https://i.postimg.cc/cL3cCYPZ/topologi.png)

Pada topologi diatas terdapat 2 buah Switch, 1 Router dan 8 PC. dimana semuanya harus saling tersambung satu sama lain dengan cara melakukan konfigurasi seperti pada gambar dibawah ini.
![Konfigurasi](https://i.postimg.cc/vZypQQSP/Konfigurasi.png)

### Konfigurasi
- Konfigurasi Router 0

![Router 0](https://i.postimg.cc/Wz5PDzY6/Konfigurasi-Router-0.jpg)

Penjelasan :
Pada gambar diatas adalah pengkonfigurasian dari Router0, pada ‘Interface f0/0.10’ saya lakukan encapsulasi dot1q 10 untuk memasukkan ip address seperti yang sudah di berikan.
Kemudian pada ‘interface f 0/0.20’ saya juga melakukan hal yang sama dengan cara melakukan encapsulasi dot1q 20 untuk memasukkan ip address sepert yang sudah diberikan.

- Konfigurasi Switch 0

![Switch0](https://i.postimg.cc/CxhdRnvX/Switch0.jpg)

Penjelasan :
Pada konfigurasi ‘Switch0’ yang pertama saya mengetikkan vlan10 kemudian diikut vlan20 kemudian memanggil masing masing Interface yang sudah tersambung untuk melakukan switchport access vlan sesuai yang sudah ditentukan oleh soal

- Konfigurasi Switch 1

![Switch1](https://i.postimg.cc/50NZvbcx/Switch1.jpg)

Penjelasan :
Sama seperti konfigurasi pada ‘Switch 0’.Pada konfigurasi ‘Switch1’ yang pertama saya mengetikkan vlan10 kemudian diikut vlan20 kemudian memanggil masing masing Interface yang sudah tersambung untuk melakukan switchport access vlan sesuai yang sudah ditentukan oleh soal