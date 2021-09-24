# Jarkom-Modul-1-T7-2021
### Laporan Resmi Pengerjaan Sesi Lab Jaringan Komputer

#### Nama Anggota Kelompok :
1. Naufal Aprilian 
2. Bryan Yehuda Mannuel (05311940000021)
3. Mulki Kusumah

## Sebutkan Webserver yang digunakan pada "ichimarumaru.tech"!

## Temukan Paket dari web-web yang menggunakan Basic Authentication method!

## Ikuti perintah di basic.ichimarumaru.tech! Username dan Password bisa didapatkan dari file .pcapng!

## Temukan Paket MySQL yang mengandung perintah Query Select!

## Login ke portal.ichimarumaru.tech kemudian ikuti perintahnya! Username dan Password bisa didapat dari Query Insert pada Table Users dari file .pcap!

## Cari Username dan Password ketika melakukan Login ke FTP Server!

## Ada 500 file Zip yang disimpan ke FTP Server dengan nama 0.zip, 1.zip, 2.zip, ..., 499.zip. Simpan dan Buka file pdf tersebut.

## Cari paket yang menunjukan pengambilan File dari FTP tersebut!

## Dari paket-paket yang menuju FTP terdapat indikasi penyimpanan beberapa file. Salah satunya adalah sebuah file berisi data rahasia dengan nama "secret.zip". Simpan dan Buka file tersebut!

## Selain itu terdapat "history.txt" yang kemungkinan berisi history Bash Server tersebut! Gunakan isi dari "history.txt" untuk menemukan Password untuk membuka file rahasia yang ada di "secret.zip"!

## Filter sehingga Wireshark hanya mengambil paket yang berasal dari Port 80!

1. Mengisi Capture Filter dengan : `src port 80`
![src port 80](https://github.com/BryanYehuda/Jarkom-Modul-1-T7-2021/blob/main/images/11-1.png?raw=true)
2. Berikut adalah hasil ketika Wireshark hanya mengambil paket yang berasal dari Port 80
![hasil dari src port 80](https://github.com/BryanYehuda/Jarkom-Modul-1-T7-2021/blob/main/images/11.png?raw=true)

## Filter sehingga Wireshark hanya mengambil paket yang mengandung Port 21!

1. Mengisi Capture Filter dengan : `port 21`
![port 21](https://github.com/BryanYehuda/Jarkom-Modul-1-T7-2021/blob/main/images/12.png?raw=true)
2. Berikut adalah hasil ketika Wireshark hanya mengambil paket yang mengandung Port 21. Karena port 21 adalah port untuk FTP dan kami tidak memiliki server FTP, jadi kelompok kami melakukan testing koneksi ke alamat random dengan Username dan Password random. Alhasil koneksi bisa terlihat pada Wireshark namun ditolak karena Username dan Passwordnya salah.
![hasil dari port 21](https://github.com/BryanYehuda/Jarkom-Modul-1-T7-2021/blob/main/images/12-bukti.png?raw=true)

## Filter sehingga Wireshark hanya menampilkan paket yang menuju Port 443!

1. Mengisi Capture Filter dengan : `dst port 443`
![dst port 443](https://github.com/BryanYehuda/Jarkom-Modul-1-T7-2021/blob/main/images/13.png?raw=true)
2. Berikut adalah hasil ketika Wireshark hanya menampilkan paket yang menuju Port 443
![hasil dari dst port 443](https://github.com/BryanYehuda/Jarkom-Modul-1-T7-2021/blob/main/images/13-bukti.png?raw=true)

## Filter sehingga Wireshark hanya mengambil paket yang tujuannya ke kemenag.go.id!

1. Mengisi Capture Filter dengan : `dst host kemenag.go.id`
![dst host kemenag.go.id](https://github.com/BryanYehuda/Jarkom-Modul-1-T7-2021/blob/main/images/14.png?raw=true)
2. Berikut adalah hasil ketika Wireshark hanya mengambil paket yang tujuannya ke kemenag.go.id, untuk bisa menampilkan hasil ini kelompok kami harus mengunjungi situs Kemenag tersebut terlebih dahulu.
![hasil dari dst host kemenag.go.id](https://github.com/BryanYehuda/Jarkom-Modul-1-T7-2021/blob/main/images/14-hasil.png?raw=true)

## Filter sehingga Wireshark hanya mengambil paket yang berasal dari IP kalian!

1. Mencari IP di komputer kami menggunakan Command Prompt dan memasukkan : `ipconfig`
2. Didapatkan IP-nya adalah `10.27.161.52`
3. Mengisi Capture Filter dengan : `src host 10.27.161.52`
![src host 10.27.161.52](https://github.com/BryanYehuda/Jarkom-Modul-1-T7-2021/blob/main/images/15.png?raw=true)
4. Berikut adalah hasil ketika Wireshark mengambil paket yang berasal dari IP kami.
![hasil dari src host 10.27.161.52](https://github.com/BryanYehuda/Jarkom-Modul-1-T7-2021/blob/main/images/15-bukti.png?raw=true)