# Comparing Files

Saat mencari perubahan antara file yang serupa, mengamati secara visual mungkin bukan pendekatan yang paling efisien! Di sinilah perintah **diff** menjadi sangat berharga.

Perintah **diff** membandingkan dua file baris demi baris dan menunjukkan perbedaan persis di antara keduanya. Misalnya:

```
hacker@dojo:~$ cat file1
hello
world
hacker@dojo:~$ cat file2
hello
universe
hacker@dojo:~$ diff file1 file2
2c2
< world
---
> universe
```

Output tersebut menunjukkan bahwa baris 2 berubah (**2c2**), dengan kata **"world"** di berkas pertama (**<**) digantikan oleh kata "universe" di berkas kedua (**>**).

Terkadang, saat baris baru ditambahkan, Anda akan melihat sesuatu seperti:

```
hacker@dojo:~$ cat old
pwn
hacker@dojo:~$ cat new
pwn
college
hacker@dojo:~$ diff old new
1a2
> college
```

Ini memberi tahu kita bahwa setelah baris 1 di file pertama, file kedua memiliki baris tambahan (**1a2** berarti "setelah baris 1 dari file1, tambahkan baris 2 dari file2").

Sekarang giliran tantangan Anda! Ada dua file di **/challenge**:
    - File **/challenge/decoys_only.txt** berisi 100 bendera palsu.
    - File **/challenge/decoys_and_real.txt** berisi semua 100 bendera palsu ditambah satu bendera asli.

Gunakan perintah **diff** untuk menemukan perbedaan antara file-file ini dan dapatkan flag-nya!

---

<table width="100%">
<tr>
<td align="left"><a href="04grep.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../../../wREADME.md">Home</a></td>

<td align="right"><a href="06list">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>