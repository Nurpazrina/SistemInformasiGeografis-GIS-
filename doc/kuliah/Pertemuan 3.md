Retrieve Pada Data Geospasial dan membuat Class pada Pyton

<p align="center">
  <img src ="../../img/Pertemuan 3.jpg" width="400px">
</p>

**Latar Belakang**

Data Geospasial merupakan pengetahuan yang mepelajari tentang titik koordinat dari suatu peta atau juga dapat disebut dengan mempelajari tentang geografis yang ada bumi. Didalam geospasial itu sendiri ada untuk manipulasi data dan menghitung record pada file .shp, dan shp itu terdapat dalam shapefile dan didalam shapefile itu tidak hanya terdapat file shp namun ada juga file dbf. Untuk membaca shapefile kita dapat menggunakan python kita dapat memanggil langsung file shp nya atau juga bisa membuat class terlebih dahulu.

&lt;Video&gt;

**Pembahasan/Isi**

**Retrieve data geospasial** adalah merupakan suatu cara untuk melakukan select/view, data record dari file dbf dan geometri dari file shp.

**SHP** adalah salah satu file yang berada didalam shapefile yang menyimpan data geometri.

Didalam file shp terdapat beberapa data seperti:

1.  Bbox adalah sebuah boundary box (koordinat 4 titik) atau koordinat batas view yang ada pada peta.

2.  Point adalah titik suatu koordinat

3.  Shapetype adalah jenis data geometri yang mempunyai standar nomor yang ditetapkan oleh ESRI seperti nomor 1 untuk poin, 2 untuk polygon, 3 untuk polyline, dll.

    Contoh ada pada link: shapefile.esri

**DBF** adalah sebuah file yang menyimpan file tabular yang menyimpan data attribut.

Membaca Jumlah data geometri dengan python:

-   Membaca data shp

    &gt;&gt; import shapefile

    &gt;&gt; sf = shapefile.Reader(“namafile.shp”)

    &gt;&gt; sf.shapes()

    &gt;&gt; a = sf.shapes()

    &gt;&gt; len(a)

-   Membaca data DBF

    &gt;&gt; import shapefile

    &gt;&gt; sf.records()

    &gt;&gt; sf.records(n)

Kesimpulan:

Dalam data Retrieve ini kita dapat melakukan select/view dan menghitung jumlah record. Dengan mendapatkan data shp kita juga belum tentu kita dapat melihat data tersebut namun kita juga harus menggunakan aplikasi sepert Qgis dan Python.

Saran:

Sebaiknya lebih banyak lagi orang yang mempelajari dan menggunakan data-data yang seperti diatas. Dan mempraktekannya, banyak orang yang mengerti tentang data retrieve pada data geospasial.

Link Github:

Nurpazrina

1144054

D4 Teknik Informatika 3B

Politeknik Pos Indonesia

Link Mata Kuliah:

<https://hanum189.wordpress.com/2013/02/11/pengantar-sig-2/>

Plagiarisme:

By smallseotools :

<https://drive.google.com/open?id=0B_4FZrdBxSUQNlNHcWFoMU1TY3M>

By duplichecker :

<https://drive.google.com/open?id=0B_4FZrdBxSUQeTVaaGtxbVo1ZVE>
