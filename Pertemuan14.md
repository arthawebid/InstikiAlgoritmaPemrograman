Berikut adalah materi perkuliahan tentang **Deklarasi Prosedur, Prosedur Tanpa Parameter, Prosedur dengan Parameter**, serta **Pemanggilan Prosedur** dalam **Algoritma Pemrograman**.

### 1. **Deklarasi Prosedur**
Prosedur adalah sekumpulan pernyataan atau blok kode yang dirancang untuk melakukan tugas tertentu. Prosedur biasanya digunakan untuk memecah masalah besar menjadi bagian-bagian yang lebih kecil. Deklarasi prosedur dilakukan dengan menentukan nama prosedur, jenis prosedur (apakah menerima parameter atau tidak), dan kode yang akan dijalankan ketika prosedur tersebut dipanggil.

#### Bentuk Umum Deklarasi Prosedur:
```pascal
procedure nama_prosedur;
begin
   // Instruksi yang akan dijalankan
end;
```
Contoh:
```pascal
procedure cetakHalo;
begin
   writeln('Halo, selamat datang di Algoritma Pemrograman!');
end;
```
Pada contoh di atas, prosedur `cetakHalo` tidak menerima parameter dan hanya mencetak pesan ke layar.

---

### 2. **Prosedur Tanpa Parameter**
Prosedur tanpa parameter adalah prosedur yang tidak memerlukan input dari pemanggilnya. Prosedur ini hanya berfungsi untuk menjalankan serangkaian pernyataan yang ada di dalam tubuh prosedur tersebut.

#### Contoh Prosedur Tanpa Parameter:
```pascal
procedure tampilkanPesan;
begin
   writeln('Selamat belajar algoritma!');
end;
```
Pada contoh di atas, prosedur `tampilkanPesan` tidak menerima parameter dan hanya menjalankan perintah untuk mencetak pesan.

---

### 3. **Prosedur dengan Parameter**
Prosedur dengan parameter memungkinkan nilai untuk diteruskan ke prosedur. Parameter adalah variabel yang digunakan untuk menerima nilai yang diberikan oleh pemanggil prosedur. Parameter ini bisa berupa **value parameter** atau **variable parameter**.

---

#### a. **Value Parameter (Passing by Value)**
Pada metode *passing by value*, nilai yang diteruskan ke prosedur adalah salinan dari nilai asli. Artinya, perubahan yang dilakukan pada parameter di dalam prosedur tidak akan mempengaruhi nilai asli dari variabel yang dipassingkan.

**Sintaks:**
```pascal
procedure nama_prosedur(parameter_tipe: tipe_data);
begin
   // Instruksi yang menggunakan parameter
end;
```

Contoh:
```pascal
procedure hitungKuadrat(x: integer);
begin
   writeln('Kuadrat dari ', x, ' adalah ', x * x);
end;
```

Pemanggilan:
```pascal
var
  angka: integer;
begin
  angka := 5;
  hitungKuadrat(angka);
end.
```
Pada contoh di atas, meskipun nilai `angka` adalah 5, nilai tersebut diteruskan ke prosedur sebagai salinan, dan prosedur menghitung kuadrat dari nilai tersebut.

---

#### b. **Variable Parameter (Passing by Reference)**
Pada metode *passing by reference*, yang diteruskan ke prosedur adalah alamat memori variabel tersebut. Dengan demikian, perubahan yang dilakukan pada parameter di dalam prosedur akan mempengaruhi nilai variabel yang ada di luar prosedur.

**Sintaks:**
```pascal
procedure nama_prosedur(var parameter_tipe: tipe_data);
begin
   // Instruksi yang menggunakan parameter
end;
```

Contoh:
```pascal
procedure ubahNilai(var x: integer);
begin
   x := x * 2;
end;
```

Pemanggilan:
```pascal
var
  angka: integer;
begin
  angka := 5;
  ubahNilai(angka);
  writeln('Nilai angka setelah diubah: ', angka);  // Akan mencetak 10
end.
```

