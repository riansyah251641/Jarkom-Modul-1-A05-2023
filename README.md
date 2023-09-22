# Jarkom-Modul-1-A05-2023

# Kelompok A05:
| Nama | NRP |
| ---------------------- | ---------- |
| Muhammad Ferbiansyah | 5025211164 |
| Layyinatul Fuadah | 5025211207 |

## No 1
User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file

a.	Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut? 

Answer: 258040667

b.	Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut?

Answer: 1044861039

![alt text](https://github.com/ayyfuadh/Jarkom-Modul-1-A05-2023/blob/main/img/jarkom%20soal%201%20juga.png?raw=true)

Melakukan filtering dengan menuliskan perintah FTP, bertujuan agar memfilter protokol FTP saja sesuai soal yang diminta. 
pada packet 147 kita dapat melihat sequence(raw) = 258040667 dan acknowledge(raw)  = 1044861039 aktivitas dengan melihat membuka FTP 

c.	Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?

Answer: 1044861039

d.	Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?

Answer: 258040696

![alt text](https://github.com/ayyfuadh/Jarkom-Modul-1-A05-2023/blob/main/img/jaekom%20soal%201.png?raw=true)

pada packet 149 kita dapat melihat sequence(raw) = 1044861039 dan acknowledge(raw) = 258040696 yang menunjukan response dengan membuka FTP.

## No 2
Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!

Answer = gunicorn

![alt text](https://github.com/ayyfuadh/Jarkom-Modul-1-A05-2023/blob/main/img/soal%20no%202.png?raw=true)

Pada soal no 2 kita di suruh umtuk mencari web server yang digunakan portal praktikum jaringan komputer. Lakukan filter http yang bertujuan untuk mendapatkan web server.
Selanjutnya Memilih nilai ip 10.21.78.111. kemudian kita buka bagian hypertext dan terdapat detail server bernamakan gunicorn.

## NO 3
a.Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?

Answer: 21

b. Protokol layer transport apa yang digunakan?

Answer: UDP

Bukti
![alt text](https://github.com/riansyah251641/Jarkom-Modul-1-A05-2023/blob/main/img/nomor3.png)

pada nomor 3 dilakukan poencarian dengan menggunakan host untuk mengetahui ip yang menggunakan source maupun deestnya adalah ip yang dicari kemudian digunakan pencaharian port dengan udp karena tidak adanya port yang bertipe tcp


## No 4
Berapa nilai checksum yang didapat dari header pada paket nomor 130?

Answer: 0x18e5

Bukti
![alt text](https://github.com/riansyah251641/Jarkom-Modul-1-A05-2023/blob/main/img/nomor4.png)

dilakukan pemcarian data pada nomor 130 kemudian ditemupan checksum pada bagian User Datagram Protokol

## No 5
Elshe menemukan suatu file packet capture yang menarik. Bantulah elshe untuk menganalisis file packet capture tersebut. (Revisi)

![alt text](https://github.com/riansyah251641/Jarkom-Modul-1-A05-2023/blob/main/img/nomor5_1.png)
![alt text](https://github.com/riansyah251641/Jarkom-Modul-1-A05-2023/blob/main/img/nomor5_2.png)
dilakukan filter dengan kata kunci pass lalu ditemukan suatu password dengan isi cHVuamFiQDEyMw== kemudian di decrypt dan didapatkan password berupa 5implePas5word. lalu dibukak files yang dikunci dan diperoleh nc 10.21.78.111 11111.


a. berapa packet yang berhasil dicapture dari file?
![alt text](https://github.com/riansyah251641/Jarkom-Modul-1-A05-2023/blob/main/img/nomor5_3.png)
jumlah files pada file no 5 diperoleh banyak paket sebesar 60

![alt text](https://github.com/riansyah251641/Jarkom-Modul-1-A05-2023/blob/main/img/nomor5_4.png)
b. port berapa server yang digunakan untuk service smtp?

dilakukan filter dengan smtp lalu ditemukan port yang digunakan yaitu 25

c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?

alamat IP dalam rentang 10.x.x.x, 172.16.x.x - 172.31.x.x, atau 192.168.x.x, maka itu adalah alamat IP pribadi, bukan alamat IP publik.

## No 6
Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal 
yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil 
pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut. (Revisi)

Answer = 
![alt text](https://github.com/riansyah251641/Jarkom-Modul-1-A05-2023/blob/main/img/nomor6.png)
pada soal didapat kode "a1 e5 u21" kemudian dilakukan decrypt dan diperoleh ip source nya yaitu 104.18.14.101 kemudian dipecah kembali agar dapat di decrypt menjadi 10 4 18 14 10 1. sehingga menghasilkan nilai JDNJA


## No 7
Berapa jumlah packet yang menuju IP 184.87.193.88?

Answer = 6

![alt text](https://github.com/ayyfuadh/Jarkom-Modul-1-A05-2023/blob/main/img/jarkom%20soal%207.png?raw=true)

Dengan menggunakan query ip.dst == 184.87.193.88, kita bisa mendapatkan jumlah packet nya  6.

## No 8
Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)


Answer =  tcp.dstport == 80 || udp.dstport == 80

Bukti
![alt text](https://github.com/riansyah251641/Jarkom-Modul-1-A05-2023/blob/main/img/nomor8.png)

dengan menggunakan perintah tcp.dstport == 80 || udp.dstport == 80 yang berarti untuk semua port yang bertipe tcp ataupun udp yang bernilai 80.

## No 9
Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34! (Revisi)

Answer = ip.src == 10.51.40.1 && ip.dst != 10.39.55.34

Bukti
![alt text](https://github.com/riansyah251641/Jarkom-Modul-1-A05-2023/blob/main/img/nomor9_1.png)
![alt text](https://github.com/riansyah251641/Jarkom-Modul-1-A05-2023/blob/main/img/nomor9_2.png)

dengan menggunakan perintah ip.src == 10.51.40.1 && ip.dst != 10.39.55.34, maka akan ditemukan packet dengan ip source 10.51.40.1 dengan ip destinationnya tidak pada 10.39.55.34

## No 10
Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet (revisi)

Answer = pada paket dengan telnet, ketika kita follow didapatkan hasil sebagai berikut, username adalah dhafin dan password nya adalah kesayangannyak0k0

Bukti
![alt text](https://github.com/riansyah251641/Jarkom-Modul-1-A05-2023/blob/main/img/nomor10.png)

dilakukan pencaharian satu persatu sesuai dengan format yang diberikan yaitu username|password dan ditemukan pada data nomor 81 dengan jawaban dhafin:kesayangannyak0k0

