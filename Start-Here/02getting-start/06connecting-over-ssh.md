# Connecting over SSH

Pengguna tingkat lanjut (advanced users) sering kali lebih memilih untuk terhubung melalui remote shell.

Agar dapat melakukan SSH ke dalam instansi tantangan Anda, Anda harus menghubungkan kunci SSH publik (public SSH key) ke akun Anda melalui menu pengaturan (settings).

Anda dapat dengan cepat membuat kunci SSH dengan menjalankan perintah berikut di terminal pada mesin host Anda (yang mendukung sistem Unix):

```
ssh-keygen -f key -N ''
```

Perintah ini akan menghasilkan dua berkas: **key** dan **key.pub**, yang masing-masing merupakan kunci privat (private key) dan kunci publik (public key) Anda.

Setelah Anda menghubungkan kunci SSH publik ke akun Anda, Anda dapat terhubung ke dojo melalui SSH dengan perintah:

```
ssh -i key hacker@dojo.pwn.college
```

**[Step-By-Step SSH](06ssh.md)**

---

<table width="100%">
<tr>
<td align="left"><a href="05pasting-into-the-desktop.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../README.md">Home</a></td>

<td align="right"><a href="07restarting-challenges.md">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>