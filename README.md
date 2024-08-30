## Membuat Visualisasi Data Lebih Efisien dan Efektif 
<br>Khusnun Nisa<br>
122450078<br>
RC<br>

### Pendahuluan
Visualisasi data merupakan sarana dalam menyajikan kisah data yang menarik kepada manusia yang lebih berorientasi secara visual. Visualisasi data sangat cocok untuk memberikan gambaran umum yang baik tentang data yang sangat besar dan mempermudah interpretasi hasil analisis data kepada ilmuwan data.

<ol>
    <li>Perkembangan Visualisasi Data</li>
  Komunitas data base meningkatkan pengalaman pengguna dengan visualisasi data secara real-time. Alur Visualisasi Data :
    <ul>
        <li>Impor data</li>
        <li>Persiapan data</li>
        <li>Manipulasi data</li>
        <li>Pemetaan</li>
        <li>Rendering</li>
    </ul>
  <li>Arah Visualisasi Data</li> 
    Tiga arah yang membuat visualisasi data menjadi lebih efisien dan efektif, namun tetap relevan bagi peneliti databse : 
    <ul>
        <li>Spesifikasi Visualisasi</li> Pengguna dapat menentukan apa yang mereka inginkan.
        <li>Pendekatan Efisien untuk Visualisasi Data</li> Melibatkan pengguna secara efektif dalam alur berulang, proses pembuatan harus efesien, terutama komponen "Manipulasi data" dan "Pemetaan".
        <li>Rekomendasi Visualisasi data</li> Sistem visualisasi dapat membantu pengguna secara cerdas dengan memberikan rekomendasi.
    </ul>  
  <li>Bahasa Visualisasi</li> 
    Survei yang dilakukan bahasa visualisasi dari perspektif tumpukan dan menekankan bagaimana bahasa digunakan dari perspektif praktis. Untuk rekomendasi visualisasi data, yang mana kami mensurvei bagaimana sistem yang berbeda merekomendasikan visualisasi yang mendalam bagi pengguna secara otomatis.
</ol>

### Spesifikasi visualisasi
<ol>
  <li>Spesifikasi visualisasi data</li> 
    Secara umum, bahasa visualisasi data terdiri dari tiga bagian: data, tanda (atau isyarat visual), dan pemetaan di antara keduanya.
  <li>Kategorisasi bahasa visualisasi data</li> 
    Dimensi lain untuk
memahami berbagai tingkat spesifikasi visualisasi bahasa adalah melalui
aksesibilitasnya (atau kemudahan penggunaannya): semakin tinggi tingkat
bahasanya, semakin mudah digunakan.
  <li>Operasi visual berbasis GUI</li> 
    cara yang lebih mudah digunakan dalam memberikan spesifikasi adalah dengan mengikuti "prinsip manipulasi langsung". Visualisasi Data Interaktif Rasionalitas di balik visualisasi data interaktif adalah
bahwa dalam banyak kasus, visualisasi data adalah proses eksplorasi, di mana
pengguna harus tetap menyimpan data. Meskipun alat interaktif berbasis GUI menyediakan antarmuka sederhana untuk membuat visualisasi umum dengan cepat, yang sangat penting bagi orang non-teknis, mungkin terdapat bagian yang tidak fleksibel untuk mengubah detail visualisasi.
  <li>Spesifikasi yang tidak ditentukan</li> 
    Secara umum, untuk spesifikasi yang tidak ditentukan, pengguna hanya memberikan beberapa “petunjuk”, dan merupakan tugas sistem visualisasi untuk menafsirkan masukan yang tidak ditentukan, dengan (mungkin) cara yang berbeda. Jenis petunjuk yaitu berbasis referensi, kberbasis ata kunsi dan berbasis bahasa alami.
</ol>

### Pendekatan efisien untuk visualisasi data
Namun terkadang, memberikan visualisasi yang tepat tidak selalu dapat dilakukan karena ukuran data yang besar dan kompleksitas kueri yang tinggi.
<ol>
    <li>Visualisasi data yang tepat</li>
    memanipulasi data dengan pernyataan SQL dan kemudian menggunakan alat visualisasi untuk merender visualisasi tersebut.
    <ul> 
        <li>Terjemahan Kueri</li> Cara alami untuk menggunakan kembali banyak
