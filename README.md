# Anggota Kelompok
<ol>
  <li>Muhamad Al Kausar Ramadhan / 11</li>
  <li>Raihan Hidayatullah Djunaedi / 14</li>
</ol>
<h1>Link Papper</h1>
<p><a href="https://docs.google.com/document/d/10tetIfvd62SKziAbxYY1VwlFdeGprebNv7p-1xOThKE/edit?usp=sharing">Link Papper</a></p>
<h1>Penjelasan Proyek</h1>
<ul>
<li>Proyek ini bertujuan untuk menganalisis data pengangguran di Kabupaten Bekasi dan melakukan prediksi persentase kenaikan pengangguran di masa depan menggunakan metode regresi linear. Data pengangguran dikumpulkan dari sumber yang relevan dan tersedia dalam format CSV. Proses analisis terdiri dari dua bagian utama: visualisasi jumlah pengangguran dari tahun 2011 hingga 2022, dan prediksi persentase kenaikan pengangguran untuk lima tahun ke depan.</li>
</ul>
<h1>Cara Setup</h1>
<ul>
  <li>Pertama, kita memasang library pyspark dengan menjalankan perintah !pip install pyspark untuk memastikan bahwa kita memiliki modul yang diperlukan untuk mengakses dan menganalisis data dengan menggunakan Apache Spark.</li>
  <li>Selanjutnya, kita mengimpor beberapa modul yang diperlukan, seperti SparkSession dari pyspark.sql untuk menginisialisasi sesi Spark, dan matplotlib.pyplot untuk melakukan visualisasi grafik.</li>
  <li>Kita juga mengimpor modul lainnya seperti VectorAssembler dan LinearRegression dari pyspark.ml.feature dan pyspark.ml.regression secara berturut-turut, yang akan digunakan untuk membangun model prediksi persentase kenaikan pengangguran.</li>
</ul>
<h1>Cara Running</h1>
<ul>
  <li>Setelah setup selesai, kita dapat memulai dengan membaca dataset pengangguran dari file CSV yang tersimpan di Google Drive atau lokasi yang sesuai.</li>
  <li>Dataset tersebut kemudian difilter untuk Kabupaten Bekasi, sehingga hanya data yang relevan yang akan digunakan dalam analisis dan prediksi.</li>
  <li>Langkah berikutnya adalah mengelompokkan data berdasarkan tahun menggunakan fungsi groupBy dan menghitung jumlah pengangguran dengan menggunakan fungsi sum.</li>
  <li>Setelah itu, kita akan mengurutkan tabel hasil berdasarkan tahun secara menaik menggunakan orderBy.</li>
  <li>Tabel hasil jumlah pengangguran akan ditampilkan untuk memberikan gambaran data yang telah diolah.</li>
  <li>Selanjutnya, kita akan memvisualisasikan data pengangguran dari tahun 2011 hingga 2022 menggunakan matplotlib.pyplot. Grafik garis akan digunakan dengan sumbu x sebagai tahun dan sumbu y sebagai jumlah pengangguran.</li>
  <li>Setelah visualisasi selesai, kita akan memulai proses prediksi persentase kenaikan pengangguran.</li>
  <li>Data 10 tahun terakhir (2011-2022) akan dipilih dan digunakan untuk melatih model regresi linear menggunakan LinearRegression.</li>
  <li>Sebuah vektor fitur akan dibuat menggunakan VectorAssembler untuk mengubah fitur tahun menjadi vektor yang dapat digunakan oleh model.</li>
  <li>Model regresi linear akan dibangun dengan fitur sebagai vektor tahun dan label sebagai jumlah pengangguran.</li>
  <li>Dengan model yang telah dilatih, kita dapat melakukan prediksi jumlah pengangguran untuk 5 tahun ke depan menggunakan data tahun terakhir yang ada.</li>
  <li>Persentase kenaikan pengangguran dihitung dengan membandingkan prediksi dengan jumlah pengangguran terakhir dalam dataset.</li>
  <li>Prediksi persentase kenaikan pengangguran untuk 5 tahun ke depan akan ditampilkan untuk memberikan gambaran tren yang diharapkan.</li>
  <li>Akurasi prediksi diukur menggunakan metrik seperti Mean Squared Error (MSE) dan R-squared untuk mengevaluasi performa model regresi linear yang telah dibangun.</li>
</ul>
<h1>Penjelasan Metode</h1>
<h2>1. Visualisasi Jumlah Pengangguran</h2>
<ul>
<li>Dataset pengangguran difilter untuk Kabupaten Bekasi agar hanya data yang relevan yang digunakan dalam analisis.</li>
<li>Data jumlah pengangguran dikelompokkan berdasarkan tahun menggunakan fungsi groupBy dan diurutkan secara menaik menggunakan orderBy.</li>
<li>Tabel hasil jumlah pengangguran akan ditampilkan untuk memberikan gambaran data yang telah diolah.</li>
<li>Visualisasi dilakukan dengan menggunakan matplotlib.pyplot untuk membuat grafik garis yang menunjukkan perubahan jumlah pengangguran dari tahun ke tahun.</li>
<br>
</ul>
<h2>2. Prediksi Persentase Kenaikan Pengangguran</h2>
<ul>
<li>Dataset pengangguran difilter untuk Kabupaten Bekasi agar hanya data yang relevan yang digunakan dalam analisis.</li>
<li>Data jumlah pengangguran dikelompokkan berdasarkan tahun menggunakan fungsi groupBy dan diurutkan secara menaik menggunakan orderBy.</li>
<li>Data 10 tahun terakhir (2011-2022) dipilih untuk melatih model prediksi.</li>
<li>Preprocessing dilakukan dengan mengubah fitur tahun menjadi vektor menggunakan VectorAssembler.</li>
<li>Model regresi linear dibangun menggunakan LinearRegression dengan fitur sebagai vektor tahun dan label sebagai jumlah pengangguran.</li>
<li>Prediksi dilakukan untuk 5 tahun ke depan menggunakan data tahun terakhir yang ada.</li>
<li>Persentase kenaikan pengangguran dihitung dengan membandingkan prediksi dengan jumlah pengangguran terakhir dalam dataset.</li>
<li>Prediksi persentase kenaikan pengangguran untuk 5 tahun ke depan akan ditampilkan untuk memberikan gambaran tren yang diharapkan.</li>
<li>Akurasi prediksi diukur menggunakan metrik seperti Mean Squared Error (MSE) dan R-squared untuk mengevaluasi performa model regresi linear yang telah dibangun.</li>
<br>
</ul>
<h4>Dengan demikian, proyek ini menggabungkan analisis data, visualisasi, dan prediksi menggunakan Apache Spark dan metode regresi linear untuk menganalisis jumlah pengangguran di Kabupaten Bekasi dan meramalkan kenaikan pengangguran di masa depan.</h4>
<h1>Hasil Pratikum</h1>
<img src="docs/tabel pertama.png" />
<br>
<img src="docs/visualisasi pertama.png" />
<br>
<img src="docs/tabel kedua.png" />
<br>
<img src="docs/visualisasi kedua.png" />
