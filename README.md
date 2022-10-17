# CORETAN UNTUK UBUNTU

## 1. Belajar Dasar comand linux.

### A. Pengenalan Linux.
Tujuan awal dari Ubuntu adalah menciptakan sebuah sistem operasi desktop Linux yang mudah dipakai oleh pengguna komputer. Sejak perilisan pertama pada 20 Oktober 2004, Canonical merilis versi Ubuntu setiap 6 bulan sekali. Setiap rilis nya akan menerima dukungan gratis selama 9 bulan (18 bulan sebelum 13.04) dengan pembaruan sistem, perbaikan keamanan dan perbaikan kesalahan / bug berdampak tinggi dan berisiko rendah yang konservatif.

#### a. Cek user yg d gunakan dapat menggunakan perintah `whoami`.

```
whoami
```

##### Contoh

```
user@host:~$ whoami
kunti
```

#### b. Print working directory terminal sedang berada pada directory mana dapat menggunakan perintah `pwd`.

```
pwd
```

##### Contoh

```
user@host:~$ pwd
/home/kunti
```

#### c. Melihat panduan dari sebuah perintah di terminaldapat menggunakan perintah `man` dan cara untuk exit adalah dengan menekan tombol `Q`.

```
man <perintah yang kita akan belum mengerti>
```

##### Contoh

```
user@host:~$ man pwd
DESCRIPTION
  Print the full filename of the current working directtory.
  
  -L, --logical
    use PWDfrom environment, even if it contains symlinks
```

#### d. melihat  folder dan file pada directory di terminaldapat menggunakan perintah `ls`.

```
ls
```

##### Contoh

```
user@host:~$ ls
folder1 folder2 file1 file2
```

#### e. melihat  folder dan file  semua termasud yg hiden pada directory di terminaldapat menggunakan perintah `ls -a`.

```
ls -a
```

##### Contoh

```
user@host:~$ ls
folder1 folder2 file1 file2 .bash1 .bash2 .bash3
```

#### f. membersihkan terminal agar kembali kosong dapat menggunakan perintah `clear`.

```
clear
```

##### Contoh

```
user@host:~$ clear
```


#### g. membuat file timestamp dapat menggunakan perintah `touch`.

```
touch <nama file>
```

##### Contoh

```
user@host:~$ touch data.txt
```

#### h. membuat file dapat menggunakan perintah `file`.

```
file <nama file>
```

##### Contoh

```
user@host:~$ file data.txt
```

#### i. membuat folder baru dapat menggunakan perintah `mkdir` make directory.

```
mkdir <nama file>
```

##### Contoh

```
user@host:~$ mkdir folder1
user@host:~$ ls
folder1
```

#### j. pindah lokasi workspace terminal dapat menggunakan perintah `cd` change directory.

```
cd <lokasi tujuan>
```

##### Contoh

```
user@host:~$ cd /home/
```

#### k. copy file atau folder dapat menggunakan perintah `cp` copy.

```
cp <nama file / folder>
```

##### Contoh

```
user@host:~$ cp file1
```

#### l. menghapus file dapat menggunakan perintah `rm` remove.

```
rm <nama file>
```

##### Contoh

```
user@host:~$ rm file1.txt
```

#### m. menghapus folder dapat menggunakan perintah `rmdir` remove directory.

```
rmdir <nama file / folder>
```

##### Contoh

```
user@host:~$ rmdir folder1
```

#### n. membuat dua folder sekaligus dalam posisi parent dapat menggunakan perintah `mkdir -p` make directory parent.

```
mkdir <nama folder induk>/<nama folder anak> -p
```

##### Contoh

```
user@host:~$ mkdir folder_angka/folder1 -p
```

#### o. menghapus folder dengan isinya dapat menggunakan perintah `rmdir -r` remove directory recursive.

```
rmdir <nama file> -r
```

##### Contoh

```
user@host:~$ cp file_angka -r
```
#### p. menjalankan perintah dengan superuser dapat menggunakan perintah `sudo`.

```
sudo <perintah>
```

##### Contoh

```
user@host:~$ sudo python3 data.py
```

#### q. merubah user dengan superuser dapat menggunakan perintah `sudo su` dan isi password superuser.

