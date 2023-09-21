Jarkom-Modul-1-B19-2023

Laporan Resmi Praktikum Jaringan Komputer Modul 1 

## 1
### Soal
```
User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file
a. Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut? 
b. Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut? 
c. Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
d. Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
```
### Pengerjaan
## 2
### Soal
```
Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!
```
### Pengerjaan
## 3
### Soal
```
Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?
b. Protokol layer transport apa yang digunakan?.
```
### Pengerjaan
## 4
### Soal
```
Berapa nilai checksum yang didapat dari header pada paket nomor 130?
```
### Pengerjaan
## 5
### Soal
```
Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.
a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut?
b. Port berapakah pada server yang digunakan untuk service SMTP?
c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?
```
### Pengerjaan
```
Langkah pertama adalah menemukan password dari zip file.
```

<img width="1338" alt="Screenshot 2023-09-22 at 00 01 08" src="https://github.com/YudisthiraPutra/Jarkom-Modul-1-B19-2023/assets/114007340/3e3636f8-b33a-4d4c-9448-30653dff9318">

```
Dengan melakukan filter paket dengan kata “pass” kita mendapatkan sebuah packet. Kemudian packet tersebut
di follow dan pada bagian bawah terdapat pesan di atas.
kemudian kita decrypt dan didapatkan password berupa 5implePas5word.
```
<img width="1339" alt="Screenshot 2023-09-22 at 00 01 55" src="https://github.com/YudisthiraPutra/Jarkom-Modul-1-B19-2023/assets/114007340/03f5d9fa-2c0a-4458-8dd0-632d50dfc6c0">

```
a. kita mampu melihat paket terakhir pada file pcap adalah 60
b. kita juga mampu melihat pada detail paket bahwa port yang dimiliki oleh service stmp adalah 25
c. kita juga mampu melihat ip address yang merupakan public yaitu 74.53.140.153
```

## 6 (PADA WAKTU REVISI)
### Soal
```
Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif.
sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama.
suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut,
laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan
"server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya
menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk
menemukan solusi kode error tersebut.
```
### Pengerjaan
<img width="1340" alt="Screenshot 2023-09-21 at 23 58 31" src="https://github.com/YudisthiraPutra/Jarkom-Modul-1-B19-2023/assets/114007340/224052b1-1459-493c-bc19-baf77ba06fa9">

```
Pada nomor 6, kita perlu melihat paket nomor 7812, kemudian melakukan decode sesuai
dengan clue yang ada yaitu a1 e55 u21, decode ini berupa merubah angka menajdi huruf. 
IP yang dimiliki paket 7812 adalah 104.18.14.101, jika dipecah akan menjadi
10 4 18 14 10 1, jika di decode akan menjadi JDRNJA
```

## 7
### Soal
```
Berapa jumlah packet yang menuju IP 184.87.193.88?
```
### Pengerjaan
<img width="1339" alt="Screenshot 2023-09-21 at 23 57 31" src="https://github.com/YudisthiraPutra/Jarkom-Modul-1-B19-2023/assets/114007340/646042d2-83b5-4217-b270-393291c5fdc6">

```
Dengan melakukan query "ip.dst == 184.87.193.88", kita mampu
mendapatkan jumlah paket sesuai di foto, yaitu 6.
```

## 8
```
### Soal
Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80!
(Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)
```
### Pengerjaan
<img width="1341" alt="Screenshot 2023-09-21 at 23 55 58" src="https://github.com/YudisthiraPutra/Jarkom-Modul-1-B19-2023/assets/114007340/7e7f69ac-cbc1-466e-8ff6-68622cd5e89d">

```
Dengan melakukan pencaharian query sebagai berikut "tcp.dstport == 80 || udp.dstport == 80"
kita mampu memilah semua paket yang menuju port 80
```

## 9
### Soal
```
Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal
dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!
```
### Pengerjaan
<img width="1344" alt="Screenshot 2023-09-21 at 23 52 23" src="https://github.com/YudisthiraPutra/Jarkom-Modul-1-B19-2023/assets/114007340/1088d864-10de-490b-a170-347decd4cc8b">

```
Dengan melakukan pencaharian query dengan tulisan sebagai berikut, "ip.src == 10.51.40.1 && ip.dst != 10.39.55.34",
kita mampu memilah paket yang berasal dari alamat 10.51.40.1 serta tidak menuju ke 10.39.55.34
```

## 10
### Soal
```
Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet
```
### Pengerjaan

<img width="1341" alt="Screenshot 2023-09-21 at 23 50 31" src="https://github.com/YudisthiraPutra/Jarkom-Modul-1-B19-2023/assets/114007340/ff3f8c1c-1722-4c68-af4d-9c9c51d807dc">

```
Dengan melakukan filtering dengan text "telnet" kita mampu mendapatkan semua paket telnet.
Kemudian ketika kita melakukan follow ke salah satu paket, maka data pada gambar diatas akan muncul,
data tersebut merupakan username serta password yang kita cari.
```


