# Lat1
# Apa itu Git?
* Git adalah salah satu sistem pengontrol versi (Version Control
System) pada proyek perangkat lunak yang diciptakan oleh Linus
Torvalds.
* Pengontrol versi bertugas mencatat setiap perubahan pada file
proyek yang dikerjakan oleh banyak orang maupun sendiri.
* Git dikenal juga dengan distributed revision control (VCS terdistribusi),
artinya penyimpanan database Git tidak hanya berada dalam satu
tempat saja.
# Instalasi Git
* Download **Git**, buka website resminya Git [ git-scm.com ]( http://git-scm.com ).
* Kemudian unduh Git sesuai dengan arsitektur komputer kita. Kalau
menggunakan 64bit, unduh yang 64bit. Begitu juga kalau
menggunakan 32bit.
* Selamat, Git sudah terinstal di Windows. Untuk mencobanya,
silahkan buka **CMD** atau **PowerShell**, kemudian ketik perintah.
"git -- version".

![Gambar 1](https://user-images.githubusercontent.com/57052298/68081099-ee3c5380-fe3a-11e9-86aa-405e7f191cc2.png)


# Menambahkan Global Config
* Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi
user.name dan user.email
* konfigurasi ini bisa dilakukan untuk global repostiry atau individual
repository.
* apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi
kegagalan saat menjalankan perintah git commit
* Config Global Repository

![Gambar 2](https://user-images.githubusercontent.com/57052298/68081114-3a879380-fe3b-11e9-9776-7d3a047c5543.png)

# Perintah Dasar Git
* git init, perintah untuk membuat repository local
* git add, perintah untuk menambahkan file baru, atau perubahan pada file
pada staging sebelum proses commit.
* git commit, perintah untuk menyimpan perubahan kedalam database git.
* git push -u origin master, perintah untuk mengirim perubahan pada
* repository local menuju server repository.
* git clone [url], perintah untuk membuat working directory yang diambil dari
repositry sever.
* git remote add origin [url], perintah untuk menambahkan remote
server/reopsitory server pada local repositry (working directory)
* git pull, perintah untuk mengambil/mendownload perubahan terbaru dari
server repository ke local repository

# Membuat Reposiory Local
* Buka direktory aktif, misal: d:\labs_pemrograman1 (buka
menggunakan Windows Explorer)
* klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash,
sehingga muncul git bash commad
* Buat direktory project praktikum pertama dengan nama latihan1
* Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya
masuk kedalam direktori tersebut dengan perintah cd (change
directory)
* direktory aktif menjadi: d:\labs_pemrograman1\latihan1

![Gambar 3](https://user-images.githubusercontent.com/57052298/68081160-ee891e80-fe3b-11e9-9ed6-44a483f2f3ac.png)

# Membuat Reposiory Local
* Jalankan perintah git init, untuk membuat repository local.
* Repository baru berhasil di inisialisasi, dengan terbentuknya satu
direktori hidden dengan nama .git
* Pada direktori tersebut, semua perubahan pada working directory
akan disimpan.

![Gambar 4](https://user-images.githubusercontent.com/57052298/68081171-36a84100-fe3c-11e9-95b9-dc427afbd807.png)

# Menambahkan File baru pada repository
* Untuk membuat file dapat menggunakan text editor, lalu menyimpan
filenya pada direktori aktif (repository)
* disini kita akan coba buat satu file bernama README.md (text file)
* File README.md berhasil dibuat.

![Gambar 5](https://user-images.githubusercontent.com/57052298/68081178-648d8580-fe3c-11e9-86d1-fd73c046112e.png)

# Menambahkan File baru pada repository
* Untuk menambahkan file yang baru saja dibuat tersebut gunakan
perintah git add.
* File README.md berhasil ditambahkan.

![Gambar 6](https://user-images.githubusercontent.com/57052298/68081196-a9b1b780-fe3c-11e9-9a4d-6d96db1397ff.png)

# Commit (Menyimpan perubahan ke database)
* Untuk menyimpan perubahan yang ada kedalam database repository
local, gunakan perintah git commit -m “komentar commit”
* Perubahan berhasil disimpan.

![Gambar 7](https://user-images.githubusercontent.com/57052298/68081208-dcf44680-fe3c-11e9-985d-6af354b6635d.png)
”

# Membuat repository server
* Server reopsitory yang akan kita gunakan adalah http://github.com
* Anda harus membuat akun terlebih dahulu.
* Pada laman github, klik tombol start a project, atau
* Dari menu (icon +) klik New Repository

# Membuat repository server
* Isi nama repositorynya, misal: labpy1.
* lalu klik tombol Create repository

![Gambar 8](https://user-images.githubusercontent.com/57052298/68081236-6c99f500-fe3d-11e9-8550-d1499a50105c.png)

# Menambahkan Remote Repository
* Remote Repository merupakan repository server yang akan
digunakan untuk menyimpan setiap perubahan pada local repository,
sehingga dapat diakses oleh banyak user.
* Untuk menambahkan remote repository server, gunakan perintah
git remote add origin [url]
$ git remote add origin https://github.com/abuazzam/labpy1.git

# Push (Mengirim perubahan ke server)
* Untuk mengirim perubahan pada local repository ke server gunakan
perintah git push.
* Perintah ini akan meminta memasukkan username dan password
pada akun github.com

![Tanpa jud l](https://user-images.githubusercontent.com/57052298/68081274-df0ad500-fe3d-11e9-8f62-6b0df2263e30.png)

# Melihat hasilnya pada server repository
* Buka laman github.com,
arahkan pada repositorinya.
* Maka perubahan akan
terlihat pada laman
tersebut.

![Tanpa judul](https://user-images.githubusercontent.com/57052298/68081276-03ff4800-fe3e-11e9-8293-872d7d439a6f.png)

# Clone Repository
* Clone repository, pada dasarnya adalah meng-copy repository server
dan secara otomatis membuat satu direktory sesuai dengan nama
repositorynya (working directory).
* Untuk melakukan cloning, gunakan perintah git clone [url]
