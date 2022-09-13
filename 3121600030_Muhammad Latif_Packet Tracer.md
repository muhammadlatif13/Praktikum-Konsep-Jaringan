## Muhammad Latif / 3121600030
## 2 D4 IT A
#
#
## Laporan Praktikum Packet Tracer



Packet Tracer adalah simulator alat-alat jaringan Cisco yang sering digunakan sebagai media pembelajaran dan pelatihan, dan juga dalam bidang penelitian simulasi jaringan komputer.

Fungsi dari packet tracer yaitu mernacang sebuah system atau topologi jaringan yang akan diterapkan pada dunia nyata atau kerja.

## Topologi 
![Gambar Toplogi](https://i.postimg.cc/gJg9rT2M/Topologi.png)
Pada gambar diatas, mterdapat 3 buah pc yang sudah disambungkan pada 1 HUB. Setiap PC memiliki IP yang berbeda beda seperti pada gambar dibawah ini

- IP PC-0
![IP PC-0](https://i.postimg.cc/CKKXX4Nk/IP-PC-0.png)
- IP PC-1
![IP PC-1](https://i.postimg.cc/632S55FQ/IP-PC-1.png)
- IP PC-2
![IP PC-2](https://i.postimg.cc/vmD23ZYv/IP-PC-2.png)

Setelah selesai mengatur IP pada masing-masing PC, selanjutnya yaitu melakukan testin.

## Testing 1: PC-0 - PC-1
Pada testing 1, kita melakukan ping IP milik PC-1 dengan menggunakan Command Prompt PC-0 dengan posisi Simulation Panel off.
#
- Langkah pertama yaitu check ARP pada PC-0
![Check ARP](https://i.postimg.cc/Fz2hsBTM/check-ARP-PC-0.png)
- Langkah kedua melakukan ping IP PC-1 melalui Command Prompt PC-0
![Ping PC-1 dari PC-0](https://i.postimg.cc/rwH76rYH/ping-IP-PC1-from-PC-0.png)
- Maka jika dilihat dari simulasinya, awal pesan akan terbentuk di Layer 2.
![](https://i.postimg.cc/fLVxGVp8/Layer1.png)
#
- Karena MAC IP Address Destinationnya belum ditemukan, maka PC-0 mengirimkan broadcast dengan address FFFF.FFFF.FFFF
![](https://i.postimg.cc/65Xv0bWj/Layer2.png)

## Testing 2 : PC-0 - PC-1
Pada testing ke-2 ini, sama saja seperti testing ke-1. Yang membedakan yaitu Simulation Panel. Pada testing ke-2 kita akan menyalakan Simulation Panelnya.

- Langkah pertama yaitu buka command prompt, kemudian lakukan ping IP PC-1 menggunakan Command Prompt PC-0
![](https://i.postimg.cc/zvj2BbDT/Screenshot-from-2022-09-13-08-38-27.png)
- Setelah dilakukan ping, maka Topologinya akan seperti gambar berikut.
![](https://i.postimg.cc/MTwYQ6F5/Screenshot-from-2022-09-13-08-38-10.png)
Setelah dilakukan ping dengan posisi Simulation Panel dinyalakan, maka akan muncul ARP.
![](https://i.postimg.cc/CxjBfGpy/Screenshot-from-2022-09-13-08-40-54.png)
Karena disini ARP-nya sudah muncul, maka PC-0 tidak akan melakukan broadcast lagi seperti pada saat pertama kali mencari MAC Destination. Berikut hasil Outbound dari paket ARP pada Testing ke-2 ini.
![](https://i.postimg.cc/J72TzkLc/Outbound-PC-1.png)
#

## Testing 3 : PC-1 - PC-0
Sama seperti testing diatas, namun sekarang kita akan melakukan testing dari PC-1 dengan memanggil IP PC-0
- Langkah pertama yaitu melakukan check ARP-nya, kemudian melakukan ping dengan menuliskan IP PC-0
![](https://i.postimg.cc/hj3HnZsV/Screenshot-from-2022-09-13-08-55-17.png)
Karena ARP-nya sudah ada, maka PC-1 tidak akan melakukan broadcast lagi seperti saat pertama kali mencari MAC Destination. berikut isi dari paket ARP pada Testing ke-3.
![](https://i.postimg.cc/DwZpvPWg/Screenshot-from-2022-09-13-08-53-12.png)