# A Proof of (In)Security of Hacking Team

**A Proof of (In)Security of Hacking Team** adalah materi presentasi dari **pwn.college** yang mendokumentasikan studi kasus nyata pembobolan perusahaan teknologi keamanan siber (_Hacking Team_) oleh peretas Phineas Fisher sebagai bukti konkret ketidakamanan suatu sistem.

## Fitur dan Poin Utama Materi

- **Studi Kasus Pembobolan Hacking Team**

  Membahas studi kasus nyata bagaimana seorang peretas bernama Phineas Fisher berhasil meretas perusahaan pembuat alat pengawas dan peretasan profesional (_Hacking Team_).

- **Tahapan Hacking the Hackers (Proses Serangan 6 Langkah)**
  - **Step 1: Reconnaissance (Pengintaian Awal)** - Menganalisis infrastruktur publik Hacking Team yang sangat minim dan dijaga ketat.
  - **Step 2: Gaining a Foothold (Mendapatkan Pijakan)** - Menemukan dan mengeksploitasi celah _zero-day_ pada salah satu perangkat jaringan terdedikasi.
  - **Step 3: Internal Reconnaissance (Pengintaian Internal)** - Melakukan pemantauan jaringan secara pasif dan pemindaian lambat hingga menemukan server rekaman audio keamanan fisik yang tidak diamankan.
  - **Step 4: Gaining Influence (Memperluas Pengaruh)** - Bergerak secara lateral untuk memperluas akses dan kontrol di dalam jaringan internal.
  - **Step 5: Total Compromise (Penguasaan Total)** - Mengambil alih seluruh sistem dan mengambil data internal perusahaan.
  - **Step 6: Gloating (Publikasi)** - Mempublikasikan data hasil peretasan serta panduan cara meretasnya (_HackBack DIY Guide_).

- **Analisis Celah Keamanan (_What Went Wrong_)**

  Menganalisis berbagai titik lemah yang dimanfaatkan, seperti ketiadaan autentikasi dua faktor (2FA), penggunaan ulang kata sandi (_password reuse_), akun pengguna biasa dengan hak akses _Domain Administrator_, serta tidak diisolasinya sistem cadangan (_backup storage_).

- **Asimetri Serangan dan Pertahanan (_Attack/Defense Asymmetry_)**

  Menegaskan prinsip dasar bahwa sistem pertahanan hanya sekuat titik terlemahnya (_a chain is only as strong as its weakest link_). Tim bertahan harus menutup seluruh celah serangan, sementara peretas hanya perlu berhasil pada satu celah saja.

---

<table width="100%">
<tr>
<td align="left"><a href="03proving_cybersecurity.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../README.md">Home</a></td>

<td align="right"><a href="05CybersecurityEthics.md">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>
