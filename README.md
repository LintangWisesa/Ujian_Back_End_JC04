# Soal Ujian Purwadhika Back-End Development

![Lintang_Purwadhika](https://static.wixstatic.com/media/2e6af2_f69a4271c3534ae1869a7ed63e278b2b~mv2.png/v1/fill/w_246,h_39,al_c,usm_0.66_1.00_0.01/2e6af2_f69a4271c3534ae1869a7ed63e278b2b~mv2.png)

**Materi Back End Web Dev dapat diakses di [klik sini!](https://github.com/LintangWisesa/Purwadhika-JC04-03_BackEndWeb)**

### **Soal 1 - MySQL Database**

Buatlah database design dengan kasus berikut.

Vincent adalah seorang bos besar sebuah perusahaan di bidang kuliner. Dia ingin membuat aplikasi dengan spesifikasi:
- Restoran terdapat beberapa cabang di berbagai tempat.
- Masing-masing cabang restoran memiliki menu makanan dan minuman dengan harga yang berbeda-beda.
- Menu makanan memiliki kategori dengan level urutan sebagai berikut:
  - Food/Beverage
  - Food: Appetizer, Main Course, Dessert
  - Beverage: Juice, Tea, Coffee, Mineral
  - Menu makanan dari setiap kategori level 2.
- Sistem dapat melihat sisa stock yang tersisa. stock akan berkurang setiap bahan digunakan dan akan bertambah setiap pembelian bahan. setiap bahan memiliki satuan nya masing-masing, misal: stock beras 5 (karung) & stock kecap 5 (botol).
- Sistem dapat mencatat setiap pengurangan stock (bahan apa, oleh karyawan siapa & waktunya kapan), dan mencatat setiap penambahan stock (bahan apa & oleh vendor apa). Vendor tidak perlu dibuat master vendor-nya.
- Setiap tamu yang akan melakukan pembayaran maka akan dibuatkan sebuah invoice yang mencatat setiap transaksi dan terdapat: kode invoice, waktu invoice, total harga, kasir yang bersangkutan, list makanan dan minuman.
- Setiap cabang restoran memiliki data karyawan masing-masing. Karyawan juga memiliki data berupa nama, gender, role kerja (kasir, cheff, pelayan, CS, dll), gaji.

**_Catatan:_** _Export database sebagai jawaban soal ini!_

### **Soal 2 - Express & MySQL**

Buatlah Function CRUD (Create/Insert, Read/Select, Update, Delete) dari database yang sudah dibuat (**Soal No. 1**) dengan menggunakan Foreign Key dari tabel yang berhubungan:
- Cabang Restoran.
- Menu makanan/minuman dengan kategori level 1, 2, 3 pada setiap cabang.
- Penambahan/pengurangan stock berdasarkan spesifikasi di atas (tidak dapat dihapus dan diedit).
- Memasukan Data Karyawan.

_**Catatan:**_ _Ketik kode javascript yang Anda buat, dalam format .txt sebagai jawaban soal ini!_

### **Soal 3 - MongoDB**

Tuliskan langkah-langkah/urutan query MongoDB untuk membuat sebuah database Non-RDBMS (Document Store) dengan spesifikasi sebagai berikut:
- Terdapat sebuah database dengan nama __"Kampus"__.
- Database __"Kampus"__ memiliki 2 buah user:
  - User pertama adalah admin database bernama __"andi"__, dengan password __"anditopsecret"__. 
  - User kedua bukanlah admin, namun tetap dapat memasukkan & membaca data dari database. User kedua bernama __"budi"__, dengan password __"buditopsecret"__.
- Database __"Kampus"__ memiliki 2 buah collection: __"Dosen"__ dan __"Mahasiswa"__.
- Masukkan 3 buah data berikut ke collection __"Dosen"__:

```javascript
    {nama:"Caca",
    usia:28,
    asal:"Jakarta",
    bidang:"Fisika Astrologi",
    titel:"S2",
    status:"Honorer",
    nip:123,
    matkul:["Metrologi","Kosmologi","Kalkulus"]}

    {nama:"Dedi",
    usia:29,
    asal:"Yogyakarta",
    bidang:"Fisika Terapan",
    titel:"S3",
    status:"PNS",
    nip:456,
    matkul:["Instrumentasi","Elektronika","Fisika Dasar"]}

    {nama:"Euis",
    usia:30,
    asal:"Bandung",
    bidang:"Fisika Teoretik",
    titel:"S1",
    status:"Honorer",
    nip:789,
    matkul:["Fisika Dasar","Fisika Modern","Kalkulus"]}
```

- Masukkan 3 buah data berikut ke collection __"Mahasiswa"__:

```javascript
    {nama:"Faza",
    usia:19,
    asal:"Aceh",
    prodi:"Fisika",
    angkatan:2017,
    nim:123}

    {nama:"Gilang",
    usia:20,
    asal:"Semarang",
    prodi:"Fisika",
    angkatan:2017,
    nim:456}

    {nama:"Hanafi",
    usia:19,
    asal:"Makassar",
    prodi:"Fisika",
    angkatan:2017,
    nim:789}
```

_**Catatan:**_ _Soal ini hanya meminta Anda untuk menuliskan langkah-langkah/urutan query MongoDB, sesuai spesifikasi di atas. Ketik jawaban dalam sebuah file .txt!_

### **Soal 4 - Express & MongoDB**

Buatlah sebuah aplikasi NodeJS (Express) sederhana yang mampu mengakses database __"Kampus"__ (**Soal No. 3**), dengan spesifikasi sebagai berikut:

- __GET /dosen__ &rarr; akan memberikan response: menampilkan semua data pada collection __"Dosen"__.

- **GET /mahasiswa** &rarr; akan memberikan response: menampilkan semua data pada collection **"Mahasiswa"**.

- __GET /dnama/:namadosen__ &rarr; akan memberikan response: menampilkan data pada collection __"Dosen"__ yang memiliki nama=namadosen. 
  > Misal __GET /dnama/Caca__ akan menampilkan semua data milik dosen __Caca__. 

- **GET /mnama/:namamahasiswa** &rarr; akan memberikan response: menampilkan data pada collection **"Mahasiswa"** yang memiliki nama=namamahasiswa. 
  > Misal **GET /mnama/Faza** akan menampilkan semua data milik mahasiswa **Faza**.

_**Catatan:**_ _Ketik kode javascript yang Anda buat, dalam format .txt sebagai jawaban soal ini!_

### *__#HappyCoding__*
