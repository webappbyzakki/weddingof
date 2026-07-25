# Undangan Zakki & Niha di GitHub Pages

Paket ini berisi:

- `index.html`: halaman undangan utama.
- `generator.html`: generator permalink nama tamu.
- `.nojekyll`: mencegah pemrosesan Jekyll yang tidak diperlukan.

## 1. Unggah ke GitHub

1. Buat repository baru, misalnya `undangan-zakki-niha`.
2. Pilih repository **Public** bila memakai GitHub Free.
3. Unggah `index.html`, `generator.html`, dan `.nojekyll` ke root repository.
4. Commit ke branch `main`.

## 2. Aktifkan GitHub Pages

1. Buka **Settings** repository.
2. Pilih **Pages**.
3. Pada **Build and deployment**, pilih **Deploy from a branch**.
4. Pilih branch `main` dan folder `/(root)`.
5. Klik **Save**.

Alamatnya biasanya:

```text
https://USERNAME.github.io/undangan-zakki-niha/
```

## 3. Membuat permalink tamu

Buka:

```text
https://USERNAME.github.io/undangan-zakki-niha/generator.html
```

Masukkan nama tamu. Generator menghasilkan link seperti:

```text
https://USERNAME.github.io/undangan-zakki-niha/?to=Bapak+Ahmad+dan+Keluarga
```

Nama akan otomatis:

- tampil pada cover;
- menjadi judul tab browser;
- masuk ke kolom Nama pada RSVP;
- kembali terisi setelah RSVP dikirim.

Parameter yang didukung:

```text
?to=Nama Tamu
?nama=Nama Tamu
?guest=Nama Tamu
```

Gunakan `?to=` sebagai standar.

## 4. Contoh

```text
https://USERNAME.github.io/undangan-zakki-niha/?to=Ibu%20Siti%20dan%20Keluarga
```

Tidak perlu membuat file HTML berbeda untuk setiap tamu.

## 5. Memperbarui undangan

Edit atau unggah ulang `index.html`, lalu commit ke branch `main`. GitHub Pages akan menerbitkan versi terbaru dari sumber yang dikonfigurasi.

## Catatan

Nama tamu diperbarui oleh JavaScript setelah halaman dibuka. Preview WhatsApp atau media sosial tetap memakai judul undangan umum karena crawler preview biasanya tidak menjalankan JavaScript query parameter.
