# 1.	Lihat peralatan I/O, character device, yang ada pada sistem komputer:
![1](https://github.com/user-attachments/assets/ae7703da-d309-4bff-852b-62ca7d9c9253)

**Penjelasan:** ls -l /dev menampilkan isi dari direktori /dev, yang merupakan tempat file device disimpan. grep "^c" digunakan untuk menyaring hanya character devices (ditandai dengan huruf "c").

# 2.	Buat subdirektori Januari, Februari, dan Maret sekaligus pada direktori latihan5:
![2](https://github.com/user-attachments/assets/0f45020b-ba32-4292-81c0-03b73fddd7c8)

**Penjelasan:** mkdir -p akan membuat direktori beserta subdirektori jika belum ada.

# 3.	Buat file dataku yang berisi nama, NIM, dan alamat pada subdirektori Januari dan copy ke Februari dan Maret:
![3](https://github.com/user-attachments/assets/bb42ed02-f5b1-41e9-a47c-443d69ff0ea1)

**Penjelasan:** echo digunakan untuk menulis isi file, cp untuk menyalin file.

# 4.	Ubah izin akses file dataku di Januari sehingga group dan others dapat write:
![4](https://github.com/user-attachments/assets/18f71197-fe04-44e3-a142-adca1ed5bfd5)

**Penjelasan:** chmod 666 memberikan izin read dan write untuk user, group, dan others.

# 5.	Ubah izin akses file dataku di Februari sehingga user dapat read, write, execute, dan group serta others hanya bisa read dan execute:
![5](https://github.com/user-attachments/assets/0af2ff84-aa3c-46cb-9b35-5432dcf222fd)

**Penjelasan:** chmod 755 memberikan izin penuh (rwx) untuk user, dan read-execute (rx) untuk group dan others.

# 6.	Ubah izin akses file dataku di Maret sehingga semua dapat write, read, dan execute:
![6](https://github.com/user-attachments/assets/71a30a8f-d288-449c-b113-9ff2e33203cc)

**Penjelasan:** chmod 777 memberikan izin penuh untuk user, group, dan others.

# 7.	Hapus direktori Maret:
![7](https://github.com/user-attachments/assets/06900434-814e-4720-a6da-51380224e0a9)

**Penjelasan:** rm -r digunakan untuk menghapus direktori beserta isinya.

# 8.	Ubah kepemilikan direktori Februari sehingga user dan group hanya dapat read, dan coba buat direktori baru haha pada subdirektori Februari:
![8](https://github.com/user-attachments/assets/a154a790-0646-449c-a527-7463ac5ab9cc)

**Penjelasan:** chmod 444 memberikan izin read-only. Percobaan membuat direktori haha akan gagal karena tidak ada izin write.

# 9.	Modifikasi umask dari file dataku pada Januari menjadi 027 dan cek nilai default-nya:
![9](https://github.com/user-attachments/assets/f3f6fd08-d2e3-4261-976a-b3ae73ebb863)

**Penjelasan:** umask 027 mengatur umask baru, umask digunakan untuk menampilkan nilai umask saat ini.

# 10.	Buat link dari file dataku ke file dataku.ini dan file dataku.juga dan lihat jumlah link-nya:
![10](https://github.com/user-attachments/assets/961694f2-8b3e-4c01-aaad-0d7628162c75)

**Penjelasan:** ln digunakan untuk membuat hard link. ls -l akan menunjukkan jumlah link pada file (2 link tambahan berarti total link menjadi 3).
