# Mengapa TypeScript Digunakan pada Mata Kuliah Pemrograman Perangkat Bergerak?

## 1. Pendahuluan

Tutorial ini menjelaskan dasar TypeScript dan alasan penggunaannya dalam mata kuliah Pemrograman Perangkat Bergerak.

TypeScript adalah pengembangan dari JavaScript yang menambahkan fitur static typing sehingga kode lebih aman, terstruktur, dan mudah dikembangkan.

---

# 2. Mengapa Menggunakan TypeScript?

## 2.1 Mengurangi Error

TypeScript dapat mendeteksi kesalahan sebelum program dijalankan.

Contoh:

```ts
let umur: number = "20";
```

Kode di atas langsung menghasilkan error karena string dimasukkan ke number.

---

## 2.2 Mendukung Pengembangan Mobile Modern

Framework modern seperti:

- Ionic
- Angular
- Vue
- React Native

mendukung atau menggunakan TypeScript.

---

## 2.3 Digunakan di Industri

Banyak perusahaan menggunakan TypeScript karena:

- lebih aman
- lebih mudah maintenance
- cocok untuk project besar
- mendukung kolaborasi tim

---

# 3. Hubungan JavaScript dan TypeScript

TypeScript adalah superset dari JavaScript.

Semua kode JavaScript valid di TypeScript.

## JavaScript

```js
function tambah(a, b) {
  return a + b;
}
```

## TypeScript

```ts
function tambah(a: number, b: number): number {
  return a + b;
}
```

---

# 4. Instalasi

## 4.1 Install Node.js

Download:

https://nodejs.org/

Gunakan versi LTS.

Cek instalasi:

```bash
node -v
npm -v
```

---

## 4.2 Install Visual Studio Code

Download:

https://code.visualstudio.com/

---

## 4.3 Install TypeScript

```bash
npm install -g typescript
```

Cek versi:

```bash
tsc -v
```

---

## 4.4 Install ts-node

```bash
npm install -g ts-node
```

---

# 5. Membuat Project

## Membuat Folder

```bash
mkdir tugas-typescript
cd tugas-typescript
```

## Inisialisasi Project

```bash
npm init -y
```

## Membuat Konfigurasi TypeScript

```bash
tsc --init
```

---

# 6. Program Pertama

Buat file:

```txt
main.ts
```

Isi:

```ts
console.log("Hello TypeScript");
```

Compile:

```bash
tsc main.ts
```

Jalankan:

```bash
node main.js
```

Atau langsung:

```bash
ts-node main.ts
```

---

# 7. Dasar TypeScript

# 7.1 Variabel

```ts
let nama: string = "Budi";
let umur: number = 20;
let aktif: boolean = true;
```

---

# 7.2 Array

```ts
let angka: number[] = [1, 2, 3];
```

---

# 7.3 Function

```ts
function tambah(a: number, b: number): number {
  return a + b;
}
```

---

# 7.4 Percabangan

```ts
let nilai: number = 80;

if (nilai >= 75) {
  console.log("Lulus");
} else {
  console.log("Tidak Lulus");
}
```

---

# 7.5 Perulangan

```ts
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

---

# 7.6 Object

```ts
let mahasiswa = {
  nama: "Budi",
  nim: "230411013",
  umur: 20
};
```

---

# 7.7 Interface

```ts
interface Mahasiswa {
  nama: string;
  nim: string;
  umur: number;
}
```

---

# 7.8 Class

```ts
class Mobil {
  merk: string;

  constructor(merk: string) {
    this.merk = merk;
  }

  jalan(): void {
    console.log(this.merk + " berjalan");
  }
}
```

---

# 7.9 Async Await

```ts
async function ambilData() {
  return "Data berhasil";
}

async function proses() {
  const hasil = await ambilData();
  console.log(hasil);
}
```

---

# 8. Kaitan dengan Pemrograman Perangkat Bergerak

Konsep-konsep TypeScript akan digunakan dalam:

- UI Component
- Navigation
- API
- State Management
- Authentication
- Database
- Mobile Event Handling

Karena itu pemahaman dasar TypeScript sangat penting sebelum mempelajari Ionic atau framework mobile lainnya.

---

# 9. Roadmap Pembelajaran

```txt
Dasar Pemrograman
        ↓
JavaScript
        ↓
TypeScript
        ↓
Vue / React
        ↓
Ionic
        ↓
Mobile Development
```

---

# 10. Referensi

- https://www.typescriptlang.org/docs/
- https://nodejs.org/en/docs
- https://code.visualstudio.com/docs
