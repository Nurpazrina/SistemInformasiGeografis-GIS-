**PENAMBAHAN CLASS PADA RETREIVE DATA GEOSPASIAL**

<p align="center">
  <img src ="../../img/Pertemuan 3.jpg" width="400px">
</p>

**Latar Belakang**

Data Geospasial merupakan pengetahuan yang mepelajari tentang titik koordinat dari suatu peta atau juga dapat disebut dengan mempelajari tentang geografis yang ada bumi. Didalam geospasial itu sendiri ada untuk manipulasi data dan menghitung record pada file .shp, dan pada pembahasan kali ini terdapat tentang class retrieve data geospasial terdapat 2 data pada DBF dan SHP. Untuk membaca shapefile kita dapat menggunakan python kita dapat memanggil langsung file shp nya atau juga bisa membuat class terlebih dahulu untuk melihat record data sedangkan shp adalah melihat data geometri.

**Pembahasan/Isi**

**Retrieve data geospasial** adalah merupakan suatu cara untuk melakukan select/view, data record dari file dbf dan geometri dari file shp.

Dalam pembahasan kali ini Retreive data geospasial yaitu dengan mengambil data vector ESRI/shapefile dibagi 2 terdapat DBF dan SHP. Terdapat 3 Geometri standar ESRI

1.  Point

2.  Poline

3.  Poligon

**Penjelasan:**

**Poin** dalam peta biasanya menunjukan sebuah tempat misalnya restoran

**Polygon** dalam peta biasanya menunjukan sebuah pulau

Perbedaan **Polygon** dan **Polyline** adalah titik awal dan akhir polygon selalu bertemu sedangkan tidak dengan polyline.

**Operasi pada Python:**

**Implementasi Retrieve Data Geospasial dalam python:**

&gt;&gt;sf = shapefile.Reader(‘namafile.shp’)

**sf** adalah variable

**shapefile** adalah nama class

**Reader** adalah nama method

**Perintah untuk mengambil data perkolom:**

&gt;&gt;sf.record(n)\[n\]

**Perintah untuk melihat isi shapefile:**

&gt;&gt;a = sf.shape(0)

&gt;&gt;dir(a)

**Untuk melihat type:**

&gt;&gt; a.shapetype

**Mencari negara:**

&gt;&gt; for a in sf.records():

&gt;&gt; if a\[8\] == “indonesia”

&gt;&gt; print a

**Melihat Baris:**

&gt;&gt; Print i

&gt;&gt; i = i + 1

**Kesimpulan:**

Dalam data Retrieve ini kita dapat melakukan select/view dan menghitung jumlah record. Dengan mendapatkan data shp kita juga belum tentu kita dapat melihat data tersebut namun kita juga harus menggunakan aplikasi sepert Qgis dan Python.

**Saran:**

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

<https://drive.google.com/open?id=0B_4FZrdBxSUQRzFRcTQ3MHd4bms>

By duplichecker :

https://drive.google.com/open?id=0B\_4FZrdBxSUQTmM4NE41QVRDcE0
