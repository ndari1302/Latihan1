# Latihan1
# Tutorial Penggunaan Git

**Apa itu Git?**

Git adalah salah satu sistem pengontrol versi (Version Control System) pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds. Pengontrol versi bertugas mencatat setiap perubahan pada file proyek yang dikerjakan oleh banyak orang maupun sendiri. Git dikenal juga dengan distributed revision control (VCS terdistribusi), artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja

# Menambahkan Global Config
Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user name dan user email konfigurasi ini bisa dilakukan untuk global repository atau individual repository. apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit Lakukan "git config --global user.name dan user.email" supaya bisa login github ketika push.

![config](https://user-images.githubusercontent.com/46927379/51920220-883c1f00-2417-11e9-9cc1-87e5137e54a2.png)

# Perintah Dasar Git
- git init: perintah untuk membuat repository local
- git add: perintah untuk menambahkan file baru, atau perubahan pada file pada staging sebelum proses commit.
- git commit: perintah untuk menyimpan perubahan kedalam database git.
- git push -u origin master: perintah untuk mengirim perubahan pada repository local menuju server repository.
- git clone [url]: perintah untuk membuat working directory yang diambil dari repositry sever.
- git remote add origin [url]: perintah untuk menambahkan remote server/reopsitory server pada local repositry (working directory)

# Membuat Repository Local
- Open gitbash, ketik cd /D
- Buat direktory project praktikum pertama dengan nama Latihan Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd (change directory)
- Direktory aktif menjadi: D/Pemograman, kemudian masuk ke direktory tersebut 
- Ketik "echo" untuk membuat file README.md

![echo](https://user-images.githubusercontent.com/46927379/51921589-495b9880-241a-11e9-8f88-88a33f6feffd.png)

- Lalu Lakukan **git init** untuk menjadikan repository lokal 
- kemudian tambahkan file tersebut ke repository dengan **git add README.md** 
- file yang berhasil ditambahkan akan terlihat seperti di gambar, dengan "ls -l" 
- Untuk Menyimpan perubahan sebuah file ke repository local gunakan perintah **git commit -m** "Nama perintahnya"

![commit](https://user-images.githubusercontent.com/46927379/51922155-106ff380-241b-11e9-8812-27787ef188fd.png)

# Membuat Repository Server
- Server reopsitory yang akan kita gunakan adalah http://github.com
- Anda harus mempunyai akun terlebih dahulu.

![login](https://user-images.githubusercontent.com/46927379/51922372-7e1c1f80-241b-11e9-997c-7f7c43b5fc6a.png)

- Pada laman github, dari menu (icon +) klik New Repository

![new repo](https://user-images.githubusercontent.com/46927379/51922419-95f3a380-241b-11e9-93fc-187899a28df9.png)

- Isi nama repositorynya, misal: latihan1, lalu klik tombol Create repository

![new repo1](https://user-images.githubusercontent.com/46927379/51922538-d05d4080-241b-11e9-8ffe-4ae2958c03f3.png)

# Menambahkan Remote Repository
- Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.
- Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]

![remote](https://user-images.githubusercontent.com/46927379/51923171-fcc58c80-241c-11e9-97ba-b63140be572b.png)

# Push (Mengirim perubahan ke server)
- Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.
- Gunakan printah git push -u origin master

![git push](https://user-images.githubusercontent.com/46927379/51923491-b02e8100-241d-11e9-84f8-8654b255b358.png)

- Perintah ini akan meminta memasukkan username dan password pada akun github.com

![push login](https://user-images.githubusercontent.com/46927379/51923609-e8ce5a80-241d-11e9-9d45-649936f3de89.png)

- Proses push berhasil, maka akan muncul gambar seperti ini

![push done](https://user-images.githubusercontent.com/46927379/51923567-d05e4000-241d-11e9-9173-067fc9009857.png)

# Melihat Hasil nya pada Repository
•	Buka laman github.com, lalu refresh page.
•	Maka perubahan akan terlihat pada laman tersebut.

![after](https://user-images.githubusercontent.com/46927379/51924615-ee2ca480-241f-11e9-9fe6-b3d8000e04e2.png)