Pada contoh di atas, variabel `angka` diubah dalam prosedur karena parameter `x` dipassing dengan referensi (`var`). Setelah prosedur selesai, nilai dari `angka` menjadi 10.

---

### 4. **Pemanggilan Prosedur**
Prosedur dipanggil ketika ingin menjalankan blok kode yang ada di dalamnya. Pemanggilan prosedur dilakukan dengan menyebutkan nama prosedur tersebut.

#### Contoh Pemanggilan Prosedur:
```pascal
var
  angka: integer;
begin
  angka := 5;
  hitungKuadrat(angka);  // Memanggil prosedur hitungKuadrat
end.
```

Pada contoh di atas, prosedur `hitungKuadrat` dipanggil dan diberikan parameter `angka`. Nilai parameter akan diproses oleh prosedur sesuai dengan yang sudah didefinisikan.

---

### 5. **Contoh Program dengan Semua Konsep:**

```pascal
program ProsedurExample;
uses crt;

procedure tampilkanPesan;
begin
   writeln('Selamat datang!');
end;

procedure hitungKuadrat(x: integer);
begin
   writeln('Kuadrat dari ', x, ' adalah ', x * x);
end;

procedure ubahNilai(var x: integer);
begin
   x := x * 2;
end;

var
  angka: integer;
begin
  clrscr;
  
  // Pemanggilan prosedur tanpa parameter
  tampilkanPesan;
  
  // Pemanggilan prosedur dengan parameter passing by value
  angka := 4;
  hitungKuadrat(angka);
  
  // Pemanggilan prosedur dengan parameter passing by reference
  angka := 5;
  ubahNilai(angka);
  writeln('Nilai angka setelah diubah: ', angka);  // Akan mencetak 10

  readln;
end.
```

#### Penjelasan:
1. **tampilkanPesan** adalah prosedur tanpa parameter, yang hanya mencetak pesan.
2. **hitungKuadrat** adalah prosedur dengan parameter passing by value, yang menghitung kuadrat dari nilai yang diteruskan.
3. **ubahNilai** adalah prosedur dengan parameter passing by reference, yang mengubah nilai variabel yang dipassingkan.

---

### Kesimpulan
1. **Deklarasi Prosedur**: Memiliki struktur dasar yang menyebutkan nama prosedur dan kode yang dijalankan.
2. **Prosedur Tanpa Parameter**: Tidak memerlukan input dari pemanggilnya.
3. **Prosedur dengan Parameter**:
   - **Passing by Value**: Mengirimkan salinan nilai variabel, perubahan pada parameter tidak mempengaruhi nilai asli.
   - **Passing by Reference**: Mengirimkan alamat memori variabel, sehingga perubahan pada parameter mempengaruhi nilai asli.
4. **Pemanggilan Prosedur**: Prosedur dipanggil dengan menyebutkan namanya, dan bisa disertai dengan parameter.

Dengan memahami konsep ini, mahasiswa dapat menulis kode yang lebih modular dan terstruktur dengan menggunakan prosedur dalam pemrograman.

---
[Pertemuan1](Pertemuan1.md) | [Pertemuan2](Pertemuan2.md) | [Pertemuan3](Pertemuan3.md) | [Pertemuan4](Pertemuan4.md) | [Pertemuan5](Pertemuan5.md) | [Pertemuan6](Pertemuan6.md) | [Pertemuan7](Pertemuan7.md) | [Pertemuan8](Pertemuan8.md) | [Pertemuan9](Pertemuan9.md) | [Pertemuan10](Pertemuan10.md) | [Pertemuan11](Pertemuan11.md) | [Pertemuan12](Pertemuan12.md) | [Pertemuan13](Pertemuan13.md) | [Pertemuan14](Pertemuan14.md) | [Pertemuan15](Pertemuan15.md) | [Pertemuan16](Pertemuan16.md)