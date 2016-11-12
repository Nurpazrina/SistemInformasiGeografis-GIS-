**MEMBUAT DATA PADA GEOSPASIAL**

<p align="center">
  <img src ="../../img/Pertemuan 5.jpg" width="400px">
</p>

**Latar Belakang**

Data Geospasial merupakan pengetahuan yang mepelajari tentang titik koordinat dari suatu peta atau juga dapat disebut dengan mempelajari tentang geografis yang ada bumi. Kemarin kita telah mempelajari penambahan class sekarang kita akan membuat data pada geospasial. Didalam geospasial itu sendiri terdapat data geospasial terdapat 2 data pada DBF dan SHP. Untuk menambahkan data itu pun harus berbentuk SHP dan berdasarkan format ESRI = 1. Dalam memasukan data kita dapat memasukannya dalam bentuk polygon, polyline dan poin.

**Pembahasan/Isi**

**Retrieve data geospasial** adalah merupakan suatu cara untuk melakukan select/view, data record dari file dbf dan geometri dari file shp.

**Menambahkan data geospasial**

1.  Import Shapefile

2.  a = shapefie.writer()

***SHP disini adalah file yang berisi geometri***

&gt;&gt;a.point(x,y)

&gt;&gt;a.poly(\[x,y\],\[x,y\])

***DBF disini yaitu file yang berisi table ***

&gt;&gt;a.field(‘namafolder’,’C’,’4’)

&gt;&gt;a.record(‘BDG’)

***Disimpan menggunakan method***

&gt;&gt;a.save(‘file.shp’)

**Menambahkan data berbentuk poin ke dalam SHP dan berdasarkan format ESRI = 1**

&gt;&gt;a.poly(\[a,b\],\[c,d\])

**Memasukan data geospasial berbentuk polygon (kembali ke titik awal) dan polyline tidak (kembali ke titik awal)**

&gt;&gt;a.field(‘kota’,’C’,’40’)

**Membuat attribute table bernama kata dengan tipe data varchar panjang 40 karakter, jika ingin tambah maka panggil kembali method field**

&gt;&gt;a.field(‘Budaya’,’C’,’40’)

&gt;&gt;a.record(‘Bandung’)

**Mengisi table yang hanya 1 field dengan value Bandung. Jika ada dua field maka**

&gt;&gt;a.record(‘Bandung’,’Kota’)

**Menyimpan file shapefile dikomputer**

&gt;&gt;a.save(‘namafile’)

**Param Writer**

-   Shapefile Polygon

-   Shapefile point

-   Shapefile Polyline

*CONTOH:*

**Point:**

&gt;&gt;a.point(‘10’,’12’)

**Polyline:**

&gt;&gt;a.ports(\[3,5\],\[5,5\],\[3,5\],shapetype.shapefile.polyline)

**Polygone:**

&gt;&gt;a.poly(ports = (\[3,5\],\[5,5\],\[5,7\]))

**Kesimpulan:**

Dalam penambahan data geospasial ini kita dapat menambahkan data dengan menambahkan atribut dari param writer yang sudah ada. Dengan memasukan data geospasial dengan berbentuk point, polygon dan polyline.

**Saran:**

Sebaiknya lebih banyak lagi orang yang mempelajari dan menggunakan data-data yang seperti diatas. Dan mempraktekannya, banyak orang yang mengerti tentang menambahkan data geospasial.

Link Github:

Nurpazrina

1144054

D4 Teknik Informatika 3B

Politeknik Pos Indonesia

Link Mata Kuliah:

<http://www.awangga.net/>

Plagiarisme:

By smallseotools :

<https://drive.google.com/open?id=0B_4FZrdBxSUQbUdkZE9Hby1oN00>

By duplichecker :

<https://drive.google.com/open?id=0B_4FZrdBxSUQWjdHQlRlblJaQm8>