```
sudo su
```

##### Contoh

```
user@host:~$ sudo su

```
#### r. keluar dapat menggunakan perintah `exit`.

```
exit
```

##### Contoh

```
user@host:~$ exit
```



### B. Linux Shell Command.
#### a. `apt`.

```
Command-line interface update upgrade install remove dll (  )
```

##### Contoh

```
user@host:~$ apt update
user@host:~$ apt upgrade
user@host:~$ apt install xxxx
user@host:~$ apt remove xxxx
```

#### b. `Sources.list `.

```
cd /etc/apt.  
```

##### Contoh

```
user@host:~$ sudo nano source.list
```


#### c. `Sources.list `.

```
cd /etc/apt.  
```

##### Contoh

```
user@host:~$ sudo nano source.list
```



### C. Permission,Redirection.

#### a. `Redirection  `.

```
output sebelum perintah dan diteruskan ke sebagai file atau di lanjutkan sebagai perintah (ls > ls.txt) menampilkan hais dari perintah ls ke ls.txt , cat ls.txt
```
```
jika ingin mengabungkan tampa menimpa isi maka (ls -la >> ls.txt)
```
```
input redirection, input sebum data dari sebuah file atai perintah (wc -c < ls.txt). 
```

#### b. `Find  `.

```
Find . -iname *.txt
```


#### c. `Grep `.

```
akan print basis matching dengan pattern (ls | grep *.txt) meneruskan output hasil ke perintah selanjutnya.
```

#### d. `Dan / && `.

```
menjalankan perintah berurutan (ls && whom)
```

#### e. `Permissions`.

```
Permissions: hak akses (ls -a) owner group other
```
value of permission<br />
r read 4 <br />
w write 2 <br />
x execute 1<br /><br />

owner Rwx 421 =7<br />
group r-x 401 5<br />
other r-x 401 5<br /><br />

ls.txt 644 -> 755<br />(chmod 755 ls.txt)

### D. Terminal Linux.
#### a. `baground`.

```
menjalankan d belakang layar
```
```
nano &
```

#### b. `Jobs`.

```
cek app berjalan 
```

#### c. `foreground `.

```
foreground : menampilkan app aground menjadi di depan layar (fg 1)
```

#### c. `PS`.

```
Ps : menampillkan isi dari proses yang sedans berjalan 
```
```
Ps aux :menampilkan proses detail
```

#### d. `Top`.

```
top -bc:match mode c comment line( top -bc | grep nano) stop  dental control c
```

#### e. `Renice `.

```
Renice : (sudo renice -n -17 -p 5102) ni : nice / priorités -20 sampan -29  
```


### E. Coretan Ahir.
#### a. Membuat directory seperti Struktur dibawah :<br />
kodio<br />
-Programing<br />
- C<br />
- Java<br />
- -Networking<br />
- Mikrotik

```
mkdir -p Kodio/{Programing/{C,Java},Networking/Mikrotik}
```

#### b. Membuat file history.txt yang berisikan perintah yang telah digunakan sebelumny
```
history > history.txt
```

#### c. Melakukan upgrade fitter menggunakan automatisasi saat terdapat from pertanyaan yes or no
```
sudo apt upgrade -y
```

#### d. Melakukan backup dengan mengcopy source.list ke sebuah file baru bernama source.list.backup
```
sudo cp /etc/apt/sourcelist /etc/apt/source.list.backup
```

#### e. Melakukan perintah update dan upgrade pada satu perintah
```
sudo apt update && sudo apt upgrade
```

#### f. Melakukan pencarian file dengan extension “.txt” di folder saatini:
```
find . -name “*.txt”
```

#### g. Menampilkan history perintah yang memiliki kata “sudo” didalamny
```
history | grep sudo
```

#### h. Membuat file history.txt memiliki has role <br />
user : read write dan execute 7<br />
group dan other : read 44
```
chmod 744 history.txt
```
#### i. Menampilkan semi proses yang sedang berjalan perintah ps
```
PS AUX
```

#### J.menampilkan proses bedasarkan penggunaan memory terrendah ke tertinggi dengan perintah top
```
top -o -%MEM
```






