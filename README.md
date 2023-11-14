# Cara-Install-Apache2-dan-Nginx
Membahas mengenai penginstallan apache2 dan nginx pada Ubuntu Server.

# Cara Install Apache2
## 1. Login user Ubuntu Server

## 2. Update dan Upgrade
    sudo apt update && sudo apt upgrade
    
## 3. Install Apache2
    sudo apt install apache2

## 4. Menampilkan Daftar Aplikasi yang telah di install
    sudo ufw app list

## 5. Melihat Status Layanan Web Server Apache2
    sudo systemctl status apache2
![image](https://github.com/intnprmtahti/Cara-Install-Apache2-dan-Nginx/assets/150001747/014e8f8c-ed9e-4d06-885c-6379f5f00345)

## 6. Menampilkan Informasi Terkait Interface pada Server 
    ip a
![image](https://github.com/intnprmtahti/Cara-Install-Apache2-dan-Nginx/assets/150001747/bb249d70-4b2a-42ac-8757-3f232875f800)

## 7. Copy IP Address pada Browser
jIka berhasil, akan ada tampilan seperti di bawah ini.
![image](https://github.com/intnprmtahti/Cara-Install-Apache2-dan-Nginx/assets/150001747/51e9a54f-d01d-46ea-a82b-9c25ce10d35e)

## 8. Pembuatan Website <br>
### 8.1 Pembuatan Website Melalui Direktori /var/www/html
    cd /var/www/html

### 8.2 Buat Direktori Baru
    mkdir <nama direktori>
contoh : mkdir intan

### 8.3 Pindah ke Root
    sudo su

### 8.4 Pindah ke Direktori yang Telah Dibuat
    cd <nama direktori>
contoh : 

root@user : /var/www/html# cd intan

### 8.5 Edit Direktori HTML dengan Teks Editor "nano"
    nano index.html
```sh
<html>
<head>

<title> website Intan </title>
</head>
<h1>
<body> Selamat datang di Website Ini </h1>
<p> Nama : Intan Permatahati
<p> NIM : 09011282227036
<p> Kelas : SK5C
<p> Prodi : Sistem Komputer !

<p> Info lebih lanjut :
<a href = "https://www.instagram.com/intnprmtahti" style="color:red">Instagram Intan Permatahati </a>
<a href = "https://wa.me/089678642004" style="color:blue">Whatsapp Intan Permatahati </a>
</body>
</html>
```
contoh program :
![image](https://github.com/intnprmtahti/Cara-Install-Apache2-dan-Nginx/assets/150001747/a52ab4cb-4769-4c37-ba24-c93e9c52aa8c)

## 9. Output
Berikut tampilan website dari proses yang telah dilakukan. 
*192.168.1.10* merupakan IP Address, */intan/* merupakan direktori yang menyimpan isi dari tampilan ini.
![image](https://github.com/intnprmtahti/Cara-Install-Apache2-dan-Nginx/assets/150001747/e111a257-910e-454a-af77-79cf51ef288d)








# Cara Install Nginx

## 1. Login ke Ubuntu Server
## 2. Update dan Upgrade Package
    sudo apt update

## 3. Install Nginx
    sudo apt install nginx
## 4. Menampilkan Daftar Aplikasi yang telah di install
    sudo ufw app list
## 5. Mengizinkan Lalu Lintas ke Web Server Nginx
    sudo ufw allow 'Nginx full'

## 6. Melihat Versi Nginx yang Terinstall
    nginx -v

## 7. Melihat Status dari UFW yang Berjalan
    sudo ufw status

## 8. Melihat Status Layanan Web Server Nginx
    sudo systemctl satus nginx

## 9. Menampilkan Informasi Terkait Interface pada Server
    ip a
contoh :
![image](https://github.com/intnprmtahti/Cara-Install-Apache2-dan-Nginx/assets/150001747/0215313c-73ed-405b-9114-71adb82b7c5e)

## 10. Output
Masukan IP Address Tersebut pada Website. Jika berhasil diakses, akan ada tampilan seperti di bawah ini.

![image](https://github.com/intnprmtahti/Cara-Install-Apache2-dan-Nginx/assets/150001747/b84b1637-c443-47b2-8218-ecc32624e857)
