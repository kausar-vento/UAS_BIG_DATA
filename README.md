# Anggota Kelompok
<ol>
  <li>Muhamad Al Kausar Ramadhan / 11</li>
  <li>Raihan Hidayatullah Djunaedi / 14</li>
</ol>
<h1>Link Papper</h1>
<p><a href="https://docs.google.com/document/d/10tetIfvd62SKziAbxYY1VwlFdeGprebNv7p-1xOThKE/edit?usp=sharing">Link Papper</a></p>
 <h1>Cara Setup</h1>
<ul>
  <li>Mengimpor dataset pengangguran: Langkah pertama adalah mengimpor dataset pengangguran yang berisi informasi pengangguran di berbagai kabupaten, termasuk Kabupaten Bekasi.</li>
  <li>Melakukan filter dataset untuk Kabupaten Bekasi: Setelah mengimpor dataset, Anda perlu melakukan filter untuk memilih data yang terkait dengan Kabupaten Bekasi saja. Hal ini dilakukan dengan memfilter baris-baris yang memiliki nilai kabupaten sama dengan "Bekasi".</li>
  <li>Mengelompokkan data berdasarkan tahun dan menghitung jumlah pengangguran: Selanjutnya, Anda perlu mengelompokkan data berdasarkan tahun, dan menghitung jumlah pengangguran dalam setiap tahun. Ini dapat dilakukan dengan menggunakan fungsi agregasi seperti sum() pada kolom pengangguran, setelah Anda melakukan operasi pengelompokan berdasarkan kolom tahun.</li>
  <li>Melakukan preprocessing pada dataset dengan menggunakan VectorAssembler: Sebelum membangun model regresi linear, Anda perlu melakukan preprocessing pada dataset. Salah satu tahap preprocessing yang umum dilakukan pada data numerik adalah menggabungkan fitur-fitur menjadi satu vektor menggunakan VectorAssembler. Dalam hal ini, Anda dapat menggabungkan fitur tahun menjadi satu kolom vektor.</li>
  <li>Membangun model regresi linear: Setelah preprocessing selesai, Anda dapat membangun model regresi linear menggunakan dataset yang telah diproses. Model regresi linear digunakan untuk memodelkan hubungan antara variabel independen (tahun) dengan variabel dependen (jumlah pengangguran). Anda dapat menggunakan pustaka atau framework pemodelan yang mendukung regresi linear, seperti scikit-learn di Python.</li>
  <li>Membuat dataframe untuk melakukan prediksi pengangguran 5 tahun ke depan di Kabupaten Bekasi: Setelah model regresi linear selesai dilatih, Anda dapat menggunakan model tersebut untuk melakukan prediksi jumlah pengangguran di Kabupaten Bekasi 5 tahun ke depan. Untuk ini, Anda dapat membuat dataframe yang berisi 5 tahun ke depan (misalnya dari tahun sekarang hingga 5 tahun ke depan) dan menggunakan model untuk memprediksi jumlah pengangguran di setiap tahun.</li>
  <li>Mengubah hasil prediksi menjadi persentase: Setelah mendapatkan hasil prediksi jumlah pengangguran, Anda dapat mengubah nilai-nilai tersebut menjadi persentase. Hal ini dapat dilakukan dengan membagi setiap nilai prediksi dengan total populasi atau angkatan kerja di Kabupaten Bekasi pada tahun yang bersangkutan, lalu dikalikan dengan 100.</li>
  <li>Menampilkan prediksi jumlah pengangguran 5 tahun ke depan di Kabupaten Bekasi: Setelah mengubah hasil prediksi menjadi persentase, Anda dapat menampilkan prediksi jumlah pengangguran 5 tahun ke depan di Kabupaten Bekasi dalam bentuk grafik atau tabel, agar lebih mudah dipahami dan divisualisasikan</li>
  <li>Menghitung akurasi model menggunakan metrik RMSE dan R-squared: Setelah melakukan prediksi, Anda dapat mengukur akurasi model regresi linear dengan menggunakan metrik evaluasi seperti Root Mean Squared Error (RMSE) dan R-squared. RMSE digunakan untuk mengukur sejauh mana nilai prediksi mendekati nilai sebenarnya, sedangkan R-squared mengindikasikan seberapa baik model cocok dengan data yang ada.</li>
</ul>
<h1>Hasil Pratikum</h1>
<img src="docs/hasil prediksi.PNG" />
<img src="docs/hasil pratikum.PNG" />
