# Home Sweet Home

Setiap pengguna memiliki direktori *home*, biasanya terletak di bawah direktori `/home` dalam sistem berkas (*filesystem*).

Di dalam *dojo*, Anda adalah pengguna `hacker`, dan direktori home Anda terletak di `/home/hacker`.

Direktori *home* biasanya menjadi tempat pengguna menyimpan sebagian besar berkas pribadi mereka.

Seiring berjalannya waktu saat Anda menyelesaikan tantangan di pwn.college, di sinilah Anda akan menyimpan sebagian besar solusi Anda.

Biasanya, sesi *shell* Anda akan dimulai dengan direktori *home* sebagai direktori kerja saat ini (*current working directory*).

Perhatikan prompt awal berikut:
```
hacker@dojo:~$
```

Karakter `~` (tilde) pada prompt ini menunjukkan direktori kerja saat ini, di mana `~` merupakan singkatan (shorthand) dari /home/hacker.

Bash menyediakan dan menggunakan singkatan ini karena sebagian besar waktu Anda akan dihabiskan di dalam direktori `home`.

Oleh karena itu, kapan pun bash mendeteksi `~` diberikan di awal argumen yang sesuai dengan format jalur (`path`), bash akan mengekspansinya menjadi direktori `home` Anda.

Perhatikan contoh berikut:

```
hacker@dojo:~$ echo LOOK: ~
LOOK: /home/hacker
hacker@dojo:~$ cd /
hacker@dojo:/$ cd ~
hacker@dojo:~$ cd ~/asdf
hacker@dojo:~/asdf$ cd ~/asdf
hacker@dojo:~/asdf$ cd ~
hacker@dojo:~$ cd /home/hacker/asdf
hacker@dojo:~/asdf$
```

Perlu dicatat bahwa ekspansi dari `~` menghasilkan jalur absolut (*absolute path*), dan hanya karakter `~` di paling awal yang akan diekspansi.

Ini berarti, sebagai contoh, `~/~` akan diekspansi menjadi `/home/hacker/~` dan bukan `/home/hacker/home/hacker`.

**Fakta menarik**: Perintah `cd` tanpa argumen akan menggunakan direktori home Anda sebagai tujuan bawaan (*default*):

```
hacker@dojo:~$ cd /tmp
hacker@dojo:/tmp$ cd
hacker@dojo:~$
```

Sekarang giliran Anda untuk mencoba!

Pada tantangan ini, `/challenge/run` akan menuliskan salinan *flag* ke berkas apa pun yang Anda tentukan sebagai argumen pada *command line*, dengan batasan berikut:

1. Argumen Anda harus berupa jalur absolut (*absolute path*).
2. Jalur tersebut harus berada di dalam direktori *home* Anda.
3. Sebelum diekspansi oleh bash, argumen Anda harus terdiri dari **3 karakter atau kurang**.

Sekali lagi, Anda harus menentukan jalur Anda sebagai argumen untuk `/challenge/run` seperti ini:
```
hacker@dojo:~$ /challenge/run YOUR_PATH_HERE
```

---

<table width="100%">
<tr>
<td align="left"><a href="08implicit-relative-path.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../../../README.md">Home</a></td>

<td align="right"><a href="../comprehending-commands/00.md">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>