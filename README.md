# belajar-github

Berikut ini adalah perintah-perintah Git yang diminta, termasuk dalam tabel:

| Perintah Git                                              | Contoh                                                   | Penjelasan                                                                                          |
| --------------------------------------------------------- | -------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `git config --global user.name "Fiki Aprian"`             | -                                                        | Mengatur nama pengguna Git secara global.                                                           |
| `git config --global user.email "fikiaprian23@gmail.com"` | -                                                        | Mengatur alamat email pengguna Git secara global.                                                   |
| `git init`                                                | -                                                        | Membuat repositori Git baru di direktori saat ini.                                                  |
| `git remote add origin <URL repositori>`                  | `git remote add origin https://github.com/user/repo.git` | Menghubungkan repositori lokal dengan repositori jarak jauh (remote repository).                    |
| `git status`                                              | -                                                        | Menampilkan status perubahan dalam repositori.                                                      |
| `git add <nama_file>`                                     | `git add file.txt`                                       | Menambahkan perubahan pada file ke dalam daftar perubahan Git.                                      |
| `git commit`                                              | -                                                        | Membuat snapshot perubahan yang sudah ditambahkan dengan pesan komit.                               |
| `git log`                                                 | -                                                        | Menampilkan riwayat komit dalam format yang lengkap.                                                |
| `git log --all --decorate --oneline --graph`              | -                                                        | Menampilkan riwayat komit dalam format yang ringkas dan grafis.                                     |
| `git branch`                                              | -                                                        | Menampilkan daftar cabang dalam repositori.                                                         |
| `git branch <nama_branch>`                                | `git branch new-feature`                                 | Membuat cabang baru dalam repositori.                                                               |
| `git checkout <nama_branch>`                              | `git checkout new-feature`                               | Beralih ke cabang atau komit tertentu dalam repositori.                                             |
| `git merge`                                               | -                                                        | Menggabungkan perubahan dari cabang tertentu ke cabang saat ini.                                    |
| `git branch --merged`                                     | -                                                        | Menampilkan daftar cabang yang sudah digabungkan ke cabang saat ini.                                |
| `git branch -d <nama_branch>`                             | `git branch -d dosen`                                    | Menghapus cabang yang sudah selesai.                                                                |
| `git pull`                                                | -                                                        | Mengambil perubahan terbaru dari repositori jarak jauh dan menggabungkannya dengan perubahan lokal. |
| `git push origin master`                                  | -                                                        | Mengirimkan perubahan lokal ke repositori jarak jauh pada cabang master.                            |

Pastikan untuk mengganti `<URL repositori>` dengan URL repositori jarak jauh yang ingin Anda hubungkan.

Berikut ini adalah tabel perintah-perintah Git lengkap beserta contoh penggunaan, penjelasan, dan opsi-opsional yang umum digunakan:

