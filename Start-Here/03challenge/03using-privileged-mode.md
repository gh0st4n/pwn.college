# Using Privileged Mode

Anda dapat menjalankan tantangan dalam dua mode dengan menggunakan tombol-tombol di bawah ini!

Sejauh ini, Anda telah menggunakan tombol **Start**, yang menjalankan tantangan sehingga Anda dapat mencoba menyelesaikannya secara nyata.

Anda juga dapat memulai tantangan dengan tombol **Privileged!**

Mode ini akan memberi Anda hak akses administratif (melalui `sudo`) di dalam kontainer tantangan. Hak akses ini memberikan kemampuan yang lebih besar untuk melakukan debugging pada solusi Anda maupun bereksperimen dengan tantangan tersebut.

Anda tidak dapat menggunakan mode ini untuk benar-benar menyelesaikan tantangan, karena berkas `/flag` pada mode privileged diganti dengan "practice flag" (flag latihan) yang tidak dapat ditukarkan dengan poin.

Anda tidak pernah membutuhkan mode Privileged untuk menyelesaikan suatu tantangan, kecuali untuk tantangan yang satu ini, karena level ini memang dirancang khusus untuk memperkenalkan Anda pada mode Privileged.

Tantangan ini memiliki berkas `/challenge/secret` yang hanya dapat dibaca oleh pengguna `root`, namun isinya tidak berubah antara mode Privileged dan mode normal.

Untuk menyelesaikan tantangan ini:

1. Jalankan tantangan dalam mode Privileged.
2. Baca berkas `/challenge/secret`.
3. Jalankan kembali tantangan dalam mode normal (menggunakan tombol **Start**).
4. Masukkan kode rahasia (secret) tersebut saat program /challenge/solve memintanya.

---

<table width="100%">
<tr>
<td align="left"><a href="02the-file-flag.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../../README.md">Home</a></td>

<td align="right"><a href="04persistant-home-dir-one.md">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>