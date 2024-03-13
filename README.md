# **Tutorial Pemrograman Lanjut 2023/2024 Genap**
**I Made Surya Anahata Putra**<br/>
**2206081370**<br/>
**ProLan B**<br/>

# **Modul 5 - Advanced Programming**

## Reflection

1. What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?

Testing performa menggunakan JMeter dan profiling dengan IntelliJ Profiler mewakili dua pendekatan yang berbeda namun saling melengkapi dalam optimasi performa aplikasi. JMeter berfokus pada evaluasi aplikasi dari luar dengan mensimulasikan beban pengguna dan mengukur metrik seperti waktu respons dan throughput untuk menentukan kemampuan aplikasi dalam skenario dunia nyata. Di sisi lain, IntelliJ Profiler menawarkan pandangan yang lebih introspektif, memungkinkan pengembang untuk mengidentifikasi dan mengoptimalkan masalah performa internal seperti penggunaan CPU dan memori, serta bottleneck pada level kode.

2. How does the profiling process help you in identifying and understanding the weak points in your application?

Proses profiling membantu saya mengidentifikasi dan memahami titik lemah dalam aplikasi dengan memberikan detail tentang penggunaan sumber daya sistem seperti CPU, memori, dan I/O selama eksekusi aplikasi. Dengan melihat bagaimana sumber daya dikonsumsi, saya dapat menemukan bagian kode yang memakan banyak waktu prosesor, kebocoran memori, dan masalah performa lainnya seperti akses database yang tidak efisien atau penggunaan thread yang kurang optimal. Informasi ini memungkinkan saya untuk secara spesifik menargetkan dan mengoptimalkan area yang paling mempengaruhi performa, yang berguna pada peningkatan efisiensi kode, pengurangan waktu respons, dan peningkatan pengalaman pengguna. 

3. Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?

Menurut saya, IntelliJ Profiler sangat efektif dalam membantu saya menganalisis dan mengidentifikasi bottleneck dalam kode aplikasi. Alat ini memberikan kemampuan untuk dengan jelas melihat di mana sumber daya seperti CPU dan memori digunakan secara berlebihan, serta mengidentifikasi bagian kode yang menjalankan operasi secara tidak efisien. Dengan fitur visualisasi yang kuat dan integrasi langsung ke dalam lingkungan pengembangan, saya dapat dengan cepat menavigasi ke bagian kode yang bermasalah dan menerapkan perbaikan. 

4. What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?

Tantangan utama yang saya hadapi saat melakukan testing performa dan profiling tidak terkait langsung dengan proses testing atau profiling itu sendiri, tetapi lebih kepada persiapan yang diperlukan, seperti saat menginstal PostgreSQL dan membuat datanya. Saya merasa kesulitan saat membuat database karena melibatkan langkah-langkah seperti instalasi, konfigurasi, dan pengisian database dengan data uji yang representatif. Untuk mengatasi tantangan ini, saya pertama-tama memastikan bahwa saya mengikuti dokumentasi instalasi PostgreSQL dengan teliti, memperhatikan versi yang kompatibel dengan sistem operasi dan aplikasi saya. 

5. What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?

Menggunakan IntelliJ Profiler untuk profiling kode aplikasi memberikan saya beberapa manfaat utama yang meningkatkan kualitas dan efisiensi pengembangan. Pertama, alat ini memungkinkan saya untuk secara akurat mengidentifikasi bagian kode yang menyebabkan penurunan performa, seperti operasi yang memakan waktu lama atau penggunaan memori yang berlebihan. Kedua, integrasinya yang mulus dengan lingkungan pengembangan IntelliJ IDEA memudahkan saya untuk langsung memperbaiki masalah yang ditemukan tanpa perlu berpindah antar alat. Ketiga, fitur visualisasi yang detail membantu saya memahami perilaku aplikasi secara lebih intuitif, memudahkan identifikasi masalah dan validasi solusi.

6. How do you handle situations where the results from profiling with Inte	lliJ Profiler are not entirely consistent with findings from performance testing using JMeter?

