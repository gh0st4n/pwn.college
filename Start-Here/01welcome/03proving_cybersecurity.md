# Proving Cybersecurity (Failures)

**Proving Cybersecurity (Failures)** adalah materi presentasi dari **pwn.college** yang menjelaskan konsep logika, model keamanan, serta metode di balik pembuktian keamanan maupun ketidakamanan suatu sistem perangkat lunak.

## Fitur dan Poin Utama Materi

- **Membuktikan Keamanan vs Ketidakamanan**

  Membuktikan suatu sistem aman secara mutlak sangat sulit karena harus membuktikan ketiadaan celah sama sekali (_proving a negative_). Sebaliknya, membuktikan sistem tidak aman sangat lugas (_straightforward_), yaitu cukup dengan menunjukkan satu kerentanan nyata (_"You can't argue with a root shell"_).

- **Analogi Pembuktian Logika Matematika**

  Proses pembuktian ketidakamanan mengadopsi logika geometri/matematika: menggunakan **Aksioma** (kondisi & konfigurasi perangkat lunak), **Model Keamanan** (seperti prinsip CIA), dan **Metode** (teknik peretasan & kerentanan) untuk menghasilkan bukti logis.

- **Model Keamanan pwn.college**

  Hampir seluruh tantangan di pwn.college menggunakan aturan model keamanan mendasar: pengguna/hacker tidak boleh bisa memanipulasi sistem untuk membaca atau membocorkan isi dari file `/flag`.

- **Eksploit sebagai Bukti Konkret (The Proof)**

  Dalam dunia keamanan siber, bukti ketidakamanan diwujudkan dalam bentuk **exploit**. Eksploit memanfaatkan kerentanan yang ada untuk melanggar kerahasiaan (_Confidentiality_) file `/flag` dan membocorkannya demi mendapatkan poin.

---

<table width="100%">
<tr>
<td align="left"><a href="02introduction.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../README.md">Home</a></td>

<td align="right"><a href="04PoSHT.md">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>
