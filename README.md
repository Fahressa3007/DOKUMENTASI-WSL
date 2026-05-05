# WSL (WINDOWS SUBSYSTEM FOR LINUX)
ibaratnya memasang linux dengan sistem operasi windows dengan terminal. Tidak lagi perlu repot repot dual-boot atau dengan membuat virtual mechine yang berat dan memakan ram.
### Beberapa keunggulan WSL
**1. Environment Web Development yang Lebih Realistis**

Hampir semua server hosting di internet menggunakan Linux. Ketika sedang membangun website (misalnya menggunakan kombinasi PHP dan MySQL) atau sedang menyiapkan project hub untuk portofolio, menjalankannya di atas WSL membuat environment di komputermu sama persis dengan server asli. Ini sangat meminimalisir error ketika website nantinya di- online -kan.

**2. Surga untuk Opreker Android**

Bagi yang suka modding smartphone, kegiatan seperti nge-build atau extract Custom ROM, memodifikasi kernel, hingga urusan root (seperti menambahkan dukungan KSU atau susfs) jauh lebih optimal, cepat, dan kompatibel jika dieksekusi di lingkungan Linux. Dengan WSL, kamu bisa menjalankan script Linux yang berat sambil tetap nyaman browsing mencari referensi di Windows.

**3. Senjata Ampuh untuk Networking**

Di dunia jaringan komputer, Linux adalah gudangnya tools Command Line (CLI) yang sangat powerful (seperti nmap, tcpdump, netcat, dll). Kalau sedang belajar konsep routing, menguji topologi jaringan, atau mengecek koneksi, menggunakan tools bawaan Linux via WSL jauh lebih leluasa dan detail hasilnya dibandingkan via Command Prompt biasa.

**4. Integrasi Lintas OS yang Mulus**

WSL ini menyatu dengan file system Windows. Artinya, bisa mengedit kode menggunakan aplikasi Windows (seperti Visual Studio Code), lalu mengeksekusi kode tersebut menggunakan terminal Linux yang ada di sebelahnya. Semuanya berjalan harmonis di satu layar.



## 🛠️ Langkah-Langkah Instalasi WSL

Sekarang masuk ke bagian serunya. Cara pasang Linux di Windows ini jauh lebih mudah dari zaman dulu, cuma butuh satu perintah sakti!

### 1. Buka Gerbang Utama (PowerShell as Admin)
Pertama, butuh hak akses penuh ke sistem. Buka **Start Menu**, cari **PowerShell**, lalu klik kanan dan wajib pilih **Run as Administrator**. Kalau tidak pakai akses admin, Windows pasti menolak permintaan instalasi kita.

### 2. Eksekusi Perintah
Setelah layar biru (atau hitam) PowerShell terbuka, ketikkan mantra di bawah ini, lalu tekan Enter:

```bash
wsl --install
```

<img width="784" height="88" alt="Cuplikan layar 2026-05-05 220236" src="https://github.com/user-attachments/assets/574c6c66-562a-43d0-bb29-047184de7b6a" />


## 🐧 Mengenal dan Menginstal Distro Linux Pilihan

Linux itu punya banyak "rasa" atau versi yang disebut **Distro (Distribusi)**.
ada 3 distro yang sangat populer.
**UBUNTU**
yang paling populer dan ramah pemula
**DEBIAN**
yang super stabil dan irit *resource*
**KALI LINUX**
yang sering di bilang gudangnya *tools* untuk *cyber security* dan *networking*.

### 1. Melihat "Menu" Daftar Distro (Cek Online)
Sebelum menginstal, harus tahu dulu OS apa saja yang didukung secara resmi. Buka **PowerShell**, lalu ketik perintah ini:

```bash
wsl --list --online
```

<img width="929" height="472" alt="Cuplikan layar 2026-05-06 003411" src="https://github.com/user-attachments/assets/d070926b-a58b-4e55-97e0-71e2fdbad482" />

lalu setelah itu akan banyak muncul banyak sekali distro. Perhatikan baik-baik teks yang ada di kolom NAME, karena nama itulah yang akan gunakan untuk memanggil perintah instalasi.

### 2. Mengeksekusi Instalasi Distro Spesifik
Misalnya, dari daftar tersebut, tertarik ingin mencoba Debian. Maka, gunakan perintah instalasi standar yang ditambahkan parameter -d (singkatan dari Distribution), lalu diikuti nama distronya.

```bash
wsl --install -d Debian
```
