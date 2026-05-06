## 💻 Perintah Dasar WSL & Debian yang Wajib Dikuasai

Setelah Debian terinstal, akan sering berinteraksi dengan terminal. Sebagai fondasi yang kuat sebelum masuk ke konfigurasi *web server* atau *networking*, berikut adalah "perintah-perintah" dasar yang akan sangat sering digunakan:

### 1. Manajemen WSL (Dijalankan di PowerShell Windows)

Perintah-perintah ini digunakan untuk mengatur status distro Linux dari luar.

*   **Masuk ke Debian:**
    Jika sedang berada di PowerShell dan ingin langsung masuk ke terminal Debian, cukup ketik:

    ```bash
    wsl distro Debian
    ```
    bisa di singkat dengan :
    
    ```bash
    wsl -d Debian
    ```

    tanda jika masih di powershell pada awal format ps:,
    sedangkan jika sudah masuk wsl nanti akan berubah username@nama-komputer:lokasi$
    
*   **Masuk sebagai *Root* (Administrator):**
    Terkadang kamu butuh akses tertinggi tanpa harus memakai `sudo` terus-menerus.
    ```bash
    sudo su
    ```
*   **Mematikan Debian (Terminate):**
    Jika Debian sedang *error* atau ingin me- *restart* layanannya tanpa me- *restart* Windows:
    ```bash
    wsl -t Debian
    ```

### 2. Perintah Dasar Debian (Dijalankan di dalam Terminal Linux)

Setelah masuk ke dalam *environment* Debian, perintah Windows sudah tidak berlaku. Ini adalah perintah dasar Linux yang wajib dihafal:

*   **Update & Upgrade Sistem (Sangat Penting):**
    Selalu jalankan perintah ini setiap kali baru menginstal Debian atau sebelum menginstal aplikasi baru (seperti PHP atau *database*). Fungsinya untuk memperbarui repositori ke versi terbaru.
    ```bash
    sudo apt update && sudo apt upgrade -y
    ```
*   **Navigasi Direktori:**
    - `pwd` : Mengecek posisi foldermu saat ini (*Print Working Directory*).
    - `ls` : Melihat daftar *file* dan folder di dalam lokasimu sekarang.
    - `cd nama_folder` : Berpindah masuk ke folder tertentu.
    - `cd ..` : Mundur satu folder ke belakang.
*   **Instalasi Aplikasi (Package Manager):**
    Debian menggunakan `apt` sebagai *package manager*. Untuk menginstal *tools* jaringan atau bahasa pemrograman, gunakan:
    ```bash
    sudo apt install nama_aplikasi
    ```
    *(Contoh: `sudo apt install net-tools` untuk memasang alat pengecekan jaringan dasar).*
*   **Pindah ke Direktori Windows:**
    Mau mengakses *file* yang ada di partisi C: Windows milikmu dari dalam Debian? Akses lewat folder `/mnt`.
    ```bash
    cd /mnt/c
    ```

---
**💡 Tips:** Di Linux, huruf besar dan kecil sangat berpengaruh (*case-sensitive*). Perintah `cd Folderku` akan berbeda hasilnya dengan `cd folderku`.