Ketika hasil dari profiling dengan IntelliJ Profiler tidak sepenuhnya konsisten dengan temuan dari testing performa menggunakan JMeter, saya mengambil langkah untuk mendekati situasi ini dengan cara yang sistematis dan analitis. Pertama, saya memeriksa konteks di mana kedua jenis analisis dilakukan, mempertimbangkan perbedaan dalam skenario pengujian, seperti beban pengguna, konfigurasi sistem, dan kondisi runtime. Kemudian, saya fokus pada pemahaman perbedaan dalam metrik yang dikumpulkan oleh kedua alat, karena IntelliJ Profiler mungkin menyoroti masalah pada level kode, sementara JMeter mengungkapkan masalah pada level sistem atau infrastruktur. Untuk mengatasi ketidaksesuaian, saya melakukan iterasi pengujian dan profiling tambahan, dengan menyesuaikan kondisi untuk lebih mencerminkan lingkungan produksi sebenarnya. 

7. What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?

Setelah menganalisis hasil dari testing performa dan profiling, strategi yang saya terapkan dalam mengoptimalkan kode aplikasi meliputi refactoring kode untuk meningkatkan efisiensi, mengurangi penggunaan memori dengan mengelola sumber daya dengan lebih baik, dan mengoptimalkan query database untuk mengurangi waktu respons. Saya juga memprioritaskan perbaikan berdasarkan dampaknya terhadap performa aplikasi, fokus pada bottleneck yang paling signifikan terlebih dahulu. Untuk memastikan perubahan tidak mempengaruhi fungsionalitas aplikasi, saya melakukan testing komprehensif, termasuk unit testing, dan integration testing, untuk memverifikasi bahwa setiap aspek aplikasi masih berfungsi seperti yang diharapkan setelah perubahan dilakukan. Penggunaan version control system seperti Git juga memungkinkan saya untuk mengelola perubahan dengan efektif, memudahkan rollback jika diperlukan. 

## JMeter Report

### Endpoint /all-student
Test Result:
![Our Features](https://cdn.discordapp.com/attachments/1037716635227799613/1217272814097137804/image.png?ex=66036ca6&is=65f0f7a6&hm=79dc7fb16dad0fc30e82cae87a0a1f6b52c17b71c3e17385b5d71161cec83cba&)

Before Optimization:
![Our Features](https://cdn.discordapp.com/attachments/1037716635227799613/1217273903127203871/image.png?ex=66036daa&is=65f0f8aa&hm=54f818bac6d3e45f8932803048b2912817528be92687e1e8fe348ccca0b7e52f&)

After Optimization:
![Our Features](https://cdn.discordapp.com/attachments/1037716635227799613/1217274197181468732/image.png?ex=66036df0&is=65f0f8f0&hm=bea99c47ed573851897c7c67693dbd64595dd4c7ae22eb504e46d1754c6301d6&)

### Endpoint /all-student-name
Test Result:
![Our Features](https://cdn.discordapp.com/attachments/1037716635227799613/1217274399976198164/image.png?ex=66036e20&is=65f0f920&hm=1e920684cb529e6f186a4637a22d91409980e26bc0462a1f9d55efd29b5b306b&)

Before Optimization:
![Our Features](https://cdn.discordapp.com/attachments/1037716635227799613/1217273676224008242/image.png?ex=66036d74&is=65f0f874&hm=10ea82c2f15c9e6bf8623ef37c212997000a49b6c0876492fa189769aebc06db&)

After Optimization:
![Our Features](https://cdn.discordapp.com/attachments/1037716635227799613/1217274987891654766/image.png?ex=66036eac&is=65f0f9ac&hm=e063788c87f1641503895e7dfde22946f54c37d020be351c967518ce1b5f6159&)

### Endpoint /highest-gpa
Test Result:
![Our Features](https://cdn.discordapp.com/attachments/1037716635227799613/1217274685193195642/image.png?ex=66036e64&is=65f0f964&hm=676fb3051112f99be7d6ccebcff0c3229dc915cc1fd1f45899fe5d0f5ec00951&)

Before Optimization:
![Our Features](https://cdn.discordapp.com/attachments/1037716635227799613/1217274650778665041/image.png?ex=66036e5c&is=65f0f95c&hm=ddb78f4ee8b2be97c0fd18b9a9dc95e4b2815fd3c18cf245592a34a6ab94a88e&)

After Optimization:
![Our Features](https://cdn.discordapp.com/attachments/1037716635227799613/1217275036877197333/image.png?ex=66036eb8&is=65f0f9b8&hm=981134f0fdf4df6ab2535bfc783b165c5cd46f27a304f75a6b6151b3f98946e6&)