| Perintah Git   | Contoh                                                   | Penjelasan                                                                                          | Opsi                                                                                                                                                                                                                                                                             |
| -------------- | -------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `git init`     | `git init my-repo`                                       | Membuat repositori Git baru di direktori saat ini atau dengan nama tertentu.                        | `--bare`: Membuat repositori kosong tanpa direktori kerja.                                                                                                                                                                                                                       |
| `git clone`    | `git clone https://github.com/user/repo.git`             | Mengkloning repositori Git yang ada ke dalam direktori lokal.                                       | `--branch <nama-cabang>`: Mengkloning cabang tertentu dari repositori. <br> `--depth <jumlah-komit>`: Mengkloning sejarah dengan jumlah komit terbatas. <br> `--recurse-submodules`: Mengkloning dan menginisialisasi submodul-submodul.                                         |
| `git add`      | `git add file.txt`                                       | Menambahkan perubahan pada file ke dalam daftar perubahan Git.                                      | `--all` atau `-A`: Menambahkan semua perubahan pada semua file. <br> `--patch` atau `-p`: Memilih perubahan secara interaktif untuk ditambahkan.                                                                                                                                 |
| `git commit`   | `git commit -m "Menambahkan fitur baru"`                 | Membuat snapshot perubahan yang sudah ditambahkan dengan pesan komit.                               | `-a`: Menambahkan dan mengcommit semua perubahan pada file yang sudah ada. <br> `--amend`: Mengubah komit terakhir dengan perubahan baru. <br> `--signoff`: Menambahkan tanda tangan digital ke komit.                                                                           |
| `git push`     | `git push origin main`                                   | Mengirimkan perubahan lokal ke repositori jarak jauh (remote repository).                           | `--force` atau `-f`: Memaksa push perubahan dan mengganti riwayat di repositori pusat. <br> `--tags`: Mengirimkan tag ke repositori pusat. <br> `--set-upstream`: Menetapkan cabang lokal sebagai upstream dari cabang jarak jauh.                                               |
| `git pull`     | `git pull origin main`                                   | Mengambil perubahan terbaru dari repositori jarak jauh dan menggabungkannya dengan perubahan lokal. | `--rebase`: Menggabungkan perubahan dengan menggunakan rebase daripada merge. <br> `--autostash`: Menyembunyikan perubahan sementara sebelum pull dan menerapkannya setelahnya.                                                                                                  |
| `git branch`   | `git branch new-feature`                                 | Membuat cabang baru dalam repositori untuk pengembangan paralel.                                    | `-d <nama-cabang>`: Menghapus cabang yang sudah selesai. <br> `-m <nama-cabang-lama> <nama-cabang-baru>`: Mengubah nama cabang. <br> `-r` atau `--remote`: Menampilkan cabang-cabang jarak jauh.                                                                                 |
| `git checkout` | `git checkout new-feature`                               | Beralih ke cabang atau komit tertentu dalam repositori.                                             | `-b <nama-cabang>`: Membuat dan beralih ke cabang baru sekaligus. <br> `-t <nama-cabang-jarak-jauh>`: Melacak cabang jarak jauh dan beralih ke cabang lokal yang sesuai.                                                                                                         |
| `git merge`    | `git merge new-feature`                                  | Menggabungkan perubahan dari cabang tertentu ke cabang saat ini.                                    | `--no-ff`: Membuat commit merge terpisah daripada fast-forward. <br> `--squash`: Menggabungkan perubahan menjadi satu komit tunggal. <br> `--strategy <nama-strategi>`: Menggunakan strategi penggabungan khusus.                                                                |
| `git status`   | `git status`                                             | Menampilkan status perubahan saat ini dalam repositori.                                             | `-s` atau `--short`: Menampilkan status yang lebih singkat. <br> `--ignored`: Menampilkan file-file yang diabaikan.                                                                                                                                                              |
| `git log`      | `git log --oneline`                                      | Menampilkan riwayat komit dalam format yang ringkas.                                                | `-p` atau `--patch`: Menampilkan perubahan yang terjadi pada setiap komit. <br> `--author=<nama-penulis>`: Menampilkan riwayat komit hanya dari penulis tertentu. <br> `--graph`: Menampilkan riwayat komit dalam bentuk grafik.                                                 |
| `git remote`   | `git remote add origin https://github.com/user/repo.git` | Mengatur repositori jarak jauh yang dihubungkan dengan repositori lokal.                            | `add`: Menambahkan repositori jarak jauh baru. <br> `remove`: Menghapus repositori jarak jauh yang terhubung. <br> `rename`: Mengubah nama repositori jarak jauh yang terhubung.                                                                                                 |
| `git stash`    | `git stash save "Perubahan sementara"`                   | Menyembunyikan perubahan sementara yang belum siap untuk dikomit.                                   | `save`: Menyimpan perubahan sementara ke dalam penyimpanan sementara. <br> `apply`: Menerapkan kembali perubahan yang tersimpan. <br> `list`: Menampilkan daftar perubahan yang tersimpan.                                                                                       |
| `git reset`    | `git reset HEAD file.txt`                                | Membatalkan penambahan file ke daftar perubahan sebelum di-commit.                                  | `--soft`: Membatalkan perubahan dan menyimpannya sebagai perubahan yang belum di-staged. <br> `--mixed`: Membatalkan perubahan dan menyimpannya sebagai perubahan yang belum di-commit. <br> `--hard`: Membatalkan perubahan dan menghapus semua perubahan di working directory. |

Perintah-perintah di atas merupakan beberapa perintah Git yang umum digunakan dalam pengembangan perangkat lunak dengan Git. Opsi-opsi yang tercantum di atas adalah beberapa opsi yang sering digunakan, namun tidak mencakup semua opsi yang tersedia. Pastikan untuk membaca dokumentasi resmi Git atau menggunakan `git --help` untuk mempelajari lebih lanjut tentang setiap perintah dan opsi yang tersedia.

Berikut adalah tabel yang lebih lengkap dengan perintah Git yang paling sering digunakan dalam pekerjaan tim, termasuk format perintah, opsi, contoh, dan penjelasan:

| Perintah        | Opsi                      | Contoh                                           | Penjelasan                                                                                                                                                                                                                                                           |
| --------------- | ------------------------- | ------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| git clone       |                           | git clone <repository-url>                       | Menduplikasi repositori Git yang ada ke dalam direktori lokal. Perintah ini digunakan saat Anda ingin mengambil salinan dari repositori ke dalam komputer lokal untuk bekerja pada proyek tersebut.                                                                  |
| git pull        |                           | git pull                                         | Mengambil perubahan terbaru dari repositori pusat dan menerapkannya ke repositori lokal. Digunakan untuk memperbarui proyek lokal dengan perubahan yang dilakukan oleh anggota tim lainnya.                                                                          |
| git add         |                           | git add <file>                                   | Menambahkan file ke daftar "staged" sehingga perubahan pada file tersebut dapat dicatat pada commit berikutnya. Anda dapat menentukan nama file spesifik atau menggunakan tanda "\*" untuk menambahkan semua file.                                                   |
| git commit      | -m <message>              | git commit -m "Commit message"                   | Merekam perubahan pada repositori dengan pesan komit yang menjelaskan perubahan yang dilakukan. Commit adalah titik tertentu dalam sejarah proyek yang mencerminkan perubahan yang dilakukan pada file dan direktori.                                                |
| git push        |                           | git push                                         | Mengirim perubahan lokal ke repositori pusat. Setelah melakukan commit, Anda menggunakan perintah ini untuk mengunggah perubahan ke repositori pusat agar anggota tim lainnya dapat melihat dan menggunakan perubahan tersebut.                                      |
| git branch      |                           | git branch                                       | Menampilkan daftar cabang yang ada dalam repositori. Anda juga dapat menggunakan perintah ini untuk membuat cabang baru atau beralih ke cabang yang berbeda.                                                                                                         |
| git checkout    |                           | git checkout <branch-name>                       | Beralih ke cabang tertentu dalam repositori. Perintah ini juga dapat digunakan untuk memulihkan file atau direktori ke versi sebelumnya atau memulihkan file yang dihapus.                                                                                           |
| git merge       |                           | git merge <branch-name>                          | Menggabungkan perubahan dari satu cabang ke cabang lainnya. Misalnya, Anda dapat menggunakan perintah ini untuk menggabungkan perubahan dari cabang fitur ke cabang utama (master) setelah selesai mengembangkan fitur tersebut.                                     |
| git pull origin | <branch-name>             | git pull origin <branch-name>                    | Mengambil perubahan terbaru dari repositori pusat pada cabang tertentu. Berguna saat Anda ingin memperbarui cabang lokal dengan perubahan yang dilakukan oleh anggota tim di cabang pusat yang sama.                                                                 |
| git status      |                           | git status                                       | Menampilkan status repositori lokal, termasuk file-file yang sudah diubah atau ditambahkan, file-file yang sudah di-"staged" untuk commit, dan perubahan yang belum di-commit. Berguna untuk melihat status pekerjaan Anda saat ini.                                 |
| git log         |                           | git log                                          | Menampilkan sejarah commit dalam repositori, termasuk informasi seperti penulis, tanggal dan waktu komit, serta pesan komit yang menjelaskan perubahan apa yang dilakukan. Berguna untuk melihat riwayat pekerjaan yang telah dilakukan oleh Anda atau tim.          |
| git remote      | add / remove              | git remote add <name> <repository-url>           | Menambahkan atau menghapus repositori pusat yang terhubung ke repositori lokal. Dengan menambahkan repositori pusat, Anda dapat dengan mudah mengirim dan menerima perubahan ke repositori pusat yang sama yang digunakan oleh anggota tim lainnya.                  |
| git fetch       |                           | git fetch                                        | Mengambil perubahan terbaru dari repositori pusat tanpa menggabungkannya ke repositori lokal Anda. Perintah ini berguna saat Anda ingin melihat perubahan terbaru yang dilakukan oleh anggota tim, tetapi tidak ingin langsung menggabungkannya ke repositori lokal. |
| git reset       |                           | git reset HEAD <file>                            | Membatalkan perubahan pada file yang sudah di-"staged" untuk commit. File tersebut akan dikembalikan ke status sebelum di-"staged". Perintah ini berguna jika Anda ingin membatalkan penambahan file atau menghapus perubahan yang tidak perlu di-commit.            |
| git remote      | -v                        | git remote -v                                    | Menampilkan daftar repositori pusat yang terhubung ke repositori lokal beserta URL-nya. Berguna untuk melihat repositori pusat yang terhubung ke repositori lokal Anda.                                                                                              |
| git diff        |                           | git diff                                         | Menampilkan perbedaan antara file yang sudah diubah dan status terakhir yang dicatat oleh Git. Perintah ini berguna untuk melihat perubahan yang dilakukan pada file sebelum melakukan commit.                                                                       |
| git stash       | save / apply / pop / list | git stash save "Stash message" / git stash apply | Menyembunyikan perubahan yang belum di-commit dan memungkinkan Anda beralih ke cabang lain atau memulihkan perubahan tersebut nanti. Anda dapat menyimpan beberapa stash berbeda untuk mengelola perubahan sementara.                                                |
| git tag         |                           | git tag <tag-name>                               | Menandai titik tertentu dalam sejarah repositori dengan tag. Misalnya, Anda dapat menggunakan tag untuk menandai rilis versi atau poin penting dalam pengembangan proyek.                                                                                            |
| git cherry-pick |                           | git cherry-pick <commit-hash>                    | Mengambil satu atau beberapa commit tertentu dari cabang lain dan menerapkan perubahan tersebut ke cabang saat ini. Berguna saat Anda hanya ingin mengambil perubahan tertentu dari cabang lain tanpa harus menggabungkan keseluruhan cabang.                        |
| git rebase      |                           | git rebase <branch-name>                         | Mengaplikasikan perubahan dari satu cabang ke cabang lain dengan mengubah urutan commit. Berguna saat Anda ingin memperbarui cabang saat ini dengan perubahan yang ada di cabang lain dan menjaga sejarah commit tetap bersih dan linear.                            |

Perintah-perintah di atas merupakan perintah Git yang paling umum digunakan dalam pekerjaan tim. Anda dapat menggunakan tabel ini sebagai referensi

saat bekerja dengan Git dalam tim Anda.
