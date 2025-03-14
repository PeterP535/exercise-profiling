# Performance Profiling Report

- **Name**: Peter Putra Lesmana
- **NPM**: 2306152361
- **Class**: Adpro-A

## Before Optimization

### Test Results (Via GUI)

#### /all-student-name
- **View Results Table**
  ![View Results Table](https://cdn.discordapp.com/attachments/916932753897967666/1350089104389574697/image.png?ex=67d577f5&is=67d42675&hm=9414645cb7eb8f3b5b761d0c49efc5f2f8e1c669a52f286ccd182ce35bf20680&)


#### /highest-gpa
- **View Results Table**
  ![View Results Table](https://cdn.discordapp.com/attachments/916932753897967666/1350089486620561450/image.png?ex=67d57851&is=67d426d1&hm=0bb761f92b4d409f7178e4b2b2a7a1e07abad5bca6fe6851457d85ac466eb97a&)


### Test Results (Via CLI)

#### /all-student-name
```sh
timeStamp,elapsed,label,responseCode,responseMessage,threadName,dataType,success,failureMessage,bytes,sentBytes,grpThreads,allThreads,URL,Latency,IdleTime,Connect
1741660686735,7438,all student name request,200,,Thread Group 1-5,text,true,,312447,132,10,10,http://localhost:8080/all-student-name,7424,0,2
1741660686431,7742,all student name request,200,,Thread Group 1-2,text,true,,312447,132,10,10,http://localhost:8080/all-student-name,7732,0,20
1741660687027,7146,all student name request,200,,Thread Group 1-8,text,true,,312447,132,10,10,http://localhost:8080/all-student-name,7143,0,1
1741660686530,7643,all student name request,200,,Thread Group 1-3,text,true,,312447,132,10,10,http://localhost:8080/all-student-name,7629,0,2
1741660687127,7046,all student name request,200,,Thread Group 1-9,text,true,,312447,132,10,10,http://localhost:8080/all-student-name,7032,0,1
1741660686628,7545,all student name request,200,,Thread Group 1-4,text,true,,312447,132,10,10,http://localhost:8080/all-student-name,7532,0,1
1741660686828,7352,all student name request,200,,Thread Group 1-6,text,true,,312447,132,4,4,http://localhost:8080/all-student-name,7350,0,1
1741660686430,7763,all student name request,200,,Thread Group 1-1,text,true,,312447,132,3,3,http://localhost:8080/all-student-name,7761,0,21
1741660687227,6967,all student name request,200,,Thread Group 1-10,text,true,,312447,132,2,2,http://localhost:8080/all-student-name,6966,0,1
1741660686928,7284,all student name request,200,,Thread Group 1-7,text,true,,312447,132,1,1,http://localhost:8080/all-student-name,7281,0,1
```

#### /highest-gpa
```sh
timeStamp,elapsed,label,responseCode,responseMessage,threadName,dataType,success,failureMessage,bytes,sentBytes,grpThreads,allThreads,URL,Latency,IdleTime,Connect
1741660833815,131,highest gpa request,200,,Thread Group 1-1,text,true,,275,127,3,3,http://localhost:8080/highest-gpa,127,0,30
1741660833815,131,highest gpa request,200,,Thread Group 1-2,text,true,,275,127,3,3,http://localhost:8080/highest-gpa,128,0,30
1741660833906,87,highest gpa request,200,,Thread Group 1-3,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,87,0,0
1741660834007,83,highest gpa request,200,,Thread Group 1-4,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,83,0,1
1741660834105,95,highest gpa request,200,,Thread Group 1-5,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,95,0,1
1741660834206,135,highest gpa request,200,,Thread Group 1-6,text,true,,275,127,2,2,http://localhost:8080/highest-gpa,134,0,1
1741660834311,94,highest gpa request,200,,Thread Group 1-7,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,94,0,1
1741660834409,85,highest gpa request,200,,Thread Group 1-8,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,85,0,1
1741660834520,82,highest gpa request,200,,Thread Group 1-9,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,82,0,1
1741660834611,104,highest gpa request,200,,Thread Group 1-10,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,104,0,0
```

## After Optimization

### Test Results (Via CLI)

#### /all-student-name
```sh
timeStamp,elapsed,label,responseCode,responseMessage,threadName,dataType,success,failureMessage,bytes,sentBytes,grpThreads,allThreads,URL,Latency,IdleTime,Connect
1741665464403,126,all student name request,200,,Thread Group 1-1,text,true,,312447,132,2,2,http://localhost:8080/all-student-name,122,0,13
1741665464440,97,all student name request,200,,Thread Group 1-2,text,true,,312447,132,1,1,http://localhost:8080/all-student-name,95,0,1
1741665464540,83,all student name request,200,,Thread Group 1-3,text,true,,312447,132,1,1,http://localhost:8080/all-student-name,82,0,0
1741665464640,85,all student name request,200,,Thread Group 1-4,text,true,,312447,132,1,1,http://localhost:8080/all-student-name,84,0,0
1741665464738,97,all student name request,200,,Thread Group 1-5,text,true,,312447,132,1,1,http://localhost:8080/all-student-name,96,0,1
1741665464838,109,all student name request,200,,Thread Group 1-6,text,true,,312447,132,2,2,http://localhost:8080/all-student-name,108,0,1
1741665464938,92,all student name request,200,,Thread Group 1-7,text,true,,312447,132,1,1,http://localhost:8080/all-student-name,91,0,1
1741665465039,101,all student name request,200,,Thread Group 1-8,text,true,,312447,132,2,2,http://localhost:8080/all-student-name,100,0,1
1741665465138,96,all student name request,200,,Thread Group 1-9,text,true,,312447,132,1,1,http://localhost:8080/all-student-name,95,0,0
1741665465237,88,all student name request,200,,Thread Group 1-10,text,true,,312447,132,1,1,http://localhost:8080/all-student-name,86,0,1
```

#### /highest-gpa
```sh
timeStamp,elapsed,label,responseCode,responseMessage,threadName,dataType,success,failureMessage,bytes,sentBytes,grpThreads,allThreads,URL,Latency,IdleTime,Connect
1741666636267,138,highest gpa request,200,,Thread Group 1-1,text,true,,275,127,3,3,http://localhost:8080/highest-gpa,133,0,14
1741666636302,109,highest gpa request,200,,Thread Group 1-2,text,true,,275,127,2,2,http://localhost:8080/highest-gpa,109,0,1
1741666636402,81,highest gpa request,200,,Thread Group 1-3,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,81,0,0
1741666636501,80,highest gpa request,200,,Thread Group 1-4,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,80,0,1
1741666636602,95,highest gpa request,200,,Thread Group 1-5,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,95,0,1
1741666636700,87,highest gpa request,200,,Thread Group 1-6,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,87,0,1
1741666636801,103,highest gpa request,200,,Thread Group 1-7,text,true,,275,127,2,2,http://localhost:8080/highest-gpa,103,0,1
1741666636899,81,highest gpa request,200,,Thread Group 1-8,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,81,0,1
1741666636999,100,highest gpa request,200,,Thread Group 1-9,text,true,,275,127,2,2,http://localhost:8080/highest-gpa,100,0,0
1741666637098,89,highest gpa request,200,,Thread Group 1-10,text,true,,275,127,1,1,http://localhost:8080/highest-gpa,89,0,1
```

# Kesimpulan
Setelah dilakukan optimasi, waktu eksekusi profil yang diukur mengalami peningkatan yang signifikan. Peningkatan ini menunjukkan efektivitas dari optimasi yang diterapkan, sehingga menghasilkan kinerja dan efisiensi aplikasi yang lebih baik.

# Refleksi

### Apa perbedaan antara pendekatan pengujian performa dengan JMeter dan pemprofilan dengan IntelliJ Profiler dalam konteks optimasi performa aplikasi?
Pengujian performa dengan JMeter berfokus pada simulasi beban pengguna dan mengukur waktu respons aplikasi, throughput, serta tingkat kesalahan dalam berbagai kondisi. Ini membantu mengidentifikasi masalah performa dari perspektif pengguna akhir. Sementara itu, pemprofilan dengan IntelliJ Profiler melibatkan analisis perilaku internal aplikasi, seperti penggunaan CPU, alokasi memori, dan waktu eksekusi metode, untuk mengidentifikasi hambatan performa pada tingkat kode.

### Bagaimana proses pemprofilan membantu Anda dalam mengidentifikasi dan memahami titik lemah dalam aplikasi?
Pemprofilan memberikan wawasan mendetail tentang perilaku runtime aplikasi, memungkinkan identifikasi jalur kode yang tidak efisien, kebocoran memori, dan operasi yang mengonsumsi sumber daya secara berlebihan. Dengan menganalisis data profil, Anda dapat memahami bagian kode mana yang menghabiskan sumber daya paling banyak dan menyebabkan degradasi performa.

### Apakah IntelliJ Profiler efektif dalam membantu Anda menganalisis dan mengidentifikasi hambatan dalam kode aplikasi Anda?
Ya, IntelliJ Profiler sangat efektif dalam menganalisis dan mengidentifikasi hambatan performa. Alat ini menyediakan berbagai fitur visualisasi dan pengukuran metrik performa, sehingga memudahkan dalam menemukan dan mengatasi masalah performa pada tingkat kode.

### Apa tantangan utama yang Anda hadapi saat melakukan pengujian performa dan pemprofilan, dan bagaimana Anda mengatasinya?
Tantangan utama mencakup waktu yang dibutuhkan untuk menyiapkan dan mengakses basis data untuk setiap endpoint karena jumlah data yang besar. Selain itu, variasi lingkungan komputer dan waktu eksekusi dapat menjadi tantangan yang signifikan. Untuk mengatasinya, saya mengoptimalkan kode aplikasi agar waktu yang dibutuhkan untuk menyiapkan dan mengakses basis data lebih singkat. Saya juga menjalankan pengujian JMeter dan IntelliJ Profiler beberapa kali untuk mengakomodasi variasi dan memvalidasi hasilnya.

### Apa manfaat utama yang Anda peroleh dari penggunaan IntelliJ Profiler untuk pemprofilan kode aplikasi?
Manfaat utama meliputi kemampuan untuk mengidentifikasi dan memperbaiki hambatan performa, mengoptimalkan penggunaan sumber daya, dan meningkatkan efisiensi aplikasi secara keseluruhan. Integrasi IntelliJ Profiler dengan lingkungan pengembangan juga memperlancar proses pemprofilan, menjadikannya lebih mudah diakses dan digunakan.

### Bagaimana Anda menangani situasi di mana hasil pemprofilan dengan IntelliJ Profiler tidak sepenuhnya konsisten dengan temuan dari pengujian performa menggunakan JMeter?
Tentu saja, hasilnya bisa bervariasi karena perbedaan metodologi dalam pengujian dan pemprofilan. Pengujian performa dengan JMeter mensimulasikan beban pengguna dan mengukur waktu respons, throughput, serta tingkat kesalahan, memberikan pandangan makro tentang performa aplikasi dalam berbagai kondisi. Sementara itu, pemprofilan dengan IntelliJ Profiler memberikan analisis yang lebih mendetail tentang perilaku internal aplikasi, seperti penggunaan CPU, alokasi memori, dan waktu eksekusi metode.

Meskipun terdapat perbedaan pendekatan, hasil dari kedua metode ini seharusnya tetap sejalan jika aplikasi berperforma secara konsisten. Ketidaksesuaian mungkin terjadi karena perbedaan lingkungan, konfigurasi pengujian, atau aspek spesifik dari performa yang diukur. Untuk mengatasi perbedaan ini, penting untuk melakukan validasi silang terhadap temuan dari kedua alat, membandingkannya dengan skenario dunia nyata, serta memastikan bahwa setiap optimasi yang dilakukan meningkatkan performa secara menyeluruh tanpa menimbulkan masalah baru.

### Strategi apa yang Anda terapkan dalam mengoptimalkan kode aplikasi setelah menganalisis hasil pengujian performa dan pemprofilan? Bagaimana Anda memastikan bahwa perubahan yang dilakukan tidak mempengaruhi fungsionalitas aplikasi?
Untuk mengoptimalkan performa aplikasi, saya menggunakan alat seperti JMeter dan IntelliJ Profiler untuk analisis. JMeter mensimulasikan beban pengguna dan mengukur waktu respons, sementara IntelliJ Profiler memberikan wawasan tentang penggunaan CPU dan alokasi memori. Dengan menggunakan alat-alat ini, saya dapat mengidentifikasi hambatan performa dan inefisiensi.

Upaya optimasi saya berfokus pada penghapusan fungsi yang tidak terpakai dan redundant, memastikan bahwa aplikasi berjalan secara efisien tanpa mengorbankan fungsionalitas. Pendekatan ini membantu dalam memahami dan menyelesaikan masalah performa secara efektif.

