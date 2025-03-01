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