sistem yang sudah matang (DBMS) adalah dengan menerjemahkan kueri visualisasi ke kueri yang diterima sistem tersebut.
        <li>Mengintegrasikan Sistem Visualisasi dengan DBMS</li> Secara intuitif, cara yang menjanjikan untuk menyelesaikan masalah yaitu banyaknya fungsi yang diulang dan metode yang dipisahkan sehingga memerlukan penerbitan kueri terus menerus, adalah mengintegrasikannya.
        <li>Kolom Menyimpan</li> Pengguna biasayan hanya tertarik pada beberapa kolo, sehingga penyimpanan kolom dapat mencapai kinerja yang lebih baik, dibandingkan penyimpanan baris.
        <li>Indeks</li> mMmbangun indeks berbasis pohon hierarki untuk mendukung
pilihan pengguna dengan kondisi pemfilteran berkelanjutan.
        <li>Kmputasi Paralel</li> Kueri
agregasi pada ubin data di imMens [31] diparalelkan menggunakan representasi indeks padat dari ubin data. Menyediakan arsitektur multithreading untuk eksplorasi visualisasi interaktif.
        <li>Prediksi dan Pemngambilan Awal</li> Memprediksi data berikut yang mungkin diminati pengguna, lalu mengambil data terlebih dahulu/cache yang dapat digunakan pada langkah berikutnya selama eksplorasi saat ini dapat mempercepat proses eksplorasi. Teknologi prefect dan prediksi dikategorikan menjadi dua jenis, yaitu: Visualisasi yang Sedang Dieksplorasi dan Data Historis. 
    <li>Studi Kasus menggunakan Kyrix dan Tableau</li> Membahas dua studi kasus menggunakan Kyrix, sistem visualisasi data.
interaktif yang dapat diskalakan, dan Tableau, salah satu alat visualisasi
paling sukses. TDE mengoptimalkan mesin data terutama dalam 4 perspektif, yaiitu: Penyimpanan dan Kompresi Berorientasi Kolom, Pemesanan Ulang Operator. Pengurangan Kardinalitas dan Dukungan Visualisasi Lainnya.
    </ul>
    <li>Perkiraan Visualisasi Data</li>
    Untuk menjembatani kesenjangan antara volume data dan interaktivitas, banyak pekerjaan mempercepat fase pemrosesan data dengan memanfaatkan perkiraan pemrosesan kueri (AQP) yang memberikan perkiraan hasil visualisasi. Terdapat 3 perspektif dalam perkiraan visualisasi :
    <ul>
        <li>Berbasis AQP </li> Menggunakan subset representatif dari data dapat memberikan perkiraan visualisasi kepada pengguna interaksi online dengan mengorbankan kualitas. Di Pangloss, pengguna bisa mendapatkan wawasan awal dari hasil perkiraan dan kemudian memverifikasi pengamatan mereka pada hasil yang tepat.
        <li>Berbasis Pengambilan Sampel Inkremental</li> Ide utama dari perkiraan visualisasi dengan pengambilan sampel bertahap adalah bahwa sistem menghasilkan perkiraan visualisasi berdasarkan sampel representatif dari kumpulan data dengan cepat. IncVisAge adalah sistem berbasis web, yang menyediakan visualisasi perkiraan tambahan, dan tidak ada fluktuasi yang signifikan, sehingga memberikan visualisasi perantara yang bermakna bagi pengguna.
        <li>Berbasis Persepsi Manusia </li> Dimungkinkan untuk memperkirakan sistem visualisasi sistem untuk menghasilkan hasil perkiraan berdasarkan sampel yang representatif tetapi dengan dampak minimal terhadap kualitas visualisasi. PFunk-H menyajikan sebuah algoritma yang dapat mempelajari pengetahuan tentang kesalahan persepsi manusia untuk memberikan perkiraan visualisasi dan dapat memberikan batasan kesalahan pada perkiraan hasil kueri di bawah batasan fungsi
persepsi.
    </ul>    
    <li>Visualisasi Data Progresif</li>
    Secara umum, mereka membangun struktur hierarki dengan menggabungkan data dalam tingkat yang berbeda.
    <ul>
        <li>Binning Berbasis Rentang</li> Pengguna dapat menjelajahi data di berbagai level dan mengubah resolusi visualisasi yang dieksplorasi saat ini dengan memperbesar atau memperkecil, lalu, sistem akan mengubah ukuran wadah agregasi yang mendasarinya.
        <li>Pengelompokan Berbasis Rentang dan Konten</li> Algoritma konstruksi pohon bersifat adaptif dan dapat disesuaikan dengan kebutuhan pengguna. pemilihan preferensi untuk parameter pohon untuk mendukung pengalaman pengguna yang lebih baik.
    </ul>
</ol>

