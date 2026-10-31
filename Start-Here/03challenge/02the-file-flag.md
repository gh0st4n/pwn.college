# The File Flag

Sejauh ini, tantangan-tantangan sebelumnya telah memberikan *flag* kepada Anda secara langsung.

Dalam tantangan ini, Anda akan mempelajari bahwa *flag* sebenarnya tersimpan di dalam berkas `/flag`.

Tujuan utama Anda yang sebenarnya dalam setiap tantangan adalah mendapatkan isi dari berkas ini melalui cara apa pun yang memungkinkan, bahkan jika program tantangan tersebut tidak sengaja menampilkannya secara langsung.

Anda mungkin mencoba untuk sekadar membaca berkas `/flag` secara mandiri.

Namun sayangnya, Anda menjalankan sesi sebagai pengguna `hacker` dan berkas `/flag` hanya dapat dibaca oleh pengguna `root`, sehingga Anda tidak dapat mengakesnya secara langsung.

Pada tantangan-tantangan sebelumnya, program tantangan itu sendiri (seperti `/challenge/solve`) yang berjalan sebagai pengguna `root` (dan dengan demikian memiliki izin untuk membaca *flag*), membaca berkas tersebut lalu mencetak isinya. Namun, level ini sedikit lebih sulit.

Seperti banyak tantangan lain di platform ini, program `/challenge/solve` pada tantangan ini tidak akan membaca berkas *flag* secara langsung.

Akan tetapi, program tersebut akan mengubah izin berkas *flag* menjadi dapat dibaca oleh siapa saja (*world-readable*) saat Anda menjalankannya!

Setelah itu, Anda perlu membaca berkas `/flag` tersebut sendiri (misalnya, menggunakan perintah `cat /flag` atau menggunakan editor teks), lalu mengirimkan isinya sebagai solusi.

---

<table width="100%">
<tr>
<td align="left"><a href="01challenge-program.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../../README.md">Home</a></td>

<td align="right"><a href="03using-privileged-mode.md">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>