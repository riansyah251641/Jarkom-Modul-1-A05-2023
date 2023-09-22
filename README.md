# Jarkom-Modul-1-A05-2023

# Kelompok A19:
| Nama | NRP |
| ---------------------- | ---------- |
| Muhammad Ferbiansyah | 5025211164 |
| Layyinatul Fuadah | 5025211207 |

## No 1
1.	User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file
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
Answer = gunucorn

![alt text](https://github.com/ayyfuadh/Jarkom-Modul-1-A05-2023/blob/main/img/soal%20no%202.png?raw=true)

Pada soal no 2 kita di suruh umtuk mencari web server yang digunakan portal praktikum jaringan komputer. Lakukan filter http yang bertujuan untuk mendapatkan web server.
Selanjutnya Memilih nilai ip 10.21.78.111. kemudian kita buka bagian hypertext dan terdapat detail server bernamakan gunicorn.

## NO 3

## No 4

## No 5
Elshe menemukan suatu file packet capture yang menarik. Bantulah elshe untuk menganalisis file packet capture tersebut. (Revisi)
a. berapa packet yang berhasil dicapture dari file? 60**
Dengan melakukan filter “pass” kita mendapatkan sebuah packet. Kemudian packet tersebut di follow dan pada bagian bawah terdapat pesan di atas. kemudian kita decrypt dan didapatkan password berupa 5implePas5word
Kita dapat melihat nomor paket terakhir yaitu 60
b. port berapa server yang digunakan untuk service smtp?
c. berapa public ip? ketika ditrace/difollow, ip 74.53.140.153 smtp dan mengirim pesan/mail**
kita bisa melihat source port nya adalah 25 dan source address bernilai 74.53.140.153

## No 6
Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal 
yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil 
pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut. (Revisi)

Dengan melakukan decrypt dengan metode “a1 e5 u21” maka diketahui bahwa source address 104.18.14.101 dapat dipecah menajdi 10 4 18 14 10 1, maka hasil decrypt adalah JDRNJA

## No 7
Berapa jumlah packet yang menuju IP 184.87.193.88?
Answear = 6

![alt text](https://github.com/ayyfuadh/Jarkom-Modul-1-A05-2023/blob/main/img/jarkom%20soal%207.png?raw=true)

Dengan menggunakan query ip.dst == 184.87.193.88, kita bisa mendapatkan jumlah packet nya  6.

## No 8

## No 9
Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34! (Revisi)

Jawabannya adalah 
ip.src == 10.51.40.1 && ip.dst != 10.39.55.34

## No 10
Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet
pada paket dengan telnet, ketika kita follow didapatkan hasil sebagai berikut, username adalah dhafin dan password nya adalah kesayangannyak0k0
