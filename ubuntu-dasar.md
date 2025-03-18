# Belajar Ubuntu dan Terminal

## 📌 1. Pengenalan Ubuntu
Ubuntu adalah salah satu distribusi Linux berbasis Debian yang populer digunakan karena kemudahan dan stabilitasnya. Ubuntu memiliki beberapa edisi, seperti:

- **🖥️ Ubuntu Desktop** → Untuk pengguna umum dengan antarmuka grafis.
- **🖧 Ubuntu Server** → Untuk kebutuhan server tanpa GUI.
- **🌍 Ubuntu Core** → Untuk IoT dan sistem tertanam.

### ✅ 1.1 Kelebihan Ubuntu
- 🆓 **Gratis dan open-source**
- 🔒 **Stabil dan aman**
- 🖥️ **Kompatibel dengan berbagai perangkat keras**
- 👥 **Dukungan komunitas yang luas**
- 📦 **Banyak perangkat lunak tersedia melalui repositori resmi**

### 📥 1.2 Instalasi Ubuntu
Untuk menginstal Ubuntu, Anda dapat mengunduh ISO dari situs resmi Ubuntu dan membuat bootable USB menggunakan alat seperti Rufus atau balenaEtcher. Setelah itu, boot dari USB dan ikuti petunjuk instalasi.

---

## 🎯 2. Menggunakan Terminal
Terminal adalah alat baris perintah yang digunakan untuk berinteraksi dengan sistem operasi Ubuntu. Beberapa cara untuk membuka terminal:

- 🔘 `Ctrl + Alt + T`
- 🔍 Mencari "Terminal" di menu aplikasi
- 🔄 Menggunakan `tty` dengan `Ctrl + Alt + F1` sampai `F6`



## 🔹 3. Perintah Dasar Terminal

### 📂 3.1 Navigasi Direktori
- `pwd` → Menampilkan direktori saat ini
- `ls -la` → Menampilkan isi direktori secara rinci
- `cd <direktori>` → Berpindah ke direktori tertentu
- `cd ..` → Kembali ke direktori sebelumnya
- `mkdir <nama_direktori>` → Membuat direktori baru
- `rmdir <nama_direktori>` → Menghapus direktori kosong
- `rm -r <nama_direktori>` → Menghapus direktori beserta isinya

### 📄 3.2 Mengelola File
- `touch <nama_file>` → Membuat file kosong
- `cp <sumber> <tujuan>` → Menyalin file atau direktori
- `mv <sumber> <tujuan>` → Memindahkan atau mengganti nama file
- `rm <nama_file>` → Menghapus file
- `cat <nama_file>` → Menampilkan isi file
- `nano <nama_file>` → Mengedit file dengan editor nano
- `less <nama_file>` → Menampilkan isi file dengan navigasi
- `head <nama_file>` → Menampilkan 10 baris pertama file
- `tail <nama_file>` → Menampilkan 10 baris terakhir file

### 🔐 3.3 Hak Akses File
- `chmod <mode> <file>` → Mengubah hak akses file
- `chown <user>:<group> <file>` → Mengubah kepemilikan file
- `ls -l` → Melihat izin file secara rinci
- `umask <nilai>` → Mengatur izin default file yang baru dibuat

### 📦 3.4 Manajemen Paket
Ubuntu menggunakan **APT (Advanced Package Tool)** untuk mengelola paket:

- `sudo apt update` → Memperbarui daftar paket
- `sudo apt upgrade` → Memperbarui semua paket
- `sudo apt install <nama_paket>` → Menginstal paket
- `sudo apt remove <nama_paket>` → Menghapus paket
- `sudo apt autoremove` → Menghapus paket yang tidak dibutuhkan
- `dpkg -i <nama_file.deb>` → Menginstal paket `.deb` secara manual
- `apt search <keyword>` → Mencari paket dalam repositori

### ⚙️ 3.5 Manajemen Proses
- `ps aux` → Menampilkan daftar proses yang berjalan
- `top` atau `htop` → Memantau proses secara real-time
- `kill <PID>` → Menghentikan proses berdasarkan ID
- `pkill <nama_proses>` → Menghentikan proses berdasarkan nama
- `nohup <perintah> &` → Menjalankan proses di latar belakang

### 🌐 3.6 Jaringan dan Koneksi
- `ip a` → Melihat alamat IP dan antarmuka jaringan
- `ping <alamat>` → Mengecek koneksi ke alamat tertentu
- `curl <url>` → Mengambil data dari URL
- `wget <url>` → Mengunduh file dari internet
- `netstat -tulnp` → Menampilkan daftar port yang terbuka

### 👤 3.7 Manajemen Pengguna
- `whoami` → Menampilkan pengguna saat ini
- `id <nama_user>` → Menampilkan informasi pengguna
- `adduser <nama_user>` → Menambahkan pengguna baru
- `deluser <nama_user>` → Menghapus pengguna
- `passwd <nama_user>` → Mengubah password pengguna
- `usermod -aG <grup> <nama_user>` → Menambahkan pengguna ke grup
- `groups <nama_user>` → Melihat daftar grup pengguna



## 📝 4. Shell Scripting Dasar
Shell script memungkinkan eksekusi beberapa perintah secara otomatis.

### 🛠️ 4.1 Membuat Shell Script
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

### 🔢 4.2 Variabel dalam Shell Script
```bash
#!/bin/bash
nama="Ubuntu"
echo "Selamat datang di $nama"
```

### 🔄 4.3 Penggunaan Kondisi (if-else)
```bash
#!/bin/bash
if [ -f "/etc/passwd" ]; then
    echo "File passwd ditemukan."
else
    echo "File tidak ditemukan."
fi
```

### 🔁 4.4 Penggunaan Loop
```bash
#!/bin/bash
for i in {1..5}; do
    echo "Perulangan ke-$i"
done
```



## 📌 5. Kesimpulan
Memahami terminal di Ubuntu sangat penting untuk efisiensi dan fleksibilitas dalam mengelola sistem. Dengan mempelajari perintah dasar, manajemen file, paket, dan pengguna, Anda akan lebih nyaman menggunakan Ubuntu secara profesional. Selain itu, memahami **shell scripting** dapat meningkatkan produktivitas dengan mengotomatisasi berbagai tugas administrasi. 🚀

