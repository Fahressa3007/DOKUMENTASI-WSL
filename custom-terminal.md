# 🎨 Menggunakan ZSH 

## Apa itu Zsh (Z Shell)?
Zsh adalah salah satu jenis Shell di Linux. Zsh dibangun di atas pondasi Bash, yang berarti semua perintah dasar Bash (seperti cd, ls, apt update) 100% bisa berjalan di Zsh. Namun, Zsh menambahkan sangat banyak fitur tingkat lanjut yang tidak dimiliki Bash secara bawaan.

Zsh diciptakan untuk menutupi kelemahan Bash dalam hal interaksi pengguna. Zsh lebih fokus pada efisiensi mengetik dan memberikan bantuan visual kepada administrator sistem atau developer.

Fitur Teknis Utama Zsh:

* Path Expansion (Ekspansi Direktori): Jika kamu ingin masuk ke /usr/local/bin, di Zsh kamu cukup mengetik cd /u/l/b lalu menekan Tab. Zsh akan membaca pola tersebut dan melengkapinya secara otomatis.

* Case-Insensitive Completion: Di Bash, jika folder bernama Documents dan kamu mengetik cd doc lalu menekan Tab, Bash tidak akan merespons karena huruf 'd' kecil tidak sama dengan 'D' besar. Di Zsh, ia akan mengabaikan perbedaan huruf besar/kecil dan tetap melengkapinya menjadi Documents.

* Advanced Globbing: Zsh memiliki sistem pencarian file (menggunakan tanda bintang *) yang jauh lebih kuat. Misalnya, kamu bisa dengan mudah mencari "semua file berekstensi .txt yang ukurannya di atas 10MB" hanya dengan satu baris perintah pendek.

* Shared History: Jika kamu membuka tiga jendela terminal secara bersamaan, perintah yang kamu ketik di jendela pertama akan langsung tersimpan dan bisa dipanggil (dengan tombol panah atas) di jendela kedua dan ketiga secara real-time.
