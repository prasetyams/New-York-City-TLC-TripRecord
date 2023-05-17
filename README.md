# New York City TLC TripRecord Data Dictionary
# Latar Belakang

Komisi Taksi dan Limusin Kota New York (TLC), yang dibentuk pada tahun 1971, adalah badan 
yang bertanggung jawab untuk memberikan izin dan mengatur taksi Medallion (Kuning) Kota New York, taksi sewaan 
kendaraan (liveries berbasis komunitas, mobil hitam dan limusin mewah), van komuter, dan 
kendaraan paratransit. Dewan Komisi terdiri dari sembilan anggota, delapan di antaranya adalah 
Komisaris yang tidak digaji. Ketua/Komisaris yang digaji memimpin rapat rutin 
secara teratur memimpin rapat komisi publik yang dijadwalkan dan merupakan kepala badan, yang membawahi 
staf sekitar 600 karyawan TLC.
Lebih dari 200.000 pemegang lisensi TLC menyelesaikan sekitar 1.000.000 perjalanan setiap harinya. Untuk beroperasi untuk 
Untuk beroperasi, pengemudi harus terlebih dahulu menjalani pemeriksaan latar belakang, memiliki catatan mengemudi yang aman, dan 
menyelesaikan pelatihan pengemudi selama 24 jam. Kendaraan berlisensi TLC diperiksa untuk keselamatan dan emisi di Fasilitas Inspeksi Woodside TLC.

