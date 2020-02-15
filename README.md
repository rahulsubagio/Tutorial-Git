## Tutorial upload project dengan `Git` ke `Github`

### -> Buat repository baru di akun github kalian

### -> Klik `Clone or Download` yang berwarna hijau

### -> Copy URL yang tersedia disitu**

### -> Arahkan pada direktori project yang akan di upload ke repository `Github`

#### Untuk pengguna `Linux`
Buka terminal lalu arahkan folder direktori project kalian

#### Untuk pengguna `Windows`
Sebelumnya pastikan bahwa kalian telah menginstal [`Git Bash`](https://git-scm.com/downloads), klik kanan folder project dan pilih `Git Bash Here` maka akan muncul command promt / CMD

### -> Konfigurasi username dan email di terminal atau cmd yang telah terarahkan ke folder project kalian

*Ini di khususkan untuk yang baru pertama kali menggunakan `git` di laptop/komputer atau untuk mengubah tujuan akun `github`*

```
git config --global user.name "username anda"
```

```
git config --global user.email "email anda"
```

### -> Lakukan inisialisai direktori lokal (folder project) sebagai `git repository`

```
git init
```

### -> Tambahkan semua file/folder yang ada dalam folder project kalian

```
git add *
```

### -> Buat `commit` project nya

```
git commit -m "<isi pesan terserah kalian>"
```

### -> Jadikan `remote` repository yang telah dibuat di akun github kalian

```
git remote add <paste kan link url yang kalian copy tadi>
```

#### Contoh

```
git remote add https://github.com/rahulsubagio/test.git
```

### -> `pull` project nya

```
git pull origin master
```

### -> `push` (upload) project nya

```
git push origin master
```

*Nanti akan muncul `pop up` lalu masukkan username/email dan password akun `github` kalian. Lalu tunggu hingga selesai, kemudian refresh halaman repository `github` kalian*

### Jika terjadi `error` ketika `push`

* **Pesan `error`**

```
! [rejected]        master -> master (non-fast-forward)
```

**Solusinya**

```
git push -f origin master
```

* **Pesan `error`**

```
! [rejected]        master -> master (fetch first)
```

**Solusinya**

```
git fetch origin master
```

Selamat mencoba :D ..
