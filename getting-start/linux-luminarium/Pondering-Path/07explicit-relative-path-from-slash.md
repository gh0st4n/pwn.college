# Explicit Relative PATH, from `/`

Sebelumnya, jalur relatif Anda bersifat "polos" (*naked*): jalur tersebut langsung menentukan direktori mana yang akan dituju dari direktori saat ini.

Pada level ini, kita akan mengeksplorasi jalur relatif yang lebih eksplisit.

Di sebagian besar sistem operasi, termasuk Linux, setiap direktori memiliki dua entri tersirat (implicit entries) yang dapat Anda rujuk dalam jalur (*path*): `.` dan `...`

Entri pertama, yaitu `.`, merujuk tepat ke direktori yang sama, sehingga jalur-jalur absolut berikut ini semuanya bernilai identik satu sama lain:

- `/challenge`
- `/challenge/.`
- `/challenge/./././././././././`
- `/./././challenge/././`

Jalur-jalur relatif berikut ini juga semuanya identik satu sama lain:
- `challenge`
- `./challenge`
- `./././challenge`
- `challenge/.`

Tentu saja, jika direktori kerja Anda saat ini (current working directory) adalah `/`, maka jalur relatif di atas akan setara dengan jalur absolut di atas.

Tantangan ini akan melatih Anda menggunakan `.` dalam jalur relatif Anda.

Direktori kerja Anda saat ini harus berada di `/`, dan jalur relatif yang Anda gunakan untuk menjalankan tantangan harus dimulai dengan karakter `.` .

Bersiaplah!

---

<table width="100%">
<tr>
<td align="left"><a href="06implicit-relative-path-from-slash.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../../../README.md">Home</a></td>

<td align="right"><a href="08implicit-relative-path.md">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>