Sumber penjelasan latar belakang dapat diakses [di sini](https://www.kaggle.com/datasets/shuhengmo/uber-nyc-forhire-vehicles-trip-data-2021). 

# Pernyataan Masalah

Ingin membandingkan 2 VendorID apakah salah satu VendorId tersebut kurang baik, berdasarkan yaitu:

    1. Passenger_count, 

    2. Trip_distance 

    3. Total_amount

Siapakah VendorID yang kurang performanya?

# Kesimpulan dan Rekomendasi 

Dari analisis yang telah dilakukan, kita bisa membuat kesilpulan berikut tetang VendorID New York City TLC Trip Record Data Dictionary:

* VeriFone. (VendorID_2) paling unggul dibandingkan dengan Creative Mobile Technologies, LLC. (VendorID_1) berdasarkan, sebagai berikut: 

    1. passenger_count dari hour_of_day
    2. passenger_count dari day_of_week
    3. total_amount dari hour_of_day
    4. total_amount dari day_of_week
    5. trip_distance dari hour_of_day
    5. trip_distance dari day_of_week

* Kualitas (Performance) berdasarkan Creative Mobile Technologies, LLC. (VendorID_1), yaitu sebagai berikut:

    1. Dari passenger_count dari hour_of_day, menjelaskan bahwa pada jam-jam tertentu terdapat peningkatan kualitas pada passenger_count, yaitu jam 15 sebanyak 631.0 passenger_count, sedangkan terdapat penurunan kualitas passenger_count, yaitu jam 5 sebanyak 32.0 passenger_count.
    2. Dari passenger_count dari day_of_week, menjelaskan bahwa pada hari-hari tertentu terdapat peningkatan kualitas pada passenger_count, yaitu hari selasa (Tuesday) sebanyak 1,245 passenger_count, sedangkan terdapat penurunan kualitas passenger_count, yaitu hari sabtu (Saturday) sebanyak 885.0.
    3. Dari total_amount dari hour_of_day, menjelaskan bahwa pada jam-jam tertentu terdapat peningkatan kualitas pada total_amount, yaitu mulai jam 16 sebanyak 12,302.49 total_amount, sedangkan terdapat penurunan kualitas total_amount, yaitu jam 5 sebanyak 576.00 total_amount.
    4. Dari total_amount dari day_of_week, menjelaskan bahwa pada hari-hari tertentu terdapat peningkatan kualitas pada total_amount, yaitu hari selasa (Tuesday) sebanyak 24,235.76 total_amount, sedangkan terdapat penurunan kualitas passenger_count, yaitu hari sabtu (Saturday) sebanyak 15,909.27.
    5. Dari trip_distance dari hour_of_day, menjelaskan bahwa pada jam-jam tertentu terdapat peningkatan kualitas pada trip_distance, yaitu mulai jam 16 sebanyak 1,650.8 trip_distance, sedangkan terdapat penurunan kualitas trip_distance, yaitu jam 5 sebanyak 87.8 trip_distance.
    6. Dari trip_distance dari day_of_week, menjelaskan bahwa pada jam-jam tertentu terdapat peningkatan kualitas pada trip_distance, yaitu hari selasa (Tuesday) sebanyak 24,665.98 trip_distance, sedangkan terdapat penurunan kualitas trip_distance, yaitu hari sabtu (Saturday) sebanyak 2,394.6 trip_distance.

* Kualitas (Performance) berdasarkan VeriFone. (VendorID_2), yaitu sebagai berikut:

    1. Dari passenger_count dari hour_of_day, menjelaskan bahwa pada jam-jam tertentu terdapat peningkatan kualitas pada passenger_count, yaitu jam 18 sebanyak 5,083.0 passenger_count, sedangkan terdapat penurunan kualitas passenger_count, yaitu jam 5 sebanyak 460.0 passenger_count.
    2. Dari passenger_count dari day_of_week, menjelaskan bahwa pada hari-hari tertentu terdapat peningkatan kualitas pada passenger_count, yaitu hari selasa (Tuesday) sebanyak 10,226.0 passenger_count, sedangkan terdapat penurunan kualitas passenger_count, yaitu hari sabtu (Saturday) sebanyak 7785.0.
    3. Dari total_amount dari hour_of_day, menjelaskan bahwa pada jam-jam tertentu terdapat peningkatan kualitas pada total_amount, yaitu mulai jam 18 sebanyak 95,205.72 total_amount, sedangkan terdapat penurunan kualitas total_amount, yaitu jam 5 sebanyak 8938.49 total_amount.
    4. Dari total_amount dari day_of_week, menjelaskan bahwa pada hari-hari tertentu terdapat peningkatan kualitas pada total_amount, yaitu hari selasa (Tuesday) sebanyak 188,514.75 total_amount, sedangkan terdapat penurunan kualitas passenger_count, yaitu hari minggu (Sunday) sebanyak 141,581.38.
    5. Dari trip_distance dari hour_of_day, menjelaskan bahwa pada jam-jam tertentu terdapat peningkatan kualitas pada trip_distance, yaitu mulai jam 18 sebanyak 11643.62 trip_distance, sedangkan terdapat penurunan kualitas trip_distance, yaitu jam 5 sebanyak 1,525.87 trip_distance.
    6. Dari trip_distance dari day_of_week, menjelaskan bahwa pada jam-jam tertentu terdapat peningkatan kualitas pada trip_distance, yaitu hari selasa (Tuesday) sebanyak 3,268.4 trip_distance, sedangkan terdapat penurunan kualitas trip_distance, yaitu hari minggu (Sunday) sebanyak 20,331.27 trip_distance.

**Rekomendasi**
1. Dalam meningkatkan performance dari vendor VeriFone. (VendorID_2), sebaiknya jumlah vendor dari vendor VeriFone. (VendorID_2).
2. Diketahui bahwa pada Creative Mobile Technologies, LLC. (VendorID_1) memang jumlahnya lebih sedikit dibandingkan dengan VeriFone. (VendorID_2), maka dari itu sebaiknya Creative Mobile Technologies, LLC. (VendorID_1) lebih meningkatkan performanya berdasarkan passenger_count, total_amount dan trip_distance.
3. Memberikan preferensi kepada VeriFone (VendorID_2) sebagai pilihan vendor karena menunjukkan kinerja yang lebih baik dalam semua variabel yang diamati. Namun, keputusan akhir harus dipertimbangkan berdasarkan faktor-faktor lain yang relevan, seperti harga, layanan pelanggan, dan ulasan pengguna.

Berikut ini link Tableau:
https://public.tableau.com/shared/S2Z5GT9KM?:display_count=n&:origin=viz_share_link

