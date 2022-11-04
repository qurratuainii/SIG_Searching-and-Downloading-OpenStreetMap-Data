# SIG_Searching-and-Downloading-OpenStreetMap-Data

*Tutorial Searching and Downloading OpenStreetMap Data

1. Cari dan instal plugin QuickOSM dari Plugin Repository resmi QGIS. Lihat menggunakan plugin untuk petunjuk tentang mengunduh plugin. PAstikan kita memiliki kotak centang yang dipilih, setelah itu klik close (*Gambar 1*)

2. Setelah terinstal, luncurkan pludin dari Vector QuickOSM lalu pilih QuickOSM... (*Gambar 2*)

3. Pada tab Quick query, kita dapat mengatur filter untuk memilih subkumpulan. Atribut fitur peta dalam database OSM disimpan sebagai Tag. Tag direpresentasikan dengan kunci dan nilai. Kuncinya adalah topik dan nilai adalah bentuk tertentu. Lihat halaman wiki Fitur Peta OSM untuk daftar lengkap tag intuk berbagai jenis fitur. Batang direpresentasikan menggunakan tag amenity: bar dan pub dengan tag amenity:pub. Kami akan mengestrak bar terlebih dahulu (*Gambar 3*)

4. Pilih bilah dari menu value drop-down (*Gambar 4*)

5. Kami dapat menghubungkan beberapa kueri dalam versi terbaru (v2.0.0 +) dari plugin QuickOSM. Klik tombol plus, bilah pemilihan kueri berikutnya akan muncul. Klik pada kotak pilihan pertama di mana kita bisa mendapatkan opsi dan atau. Dan hanya akan memilih fitur yang benar untuk semua kueri. Atau akan memilih semua fitur yang benar untuk salah satu kueri. Klik atau untuk memilih fitur bar dan pub (*Gambar 5*)

6. Pilih amenity sebagai kunci dari menu drop-down. Kemudian pilih pub dari menu value drop-down (*Gambar 6*)

7. Masukkan london sebagai In untuk membatasi pencarian di dalam batas kota (*Gambar 7*)

8. Perluas bagian lanjutan. Dalam model data OSM, fitur direpresentasikan menggunakan node, cara dan relasi. Karena kami tertarik dengan fitur titik, kita hanya dapat memilih node dan points. Klik run query (*Gambar 8*)

9. Setelah query selesai, alihkan ke jendela utama QGIS. Kita akan melihat layer baru bernama amaenity_bar_amenity_pub_London ditambahkan ke panel Layers. Kanvas akan menunjukkan lokasi bar dan pub yang diekstraksi (*Gambar 9*)

10. Buka tabel Atribut pada layer. Ada 2.091 fitur. Fasilitas kolom berisi kategori apakah fitur tersebut pub atau bar. Dengan menggunakan kolom categorical, kita bisa menata layernya (*Gambar 10*)

11. Klik icon panel Open the Later Styling, pilih Categorized, lalu di value pilih amanity lalu klik Classify. Sekarang layer akan ditata dengan 2 warna yang menampilkan pub dan bar (*Gambar 11*)

12. Sekarang klik kanan pada layer, Export lalu pili Save Features As... untuk mengekspor layer sebagai GeoPackage (*Gambar 12*)

13. Pada kotak dialog Save Vector Layer as... , pada Format pilih GeoPackage, pada file name klik... dan browase ke direktori tempat kita ingin menyimpan data dan beri nama output london.gpkg. Dalam nama layer masukkan bar_and_pubs. Klik OK (*Gambar 13*)

14. Sekarang layer GeoPackage london_bar_and_pubs akan ditambahkan ke kanvas (*Gambar 14*)
