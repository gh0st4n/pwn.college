## 1. Buat SSH key

Di terminal Linux/macOS (atau WSL / Git Bash di Windows):

```bash
ssh-keygen -f key -N ''
```

- `-f key` : nama file output (`key` = private key, `key.pub` = public key)
- `-N ''` : tanpa passphrase

Kalau mau lebih rapi dan aman, simpan di folder `~/.ssh` dan pakai algoritma modern:

```bash
ssh-keygen -t ed25519 -f ~/.ssh/pwncollege -N ''
```

Opsional: ganti `-N ''` dengan passphrase kalau mau kuncinya terlindungi.

## 2. Daftarkan public key ke akun

1. Tampilkan isi public key:
   ```bash
   cat key.pub
   ```
   (atau `cat ~/.ssh/pwncollege.pub` kalau pakai cara kedua)
2. Salin seluruh isinya (satu baris, diawali `ssh-ed25519` atau `ssh-rsa`).
3. Login ke pwn.college, buka **Settings**, cari bagian **SSH Key**, tempel public key, lalu simpan.

**Penting:** yang ditempel hanya file `.pub`. Jangan pernah membagikan private key (`key`).

## 3. Atur permission private key

SSH menolak private key yang permission-nya terlalu terbuka:

```bash
chmod 600 key
```

## 4. Mulai challenge, lalu connect

Challenge instance harus sudah berjalan. Buka challenge di website pwn.college, klik **Start** (mode Normal atau Privileged), baru kemudian jalankan:

```bash
ssh -i key hacker@dojo.pwn.college
```

Kalau key disimpan di `~/.ssh/pwncollege`:

```bash
ssh -i ~/.ssh/pwncollege hacker@dojo.pwn.college
```

Setelah masuk, kamu berada di shell container challenge sebagai user `hacker`. Dari sana kamu bisa menjalankan `/challenge/...`, debugging dengan gdb, dan seterusnya.

## 5. (Opsional) Permudah dengan SSH config

Supaya tidak perlu mengetik panjang, tambahkan ke `~/.ssh/config`:

```
Host dojo
    HostName dojo.pwn.college
    User hacker
    IdentityFile ~/.ssh/pwncollege
```

Lalu cukup:

```bash
ssh dojo
```

## Tips berguna

**Transfer file** dari/ke dojo:

```bash
# Upload ke dojo
scp -i key exploit.py hacker@dojo.pwn.college:/home/hacker/

# Download dari dojo
scp -i key hacker@dojo.pwn.college:/home/hacker/file.txt .
```

**Edit file jarak jauh dengan VS Code:** pakai ekstensi *Remote - SSH* dan tambahkan host `dojo` dari config di atas.

## Troubleshooting

- **`Permission denied (publickey)`**: public key belum tersimpan di Settings, atau salah file yang ditempel. Pastikan juga `-i` mengarah ke private key yang benar.
- **`Connection closed` / langsung terputus**: biasanya challenge belum di-start. Start dulu dari website.
- **`UNPROTECTED PRIVATE KEY FILE`**: jalankan `chmod 600 key`.
- **Ingin lihat detail error**: tambahkan `-v` (`ssh -v -i key hacker@dojo.pwn.college`).

---

<table width="100%">
<tr>
<td align="left"><a href="06connecting-over-ssh.md">&lt;&lt;&lt; Previous</a></td>

<td align="center"><a href="../README.md">Home</a></td>

<td align="right"><a href="07restarting-challenges.md">Next &gt;&gt;&gt;</a></td>
</tr>
</table>

---

<div align="center">

[@T4n-Labs](https://t4nlabs.web.id/) • [@Gh0sT4n](https://gh0st4n.my.id)

</div>