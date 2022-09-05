# flutter_plugin_pubdev

A new Flutter project.

# Tugas Praktikum

## 1. Selesaikan Praktikum tersebut, lalu dokumentasikan dan push ke repository Anda berupa screenshot hasil pekerjaan beserta penjelasannya di file README.md!
![plot](images/1.png)
- Pada praktikum ini menambahkan plugin auto_size_text dan menerapkannya, yang hasil output project tersebut terdapat perbedaan diantara teks yang dibaris pertama dan baris kedua pernedaanya terdapat pada ukuran font dan warna background.
## 2. Jelaskan maksud dari langkah 2 pada praktikum tersebut!
- Langkah 2 yaitu Proses Menambahkan Plugin auto_size_text dalam project praktikum, yaitu dengan cara  menggunakan perintah "flutter pub add auto_size_text". Jika plugin berhasil ditambahaknan maka pada file pubspec.yaml bagian dependencies akan muncul nama dan versi dari plugin. Pada projek ini menggunakan versi 3.0.0

### 3. Jelaskan maksud dari langkah 5 pada praktikum tersebut!
- Langkah 5 yaitu Membuat Variabel text dan parameter di constructor
```
final String text;
const RedTextWidget({Key? key, required this.text}) : super(key: key);
```
menambahkan inisialisasi variable dengan nama "text" pada konstruktor agar dapat memanggil variabel tersebut pada file main.dart untuk menampilkan sesuai pangilan dari class RedTextWidget yang didalamnya terdapat return AutoSizeText.

### 4. Pada langkah 6 terdapat dua widget yang ditambahkan, jelaskan fungsi dan perbedaannya!
- Langkah 6 yaitu Tambahkan widget di main.dart
Menambahkan dua widget ini pada file main.dart
```
Container(
   color: Colors.yellowAccent,
   width: 50,
   child: const RedTextWidget(
	text: 'You have pushed the button this many times:',
	),
),
Container(
    color: Colors.greenAccent,
    width: 100,
    child: const Text(
	'You have pushed the button this many times:',
	),
),
```
#### Kedua widget tersebut yang ditambahkan adalah widget Container. 
- Pada container pertama child diisi dengan widget class RedTextWidget untuk menerapkan penggunaan dari  Plugin AutoSizeText. 
- Pada container kedua child diisi dengan widget text biasa yang tanpa mengunakan Plugin untuk melihat perbedaan dari hasil tampilan antara widget text biasa dan widget class RedTextWidget. Perbedaanya jika menggunakan Plugin maka terlihat lebih rapi dan teratur dan jika tanpa pugin maka text yang di tampilkan kurang teratur.

# 5. Jelaskan maksud dari tiap parameter yang ada di dalam plugin auto_size_text berdasarkan tautan pada dokumentasi ini ! 
