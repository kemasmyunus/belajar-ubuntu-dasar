# Belajar Ubuntu dan Terminal

## 1. Pengenalan Ubuntu
Ubuntu adalah salah satu distribusi Linux berbasis Debian yang populer digunakan karena kemudahan dan stabilitasnya. Ubuntu memiliki beberapa edisi, seperti:
- **Ubuntu Desktop**: Untuk pengguna umum dengan antarmuka grafis.
- **Ubuntu Server**: Untuk kebutuhan server tanpa GUI.
- **Ubuntu Core**: Untuk IoT dan sistem tertanam.

## 2. Menggunakan Terminal
Terminal adalah alat baris perintah yang digunakan untuk berinteraksi dengan sistem operasi Ubuntu. Beberapa cara untuk membuka terminal:
- Menekan `Ctrl + Alt + T`
- Mencari "Terminal" di menu aplikasi
- Menggunakan `tty` dengan `Ctrl + Alt + F1` sampai `F6`

## 3. Perintah Dasar Terminal

### 3.1 Navigasi Direktori
- `pwd` → Menampilkan direktori saat ini
- `ls` → Menampilkan isi direktori
- `cd <direktori>` → Berpindah ke direktori tertentu
- `cd ..` → Kembali ke direktori sebelumnya
- `mkdir <nama_direktori>` → Membuat direktori baru
- `rmdir <nama_direktori>` → Menghapus direktori kosong

### 3.2 Mengelola File
- `touch <nama_file>` → Membuat file kosong
- `cp <sumber> <tujuan>` → Menyalin file atau direktori
- `mv <sumber> <tujuan>` → Memindahkan atau mengganti nama file
- `rm <nama_file>` → Menghapus file
- `cat <nama_file>` → Menampilkan isi file
- `nano <nama_file>` → Mengedit file dengan editor nano

### 3.3 Hak Akses File
- `chmod <mode> <file>` → Mengubah hak akses file
- `chown <user>:<group> <file>` → Mengubah kepemilikan file
- `ls -l` → Melihat izin file

### 3.4 Manajemen Paket
Ubuntu menggunakan **APT (Advanced Package Tool)** untuk mengelola paket.
- `sudo apt update` → Memperbarui daftar paket
- `sudo apt upgrade` → Memperbarui semua paket
- `sudo apt install <nama_paket>` → Menginstal paket
- `sudo apt remove <nama_paket>` → Menghapus paket
- `dpkg -i <nama_file.deb>` → Menginstal paket .deb secara manual

### 3.5 Manajemen Proses
- `ps aux` → Menampilkan daftar proses
- `top` atau `htop` → Memantau proses yang berjalan
- `kill <PID>` → Menghentikan proses berdasarkan ID
- `pkill <nama_proses>` → Menghentikan proses berdasarkan nama

### 3.6 Jaringan dan Koneksi
- `ip a` → Melihat alamat IP
- `ping <alamat>` → Mengecek koneksi ke alamat tertentu
- `curl <url>` → Mengambil data dari URL
- `wget <url>` → Mengunduh file dari internet

### 3.7 Manajemen Pengguna
- `whoami` → Menampilkan pengguna saat ini
- `adduser <nama_user>` → Menambahkan pengguna baru
- `deluser <nama_user>` → Menghapus pengguna
- `passwd <nama_user>` → Mengubah password

## 4. Shell Scripting Dasar
Shell script memungkinkan eksekusi beberapa perintah secara otomatis.
Buat file script:
```bash
nano script.sh
```
Isi dengan contoh berikut:
```bash
#!/bin/bash
echo "Hello, Ubuntu!"
```
Simpan, lalu jalankan dengan:
```bash
chmod +x script.sh
./script.sh
```
