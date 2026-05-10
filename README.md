# Tutorial TypeScript untuk Penyelesaian Tugas Berbasis NIM

## 1. Pendahuluan

Tutorial ini membantu mahasiswa mempelajari dasar penggunaan **TypeScript** untuk menyelesaikan beberapa permasalahan algoritmik sederhana berbasis NIM.

TypeScript merupakan pengembangan dari JavaScript yang menambahkan fitur **static typing** sehingga kode menjadi lebih aman, mudah dibaca, dan lebih mudah dikembangkan untuk project skala besar.

Pada tutorial ini mahasiswa akan mempelajari:

- Instalasi Node.js dan TypeScript
- Menjalankan program TypeScript
- Struktur dasar program TypeScript
- Variabel dan tipe data
- Percabangan
- Perulangan
- Function
- Array
- Implementasi algoritma sederhana

---

# 2. Instalasi dan Persiapan Lingkungan

## 2.1 Install Node.js

TypeScript berjalan menggunakan runtime JavaScript yaitu **Node.js**.

Download Node.js:

https://nodejs.org/

Gunakan versi **LTS (Long Term Support)**.

### Windows

1. Download installer `.msi`
2. Klik Next sampai selesai
3. Pastikan opsi:
   - `Add to PATH`
   - `Install npm`

dalam keadaan aktif.

### Linux (Ubuntu/Debian)

```bash
sudo apt update
sudo apt install nodejs npm
```

### macOS

```bash
brew install node
```

---

# 2.2 Verifikasi Instalasi

Cek versi Node.js:

```bash
node -v
```

Cek npm:

```bash
npm -v
```

---

# 2.3 Install Visual Studio Code

Download:

https://code.visualstudio.com/

---

# 2.4 Install TypeScript Secara Global

```bash
npm install -g typescript
```

---

# 2.5 Verifikasi TypeScript

```bash
tsc -v
```

---

# 2.6 Membuat Folder Project

```bash
mkdir tugas-typescript
cd tugas-typescript
code .
```

---

# 2.7 Inisialisasi Project

```bash
npm init -y
```

---

# 2.8 Membuat Konfigurasi TypeScript

```bash
tsc --init
```

---

# 2.9 Membuat Program Pertama

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

---

# 2.10 Install ts-node

```bash
npm install -g ts-node
```

Jalankan langsung:

```bash
ts-node main.ts
```

---

# 3. Dasar TypeScript

## Variabel

```ts
let nama: string = "Budi";
let umur: number = 20;
let aktif: boolean = true;
```

## Array

```ts
let angka: number[] = [1, 2, 3];
```

## Function

```ts
function tambah(a: number, b: number): number {
  return a + b;
}
```

## Percabangan

```ts
if (umur >= 18) {
  console.log("Dewasa");
}
```

## Perulangan

```ts
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

---

# 4. Soal 1 — Pola Segitiga dari NIM

## Contoh

NIM:

```txt
230411013
```

Output:

```txt
1
1 2
1 2 3
```

## Program

```ts
const nim: string = "230411013";

let tinggi: number = Number(nim[nim.length - 1]);

if (tinggi === 0) {
  tinggi = 10;
}

for (let i = 1; i <= tinggi; i++) {
  let baris: string = "";

  for (let j = 1; j <= i; j++) {
    baris += j + " ";
  }

  console.log(baris);
}
```

---

# 5. Soal 2 — Deret Aritmatika dari NIM

## Contoh

NIM:

```txt
230411013
```

- Start = 13
- Step = 1

Output:

```txt
13, 14, 15, 16, 17, 18, 19, 20, 21, 22
```

## Program

```ts
const nim: string = "230411013";

const start: number = Number(nim.slice(-2));

const step: number =
  Number(nim[nim.length - 3]) + 1;

let hasil: number[] = [];

for (let i = 0; i < 10; i++) {
  hasil.push(start + i * step);
}

console.log(hasil);
```

---

# 6. Soal 3 — Bilangan Prima dari NIM

## Contoh

NIM:

```txt
230411013
```

Batas:

```txt
23
```

Output:

```txt
2, 3, 5, 7, 11, 13, 17, 19, 23
```

## Program

```ts
const nim: string = "230411013";

const batas: number =
  Number(nim.slice(-2)) + 10;

let prima: number[] = [];

for (let angka = 2; angka <= batas; angka++) {
  if (isPrima(angka)) {
    prima.push(angka);
  }
}

console.log(prima);

function isPrima(n: number): boolean {
  if (n < 2) {
    return false;
  }

  for (let i = 2; i <= Math.sqrt(n); i++) {
    if (n % i === 0) {
      return false;
    }
  }

  return true;
}
```

---

# 7. Cara Menjalankan Program

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

# 8. Format Pengumpulan

```txt
Nama:
NIM:
Kelas:
Link GitHub:
Screenshot hasil program:
```

---

# 9. Kriteria Penilaian

| Aspek | Bobot |
|---|---:|
| Program berjalan | 30 |
| Soal 1 benar | 20 |
| Soal 2 benar | 20 |
| Soal 3 benar | 20 |
| Dokumentasi GitHub | 10 |
| Total | 100 |

---

# 10. Referensi

- https://www.typescriptlang.org/docs/
- https://nodejs.org/en/docs
- https://code.visualstudio.com/docs
