# Implicit Relative PATH, from `/`

Sekarang Anda sudah familiar dengan konsep merujuk ke jalur absolut (absolute paths) dan mengubah direktori.

Jika Anda menggunakan jalur absolut di mana saja, maka tidak masalah di direktori mana Anda berada, seperti yang mungkin sudah Anda temukan pada tiga tantangan sebelumnya.

Namun, direktori kerja saat ini (current working directory / `cwd`) sangat berpengaruh untuk jalur relatif (relative paths).

- Jalur relatif adalah semua jalur yang tidak dimulai dari root (artinya, tidak dimulai dengan karakter `/`).
- Jalur relatif diinterpretasikan relatif terhadap direktori kerja Anda saat ini (`cwd`).
- `cwd` Anda adalah direktori tempat prompt Anda berada saat ini.

Ini berarti cara Anda menentukan berkas tertentu tergantung pada lokasi prompt terminal berada.

Bayangkan kita ingin mengakses sebuah berkas yang terletak di `/tmp/a/b/my_file`:
- Jika `cwd` saya adalah `/`, maka jalur relatif ke berkas tersebut adalah `tmp/a/b/my_file`.
- Jika `cwd` saya adalah `/tmp`, maka jalur relatif ke berkas tersebut adalah `a/b/my_file`.
- Jika `cwd` saya adalah `/tmp/a/b/c`, maka jalur relatif ke berkas tersebut adalah `../my_file`. Karakter `..` merujuk pada direktori induk (*parent directory*).

Mengubah direktori dan menjalankan program adalah dua tindakan yang terpisah.

Sebagai contoh:
```
hacker@dojo:~$ cd /
hacker@dojo:/$ bin/echo Hello
Hello
```

1. Perintah pertama mengubah direktori kerja saat ini ke `/`.
2. Perintah kedua menjalankan `/bin/echo` menggunakan jalur relatif `bin/echo`.

Mari kita coba di sini!

Pertama, ubah direktori kerja Anda saat ini ke `/`. Kemudian jalankan `/challenge/run` menggunakan jalur relatif.

Untuk level ini, saya akan memberi Anda petunjuk (hint):
Jalur relatif Anda dimulai dengan huruf `c` 😊

---

<table width="100%">
<tr>
<td align="left"><a href="05position-elsewhere.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../../../README.md">Home</a></td>

<td align="right"><a href="07explicit-relative-path-from-slash.md">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>
