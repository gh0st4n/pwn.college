# implicit relative path

Pada level ini, kita akan lebih banyak berlatih merujuk pada jalur (*paths*) menggunakan entri `.` .

Tantangan ini mengharuskan Anda untuk menjalankannya langsung dari dalam direktori `/challenge`.

Di sinilah hal-hal mulai sedikit rumit.

Sistem operasi Linux secara eksplisit mecegah pencarian otomatis di dalam direktori saat ini jika Anda hanya memasukkan jalur yang "polos" (*naked path*).

Perhatikan contoh berikut:
```
hacker@dojo:~$ cd /challenge
hacker@dojo:/challenge$ run
```

Perintah di atas tidak akan mengeksekusi `/challenge/run`.

Ini sebenarnya merupakan sebuah langkah keamanan: jika Linux selalu mencari program di dalam direktori saat ini setiap kali Anda memasukkan nama perintah/jalur polos, Anda bisa saja secara tidak sengaja mengeksekusi program di direktori tersebut yang kebetulan memiliki nama yang sama dengan utilitas inti sistem!

Akibatnya, perintah di atas akan menghasilkan pesan kesalahan (*error*) berikut:
```
bash: run: command not found
```

Kita akan mengeksplorasi mekanisme di balik konsep ini nanti. Namun pada tantangan ini, kita akan belajar cara menggunakan jalur relatif secara eksplisit untuk menjalankan program *run* dalam skenario seperti ini.

Caranya adalah dengan memberi tahu Linux secara eksplisit bahwa Anda ingin mengeksekusi program yang berada di direktori saat ini, yaitu dengan menggunakan `.` seperti pada level-level sebelumnya.

Coba lakukan sekarang!

---

<table width="100%">
<tr>
<td align="left"><a href="07explicit-relative-path-from-slash.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../../../README.md">Home</a></td>

<td align="right"><a href="09home-sweet-home.md">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>
