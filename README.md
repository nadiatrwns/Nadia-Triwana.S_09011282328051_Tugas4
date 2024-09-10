### The following is article on how install Linux, I want you to format them for README Github, maket them looka bit fancy and keep the language in Indonesian:

## 1.	Lihat peralatan I/O, character device, yang ada pada system komputer.
![1](https://github.com/user-attachments/assets/a93cdbb5-4d8e-4b84-ad75-9a940e6359c9)
# Perintah ini akan menampilkan daftar file perangkat di direktori /dev yang merupakan character devices. Output yang ditampilkan hanya akan menyertakan baris yang diawali dengan c pada kolom pertama, menunjukkan bahwa file tersebut adalah character device.

## 2.	Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5.
![2](https://github.com/user-attachments/assets/60d1debf-255b-4290-be3a-1e477ff5be68)
# •	mkdir ~/latihan5: Direktori latihan5 akan dibuat di dalam direktori home.
# •	cd ~/latihan5: Kamu sekarang berada di dalam direktori latihan5.
# •	pwd: Terminal akan menampilkan jalur penuh dari direktori latihan5, misalnya /home/nama_pengguna/latihan5, sehingga kamu bisa memverifikasi bahwa kamu berada di direktori yang benar.
# •	mkdir januari februari maret: Tiga direktori tersebut akan muncul di dalam latihan5.
# •	ls: Terminal akan menampilkan nama-nama dari ketiga direktori yang baru saja dibuat (januari, februari, maret).

## 3.	Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari dan copy-kan file tersebut ke sub direktori februari dan maret.
![3](https://github.com/user-attachments/assets/d2bec0b9-9cef-4272-ae3e-ff5513bb92dd)
# •	echo -e "Nama: [Nama Kamu]\nNIM: [NIM Kamu]\nAlamat: [Alamat Kamu]" > januari/dataku: Sebuah file bernama dataku akan dibuat di dalam direktori januari, berisi informasi nama, NIM, dan alamat yang kamu masukkan.
# •	cp januari/dataku februari/: File dataku akan disalin dari direktori januari ke direktori februari.
# •	cp januari/dataku maret/: File dataku juga akan disalin dari direktori januari ke direktori maret.
# •	ls februari/ maret/: Terminal akan menampilkan daftar isi dari direktori februari dan maret, yang seharusnya mencakup file dataku.

## 4.	Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others dapat melakukan write.  
![4](https://github.com/user-attachments/assets/5f1e9d26-121c-4504-bf75-ffcceaa38756)
# •	chmod go+w januari/dataku: Izin tulis (write) akan diberikan kepada pengguna yang termasuk dalam kelompok (group) dan pengguna lain (others) untuk file dataku di dalam direktori januari. Setelah perintah ini dijalankan, group dan others akan memiliki izin untuk mengubah konten file dataku.
# •	ls -l januari/dataku: Terminal akan menampilkan informasi rinci tentang file dataku, termasuk izin aksesnya. 
# Penjelasan dari output:
# •	-rw-rw-rw- menunjukkan bahwa pemilik (user) dan group memiliki izin baca (r) dan tulis (w), serta others juga memiliki izin baca dan tulis. (Bagian pertama rw- adalah untuk pemilik, rw- untuk group, dan rw- untuk others).
# •	nadiatriwana nadiatriwana menunjukkan pemilik dan grup dari file tersebut.

## 5.	Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read dan execute.
![5](https://github.com/user-attachments/assets/24ec219f-8fec-4e7a-b14b-a69ad0df5d82)
# •	chmod 754 februari/dataku: Setelah menjalankan perintah ini, file dataku di dalam direktori februari akan memiliki izin sebagai berikut:
# 	Pemilik (user) bisa membaca, menulis, dan mengeksekusi file.
# 	Group bisa membaca dan mengeksekusi file.
# 	Others hanya bisa membaca file.
# •	ls -l februari/dataku: Terminal akan menampilkan informasi rinci tentang file dataku, termasuk izin aksesnya
# Penjelasan dari output :
# •	-rwxr-xr-- menunjukkan bahwa pemilik (user) memiliki izin baca (r), tulis (w), dan eksekusi (x) (rwx), group memiliki izin baca (r) dan eksekusi (x) (r-x), dan others hanya memiliki izin baca (r) (r--).
# •	nadiatriwana nadiatriwana menunjukkan pemilik dan grup dari file tersebut.
  
## 6.	Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat melakukan write, read dan execute.
![6](https://github.com/user-attachments/assets/8f4f79b4-6bee-4b9d-8ee5-2771297b429c)
# •	chmod 777 maret/dataku:Setelah menjalankan perintah ini, file dataku di dalam direktori maret akan memiliki izin sebagai berikut: Pemilik (user), group, dan others semuanya memiliki izin penuh untuk membaca, menulis, dan mengeksekusi file.
# •	ls -l maret/dataku: Terminal akan menampilkan informasi rinci tentang file dataku, termasuk izin aksesnya
# Penjelasan dari output :
# •	-rwxrwxrwx menunjukkan bahwa pemilik (user), group, dan others semuanya memiliki izin baca (r), tulis (w), dan eksekusi (x).
# •	nadiatriwana nadiatriwana menunjukkan pemilik dan grup dari file tersebut.

## 7.	Hapuslah direktori maret.
![7](https://github.com/user-attachments/assets/7047e076-0fe5-46da-bb9f-a832a7a71a09)
# •	rm -r maret: Direktori maret dan semua file serta subdirektori yang ada di dalamnya akan dihapus secara permanen.
# •	ls: Terminal akan menampilkan daftar semua file dan direktori yang tersisa di dalam direktori saat ini. Jika perintah rm -r maret berhasil, maka direktori maret tidak akan muncul lagi dalam daftar ini.

## 8.	Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori februari. 
![8](https://github.com/user-attachments/assets/d97175f3-473f-419a-9ac3-0308416bff7e)
# •	ls -ld februari: Menampilkan informasi lengkap tentang direktori februari, termasuk izin aksesnya.
# •	chmod u+w februari: Pemilik dari direktori februari sekarang memiliki izin untuk menulis (write) ke dalam direktori tersebut, yang berarti mereka bisa membuat, mengubah, atau menghapus file/direktori di dalamnya.
# •	chmod 777 februari: Semua pengguna (pemilik, grup, dan others) akan memiliki izin penuh untuk membaca, menulis, dan mengeksekusi dalam direktori februari.
# •	mkdir februari/haha: Direktori baru bernama haha akan dibuat di dalam direktori februari.

## 9.	Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan nilai default-nya ?
![9](https://github.com/user-attachments/assets/52f5c4f9-5753-463f-918c-3d3d711b2fd9)
# •	umask: Menampilkan nilai umask saat ini.
# •	umask 027: Mengatur umask sehingga file baru dibuat dengan izin yang lebih ketat, biasanya 640 untuk file dan 750 untuk direktori.
# •	touch januari/dataku: Membuat file dataku dengan izin yang diatur oleh umask 027, yang berarti izin file ini adalah 640.
# •	umask 022: Mengembalikan umask ke pengaturan yang lebih permisif, 022.

## 10.	Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah list perhatikan berapa link yang terjadi ?
![10](https://github.com/user-attachments/assets/db715eb3-fb99-43f2-82b2-1ed0ace3c7fe)
# •	cd januari: Pindah ke direktori januari.
# •	ln dataku dataku.ini dan ln dataku dataku.juga: Membuat dua hard link dari file dataku.
# •	ls -l dataku*: Menampilkan rincian file asli dan hard link-nya, menunjukkan bahwa ketiganya merujuk pada data yang sama dengan jumlah link yang sama.
# Penjelasan dari output :
# •	-rw-r----- menunjukkan izin akses (read and write untuk owner, read untuk group, none untuk others).
# •	3 menunjukkan jumlah link (tiga nama file yang menunjuk ke data fisik yang sama).
# •	68 adalah ukuran file dalam byte.
# •	Sep 5 10:12 adalah waktu modifikasi terakhir.
# •	dataku, dataku.ini, dan dataku.juga semuanya merujuk pada data yang sama di disk.
