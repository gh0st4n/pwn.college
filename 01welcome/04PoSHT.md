# A Proof of (In)Security of Hacking Team

**A Proof of (In)Security of Hacking Team** adalah materi presentasi dari **pwn.college** yang mendokumentasikan studi kasus nyata pembobolan perusahaan teknologi keamanan siber (*Hacking Team*) oleh peretas Phineas Fisher sebagai bukti konkret ketidakamanan suatu sistem.

## Fitur dan Poin Utama Materi

- **Studi Kasus Pembobolan Hacking Team**
Membahas studi kasus nyata bagaimana seorang peretas bernama Phineas Fisher berhasil meretas perusahaan pembuat alat pengawas dan peretasan profesional (*Hacking Team*).

- **Tahapan Hacking the Hackers (Proses Serangan 6 Langkah)**
  1. **Step 1: Reconnaissance (Pengintaian Awal)** - Menganalisis infrastruktur publik Hacking Team yang sangat minim dan dijaga ketat.
  2. **Step 2: Gaining a Foothold (Mendapatkan Pijakan)** - Menemukan dan mengeksploitasi celah *zero-day* pada salah satu perangkat jaringan terdedikasi.
  3. **Step 3: Internal Reconnaissance (Pengintaian Internal)** - Melakukan pemantauan jaringan secara pasif dan pemindaian lambat hingga menemukan server rekaman audio keamanan fisik yang tidak diamankan.
  4. **Step 4: Gaining Influence (Memperluas Pengaruh)** - Bergerak secara lateral untuk memperluas akses dan kontrol di dalam jaringan internal.
  5. **Step 5: Total Compromise (Penguasaan Total)** - Mengambil alih seluruh sistem dan mengambil data internal perusahaan.
  6. **Step 6: Gloating (Publikasi)** - Mempublikasikan data hasil peretasan serta panduan cara meretasnya (*HackBack DIY Guide*).

- **Analisis Celah Keamanan (*What Went Wrong*)**
Menganalisis berbagai titik lemah yang dimanfaatkan, seperti ketiadaan autentikasi dua faktor (2FA), penggunaan ulang kata sandi (*password reuse*), akun pengguna biasa dengan hak akses *Domain Administrator*, serta tidak diisolasinya sistem cadangan (*backup storage*).

- **Asimetri Serangan dan Pertahanan (*Attack/Defense Asymmetry*)**
Menegaskan prinsip dasar bahwa sistem pertahanan hanya sekuat titik terlemahnya (*a chain is only as strong as its weakest link*). Tim bertahan harus menutup seluruh celah serangan, sementara peretas hanya perlu berhasil pada satu celah saja.

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) · [@Gh0sT4n](https://gh0st4n.my.id)

</div>