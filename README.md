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

### 2. Eksekusi Perintah Sakti
Setelah layar biru (atau hitam) PowerShell terbuka, ketikkan mantra di bawah ini, lalu tekan Enter:

```bash
wsl --install
