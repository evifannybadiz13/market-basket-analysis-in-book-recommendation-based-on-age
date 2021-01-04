# Market Basket Analysis In Book Recommendation Based On Age

### Topik		: Market Basket Analysis

#### Business Understanding		
a.	Business Objectives

Stok buku merupakan permasalahan operasional yang sering dihadapi oleh toko buku. Jika jumlah buku terlalu sedikit dan permintaan tidak dapat dipenuhi karena kekurangan persediaan, maka akan mengakibatkan konsumen merasa kecewa dan ada kemungkinan konsumen tidak akan kembali lagi. Begitu juga jika pengadaan terlalu besar, maka akan mengakibatkan kerugian bagi toko buku karena harus menyediakan tempat yang lebih besar, terjadinya penyusutan nilai guna buku, serta harus menyediakan biaya tambahan yang terkait dengan biaya inventori seperti biaya pemeliharaan buku. Salah satu cara yang dapat dilakukan untuk mengetahui kondisi pasar (konsumen) adalah dengan mengamati transaksi penjualan buku tersebut. Data transaksi penjualan yang disimpan dalam basis data dapat diolah lebih lanjut sehingga didapatkan informasi baru. Jika diketahui bahwa konsumen yang membeli satu buku cenderung membeli buku lain maka memungkinkan bagi produsen toko buku untuk memasarkan buku tersebut bersama-sama. Keterkaitan buku tersebut merupakan informasi berharga yang dapat digunakan sebagai strategi pemasaran.


Pada proyek ini, market basket analysis dilakukan dengan algoritma apriori untuk mengetahui hubungan atau pola-pola yang dihasilkan berdasarkan buku yang dibeli oleh konsumen. Market Basket Analysis hadir sebagai solusi bagi produsen toko buku untuk mengambil keputusan dalam menentukan strategi pemasaran dan keterkaitan antara buku yang dibeli oleh konsumen sehingga dapat meningkatkan pelayanan pada konsumen. Jika seorang konsumen membeli buku A dan berdasarkan history transaksi penjualan, konsumen yang membeli buku A juga membeli buku C maka sistem akan memberikan rekomendasi kepada konsumen tersebut untuk membeli buku C. 

b.	Situation Assessment

Toko Buku ABC merupakan toko yang menjual berbagai kategori buku. Toko ini ingin meningkatkan pendapatan dengan menentukan strategi pemasaran yang tepat. History data penjualan buku dapat digunakan untuk mengetahui hubungan atau pola-pola yang dihasilkan berdasarkan buku yang dibeli oleh konsumen. History data tersebut antara lain berupa id buku, id users, rating, dan lain-lain. Atribut terkait transaksi ini akan menjadi fokus untuk memberikan rekomendasi kepada konsumen di Toko Buku ABC berdasarkan algoritma apriori.
 
c.	Data Mining Goal

Tujuan dari pengerjaan proyek adalah sebagai berikut: 

1.	Mendapatkan informasi mengenai behaviour konsumen dan memahaminya berdasarkan transaksi pembelian buku. 

2.	Mempelajari buku yang paling banyak dibeli oleh konsumen. 

3.	Menghasilkan model rekomendasi buku berdasarkan umur  melalui data yang tersedia dan menyarankan buku kepada konsumen.

d.	Produce Project Plan

Proyek ini akan menggunakan algoritma Apriori pada python. Data transaksi penjualan buku akan dianalisis terlebih dahulu kemudian dilakukan preparasi data dengan menghapus beberapa atribut yang tidak dibutuhkan. Kemudian proses market basket analysis dilakukan dengan menggunakan algoritma Apriori untuk menemukan semua aturan Apriori yang memenuhi syarat minimum berupa support dan syarat minimum untuk confidence. Penerapan Algoritma Apriori dapat membantu dalam membentuk kandidat kombinasi item, kemudian dilakukan pengujian apakah kombinasi tersebut memenuhi parameter support dan confidence minimum yang merupakan nilai ambang yang diberikan oleh tim. Jika memenuhi parameter support dan confidence maka hasil tersebut dapat membantu dalam penentuan pola penjualan buku.
Setelah pola transaksi penjualan buku diperoleh maka dilakukan pengelompokkan buku tersebut berdasarkan umur konsumen. Hasil akhir dari proses ini berupa rekomendasi pola-pola transaksi buku yang dibeli sehingga menjadi informasi bagi produsen untuk menentukan strategi pasar dan juga berupa rekomendasi buku yang memiliki pola yang sama jika dilakukan transaksi pembelian buku.

Data understanding

a.	Collect Initial Data

b.	Describe Data

c.	Explore Data

d.	Verify Data Quality

Pada proyek ini, dataset pada kaggle.com yang digunakan adalah Book-Crossing: User review ratings yang merupakan kumpulan data buku. Dataset ini terdiri dari 278,858 users (anonim tetapi dengan informasi demografis), 1,149,780 ratings (eksplisit/implisit), dan 271,379 books.