### Rekomendasi visualisasi
Bagian rekomendasi akan disusun berdasarkan: spesifikasi, berbasis perilaku dan yang dipersonalisasi. Dalam menyelesaikan permasalahan terdapat Ikhtisar Solusi dan Memangkas Visualisasi yang Tidak Berarti.
<ol>
    <li>Rekomendasi berdasarkan spesifikasi</li>
    <ul>
        <li>Spesifikasi tidak lengkap</li> Satu-satunya perbedaan antara spesifikasi kosong dan parsial adalah spesifikasi kosong harus memangkas ruang pencarian berdasarkan batasan yang ditentukan pengguna saat menghitung elemen visualisasi untuk menghasilkan kandidat visualisasi. 
        <li>Pemeringkatan visualisasi berdasarkan aturan</li> Sistem rekomendasi berbasis aturan memberi peringkat kandidat visualisasi berdasarkan aturan yang telah ditentukan sebelumnya. Terdapat 2 aturan, yaitu: statistik dan perseptual.
        <li>Peringkat visualisasi berbasis pembelajaran mesin</li> Dengan adanya dua visualisasi u dan v, sistem harus menentukan mana yang lebih baik. terdapat 2 sistem belajar, yaitu dengan batsan lunak dan dengan contoh.
        <li> Spesifikasi berbasis referensi</li> Biasanya, sistem akan merekomendasikan visualisasi yang mirip atau berbeda dari yang diberikan referensi dalam aspek tertentu. Seperti: SeeDB berbasis deviasi, Profiler berbasis anomali, Zenvisage berbasis Kesamaan/Jarak.
    </ul>    
    <li>Rekomendasi Berbasis Perilaku/li>
    Sistem rekomendasi berbasis perilaku menangkap perilaku pengguna saat ini
sebagai masukan, kemudian menyimpulkan tugas yang diinginkan pengguna dan merekomendasikan visualisasi yang berguna berdasarkan tugas mereka. jika a pengguna secara berulang memeriksa harga hotel di berbagai wilayah
peta, HARVEST dapat mendeteksi pola pemindaian, yang artinya bahwa pengguna ingin membandingkan beberapa atribut di antara beberapa atribut objek serupa, sehingga HARVEST dapat merekomendasikan diagram batang menunjukkan perbandingan harga hotel dari berbagai daerah.
    <li>Rekomendasi yang Dipersonalisasi</li>
    Sistem rekomendasi yang dipersonalisasi menangkap perilaku historis
pengguna sebagai masukan untuk merekomendasikan visualisasi menarik yang dipersonalisasi.
    <ul>
        <li>Model Linier</li> VizDeck memberikan hasil rekomendasi visualisasi yangmdipersonalisasi dengan melatih model linier setiap pengguna menggunakan perilaku historisnya, kemudian memberi skor vizlet untuk rekomendasi masa mendatang.
        <li>Pemfilteran Kolaboratif</li> Kolaboratif filtering (CF) [135] adalah algoritma rekomendasi hasil personalisasi yang banyak digunakan. Berdasarkan CF, VizRec mengusulkan tiga metode untuk rekomendasi visualisasi yang dipersonalisasi, yaitu: Pemfilteran Kolaboratif, Pemfilteran Berbasis Konten dan Penyaringan Hibrid.
    </ul>
</ol>

### Arah penelitian lainnya
<ol>
    <li>Persiapan Data Untuk Visualisasi Data</li>
    Secara alami, data yang divisualisasikan harus dibersihkan, seperti normalisasi nilai, deduplikasi, imputasi nilai yang hilang, dan deteksi outlier. Dampak data kotor pada visualisasi data :
    <ul>
        <li>Analisis Bagaimana-jika untuk Outlie</li>
        <li>Mengevaluasi Visualisasi dengan Data yang Hilang</li>
        <li>Mendeteksi visualisasi yang bias</li>
        <li>Pembersihan data sadar tugas</li>
    </ul>
    <li>Tolok Ukur Visualisasi Data</li>
    Terdapat fokus yang muncul pada pengembangan tolok ukur untuk ukuran
kinerja, yaitu :
    <ul>
        <li>Teknik desain visualisasi, dan mengembangkan model benchmark dan
algoritma untuk mengotomatisasi analisis visual</li>
        <li>Kategorisasi visualisasi</li>
        <li>Data pelatihan</li>
    </ul>
    <li>Visualisasi Data Untuk Aplikasi Terkait Database/li>
    Tentu saja, dengan pesatnya perkembangan teknik visualisasi, terdapat lebih banyak peluang dalam penggunaan visualisasi data untuk aplikasi yang berhubungan dengan database.
    <ul>
        <li>Visualisasi data untuk penemuan data</li>
        <li>Visualisasi data untuk debugging data</li>
    </ul>
</ol>







