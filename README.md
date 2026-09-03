# backend-nrp

Repo tugas mata kuliah **Pengembangan Backend Dasar**, dibuat dari template [`webdev-if-its/backend-template`](https://github.com/webdev-if-its/backend-template). Ganti judul di atas jadi nama repo kalian sendiri (`backend-nrp`, contoh: `backend-5025201012`).

## Aturan Umum

- Tugas tiap pertemuan disimpan di folder `pertemuan-XX/` pada repo ini.
- Commit message wajib menyebut level yang dicapai: `pertemuan-XX: level N selesai`.
- Deadline push: sebelum pertemuan berikutnya dimulai.
- Semua level dicek otomatis lewat `go test` — baca `pertemuan-XX/SOAL.md` tiap minggu untuk detail levelnya.

## Mengambil Pertemuan Baru Tiap Minggu

Repo ini **tidak otomatis sinkron** dengan template dosen. Begitu ada pertemuan baru, jalankan (ganti `pertemuan-02` sesuai minggu berjalan):

```bash
git fetch https://github.com/webdev-if-its/backend-template.git main
git checkout FETCH_HEAD -- pertemuan-02
```

Perintah ini **aman dijalankan kapan pun** — tidak akan menimpa folder pertemuan lain yang sudah kalian kerjakan, karena hanya mengambil folder yang disebutkan. Setelah itu, commit folder barunya seperti biasa.

Kalau dosen memperbaiki sesuatu di pertemuan yang sudah dirilis (mis. ada bug di test), biasanya cukup ambil ulang file yang diperbaiki saja, bukan seluruh folder — akan diumumkan file mana yang berubah.

---

Bagian di bawah ini **isi bertahap** sesuai level yang sedang kalian kerjakan (lihat `pertemuan-01/SOAL.md`) — heading-nya dicek otomatis, jangan diganti namanya.

## Identitas
- Nama: Fathiya Haya Shafa Kamila Setiadi
- NRP: 5053241047
- Kelas: Pengembangan Backend Dasar (M)

## Commit vs Push
Git commit adalah ketika pengerjaan kode terbaru ditandai perubahannya dan tersimpan di repository lokal, lalu git push adalah proses penyimpanan atau penetapan kode terbaru tersebut di repositori jaringan git. Jika seseorang melakukan commit tanpa melakukan push, maka pembaruan kode tidak akan tersimpan dan tidak dapat diakses atau dilihat oleh tim secara online.

## Reproducibility
Reproducibility adalah ketika suatu kode atau program dipastikan dapat berjalan dengan lancar dan menghasilkan output yang sama di semua environment.

Jika pada pengerjaan suatu project, terdapat perbedaan versi bahasa, misalnya dalam Go, di antara anggota tim, hal ini mungkin saja memunculkan suatu hambatan dalam tercapainya reproducibility. Hambatan tersebut bisa muncul ketika kode project mulai menggunakan fitur atau library yang dirilis di versi terbarunya. Anggota tim yang menggunakan versi Go yang lebih lama tentu akan kesulitan untuk mendapatkan output yang sama dari kode tersebut.

Namun, perbedaan versi ini juga masih bisa dimaklumi jika pengerjaan project menggunakan fitur atau package dasar yang tersedia di setiap versi Go tersebut. Karena dengan begitu, output yang dihasilkan akan selalu sama dan reproducibility tetap tercapai.

## Catatan Merge Conflict
Conflict terjadi di baris kode yang mengimplementasikan fungsi CetakInfo. Hal ini karena ketika branch fitur-sapaan dibuat dan file main.go diperbarui pada bagian CetakInfo-nya, fungsi yang sama juga diperbarui di main branch sehingga kini ada dua versi fungsi yang berbeda. Untuk menyelesaikan conflict ini, saya membersihkan versi CetakInfo yang ada di main branch sehingga versi yang ada di branch fitur-sapaan dapat digunakan. Alasan dipilihnya versi CetakInfo di branch fitur-sapaan adalah karena versi ini sudah memenuhi arahan pemanggilan fungsi Sapa sambil tetap mempertahankan hasil Nama, NRP, dan versi Go yang digunakan.

## Kenapa .gitignore Penting
(tulis di sini)

## Refleksi
(tulis di sini)
