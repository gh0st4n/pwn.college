# Cat : not the pet, but the command

Salah satu perintah Linux yang paling krusial adalah **cat**. **cat** paling sering digunakan untuk membaca dan menampilkan isi berkas, seperti ini:

```
hacker@dojo:~$ cat /path/to/file
Hello Hackers!
```

**cat** akan menggabungkan (concatenate, dari sinilah namanya berasal) beberapa berkas jika Anda memberikan beberapa argumen sekaligus.Sebagai contoh:

```
hacker@dojo:~$ cat myfile
This is my file!
hacker@dojo:~$ cat yourfile
This is your file!
hacker@dojo:~$ cat myfile yourfile
This is my file!
This is your file!
hacker@dojo:~$ cat myfile yourfile myfile
This is my file!
This is your file!
This is my file!
```

Terakhir, jika Anda tidak memberikan argumen sama sekali, **cat** akan membaca masukan langsung dari terminal dan menampilkannya kembali sebagai keluaran. Kita akan mengeksplorasi hal tersebut pada tantangan-tantangan berikutnya...

Pada tantangan ini, saya akan menyalin flag ke berkas bernama **flag** yang berada di dalam direktori home Anda (tempat shell Anda dimulai).

Buka dan baca berkas tersebut menggunakan **cat**!

---

<table width="100%">
<tr>
<td align="left"><a href="00.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../../../wREADME.md">Home</a></td>

<td align="right"><a href="02catting.md">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>
