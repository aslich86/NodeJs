# Tutorial Pengenalan ke Node.js dan NPM

## Apa itu Node.js?
Node.js adalah platform runtime yang dibangun di atas mesin JavaScript V8 milik Google Chrome. Ini memungkinkan kita menjalankan kode JavaScript di sisi server, bukan hanya di browser. Node.js membawa lingkungan eksekusi JavaScript ke luar browser dan memungkinkan kita untuk membangun aplikasi server-side, aplikasi berbasis baris perintah, alat utilitas, dan banyak lagi.

## Keuntungan Menggunakan Node.js:
1. **Kinerja Tinggi**: Dibangun di atas V8, Node.js menghadirkan kinerja yang sangat cepat.

2. **Asynchronous I/O**: Node.js beroperasi dengan model asinkron, memungkinkan menangani banyak koneksi tanpa memblokir proses lainnya.

3. **Kode yang Sama**: Dengan Node.js, Anda dapat menggunakan JavaScript di seluruh aplikasi, baik di sisi klien (browser) maupun server.

4. **Komunitas Besar**: Node.js memiliki komunitas yang besar dan aktif, yang berarti banyak dukungan, modul, dan sumber daya yang tersedia.

## Cara Memulai dengan Node.js dan NPM:

### 1. Instalasi Node.js:
Pertama-tama, Anda perlu menginstal Node.js di sistem Anda. Kunjungi situs resmi Node.js (https://nodejs.org) dan unduh installer yang sesuai dengan sistem operasi Anda. Ikuti panduan instalasi yang disediakan.

### 2. Cek Instalasi:
Setelah selesai menginstal Node.js, Anda dapat memeriksa versi Node.js yang terinstal dengan menjalankan perintah berikut di terminal atau command prompt:

```
node -v
```

Juga, pastikan NPM (Node Package Manager) terinstal dengan perintah:

```
npm -v
```

### 3. Inisialisasi Proyek Node.js:
Untuk memulai proyek baru, buat direktori baru dan masuk ke dalamnya menggunakan terminal atau command prompt. Lalu, jalankan perintah berikut untuk menginisialisasi proyek Node.js baru:

```
npm init
```

Ikuti instruksi untuk mengisi informasi proyek seperti nama, deskripsi, versi, dan lainnya. Jika Anda ingin mengabaikan pertanyaan tertentu, cukup tekan "Enter" untuk meneruskan.

### 4. Penggunaan Modul NPM:
Node.js memiliki ekosistem modul yang besar, yang dikelola oleh NPM. Modul adalah paket atau pustaka JavaScript yang bisa Anda gunakan dalam proyek Anda. Anda dapat mencari modul yang ingin Anda gunakan di situs web NPM (https://www.npmjs.com).

Misalnya, untuk menginstal modul "express", jalankan perintah berikut:

```
npm install express
```

Setelah itu, Anda dapat menggunakannya dalam kode JavaScript Anda dengan menambahkan baris berikut:

```javascript
const express = require('express');
```

### 5. Membuat Aplikasi Node.js Sederhana:
Berikut adalah contoh kode sederhana untuk aplikasi server HTTP menggunakan Node.js dan modul Express:

```javascript
const express = require('express');
const app = express();
const port = 3000;

app.get('/', (req, res) => {
    res.send('Hello, world!');
});

app.listen(port, () => {
    console.log(`Server berjalan di http://localhost:${port}`);
});
```

Simpan kode di atas dalam file dengan ekstensi `.js` (misalnya `app.js`). Kemudian, jalankan aplikasi dengan perintah:

```
node app.js
```

Aplikasi server Anda akan berjalan di http://localhost:3000, dan setiap kali Anda mengaksesnya, Anda akan melihat pesan "Hello, world!".


