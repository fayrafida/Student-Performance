# Proyek Akhir: Menyelesaikan Permasalahan Jaya Jaya Institut

## Business Understanding

Jaya Jaya Institut merupakan institusi pendidikan perguruan yang telah berdiri sejak tahun 2000 dan dikenal luas karena telah melahirkan lulusan-lulusan dengan reputasi baik. Meskipun demikian, institusi ini menghadapi tantangan serius dalam hal tingginya angka siswa yang tidak menyelesaikan pendidikan mereka alias dropout. Tingginya angka dropout bukan hanya mencerminkan kegagalan dalam mempertahankan siswa hingga lulus, tetapi juga dapat memengaruhi reputasi, akreditasi, serta daya saing institusi di tengah persaingan dunia pendidikan yang semakin ketat.

Fenomena dropout ini dapat dipicu oleh berbagai faktor, mulai dari prestasi akademik yang rendah, ketidaksesuaian minat dengan program studi, hingga kendala sosial dan ekonomi. Jika tidak ditangani secara sistematis dan berbasis data, institusi berisiko kehilangan lebih banyak siswa potensial dan mengalami penurunan kualitas output pendidikan.

Untuk itu, Jaya Jaya Institut berinisiatif memanfaatkan pendekatan data-driven melalui penerapan teknologi Machine Learning. Dengan algoritma Random Forest, sebuah metode ensemble learning berbasis pohon keputusan yang dikenal kuat dalam menangani data dengan banyak fitur dan menghasilkan prediksi yang andal, institusi berharap dapat membangun sebuah sistem prediktif yang mampu mengidentifikasi siswa yang berisiko tinggi mengalami dropout sejak dini.

Dengan melakukan pelatihan model Random Forest pada data historis performa siswa, sistem dapat mempelajari pola-pola dropout berdasarkan fitur-fitur seperti nilai akademik, jumlah mata kuliah yang disetujui, kehadiran, dan latar belakang siswa. Hasil prediksi ini nantinya akan digunakan untuk memberikan intervensi dini dan bimbingan khusus kepada siswa yang terdeteksi memiliki risiko tinggi.

Sebagai bagian dari inisiatif ini, dibutuhkan pula dashboard interaktif untuk memvisualisasikan hasil analisis dan performa siswa secara real-time, sehingga manajemen dan staf akademik dapat mengambil keputusan strategis secara cepat dan tepat sasaran.

### Permasalahan Bisnis

Berdasarkan kondisi yang dihadapi oleh Jaya Jaya Institut, berikut adalah permasalahan bisnis utama yang ingin diselesaikan:

1. **Tingginya Angka Dropout Siswa**  
   Jumlah siswa yang tidak menyelesaikan pendidikan di Jaya Jaya Institut tergolong tinggi. Hal ini dapat menurunkan reputasi institusi, memengaruhi akreditasi, dan berpengaruh negatif terhadap kepercayaan calon siswa dan orang tua.

2. **Keterlambatan dalam Deteksi Risiko Dropout**  
   Saat ini belum tersedia sistem yang mampu mendeteksi secara dini siswa-siswa yang memiliki risiko tinggi untuk mengalami dropout. Akibatnya, intervensi atau bimbingan sering kali dilakukan terlambat.

3. **Kurangnya Pemanfaatan Data Historis Siswa**  
   Meskipun institusi telah mengumpulkan berbagai data akademik dan latar belakang siswa, data tersebut belum dimanfaatkan secara optimal untuk mendukung pengambilan keputusan strategis yang berbasis data.

4. **Kebutuhan Sistem Prediktif yang Akurat dan Andal**  
   Jaya Jaya Institut membutuhkan sistem berbasis machine learning, khususnya menggunakan algoritma Random Forest, untuk membangun model prediksi yang mampu mengidentifikasi siswa berisiko dropout secara akurat dan dapat dipercaya.

5. **Minimnya Visualisasi yang Informatif dan Interaktif**  
   Manajemen kesulitan dalam memantau performa siswa secara keseluruhan karena belum tersedia dashboard visual yang menampilkan data performa dan risiko dropout secara intuitif, terstruktur, dan mudah dipahami.

### Cakupan Proyek

Proyek ini dirancang untuk membantu Jaya Jaya Institut dalam mengidentifikasi siswa yang berisiko mengalami dropout secara dini. Adapun cakupan proyek yang akan dikerjakan meliputi:

1. **Eksplorasi dan Pra-pemrosesan Data**  
   - Memahami struktur dan kualitas data siswa yang tersedia.  
   - Melakukan pembersihan data, penanganan nilai hilang, dan encoding variabel kategori.

2. **Analisis Eksploratori (Exploratory Data Analysis - EDA)**  
   - Mengidentifikasi pola umum, tren, dan hubungan antar fitur yang berkorelasi dengan dropout.  
   - Menampilkan visualisasi distribusi dan korelasi antar variabel.

3. **Pengembangan Model Prediksi Dropout**  
   - Membangun model machine learning menggunakan algoritma **Random Forest** untuk memprediksi kemungkinan siswa mengalami dropout.  
   - Melakukan evaluasi model menggunakan metrik seperti accuracy, precision, recall, dan f1-score.

4. **Identifikasi Fitur Penting**  
   - Menganalisis fitur-fitur yang paling berkontribusi terhadap prediksi dropout untuk memberikan wawasan bagi tindakan preventif.

5. **Pembuatan Dashboard Visualisasi**  
   - Membangun dashboard interaktif yang menyajikan informasi penting terkait performa siswa dan hasil prediksi risiko dropout.  
   - Dashboard dirancang agar mudah diakses dan dipahami oleh pihak manajemen dan staf akademik.

6. **Rekomendasi Strategis**  
   - Menyusun rekomendasi tindakan bagi siswa berisiko tinggi berdasarkan hasil prediksi dan visualisasi data.

### Persiapan

Sumber data: [Student Performance](https://github.com/dicodingacademy/dicoding_dataset/tree/main/students_performance)

Setup environment:

Setelah file `requirements.txt` tersedia, Anda dapat menginstal seluruh dependensi yang dibutuhkan proyek menggunakan perintah berikut:

```bash
pip install -r requirements.txt
```

## Business Dashboard
[Link Dashboard](https://public.tableau.com/shared/RD82G6394?:display_count=n&:origin=viz_share_link)

Dashboard ini dikembangkan untuk membantu manajemen Jaya Jaya Institut dalam memahami pola dropout mahasiswa dan memantau indikator-indikator kunci yang berhubungan dengan risiko putus studi. Dengan tampilan visual yang interaktif, dashboard ini memungkinkan pihak institusi untuk melakukan eksplorasi data secara intuitif dan mengambil keputusan berbasis data (data-driven decision making).

1. Overview Dashboard

    Halaman ini memiliki komponen yaitu :

    - Jumlah Total Siswa, Jumlah Dropout, dan Dropout Rate ditampilkan secara ringkas untuk memberikan gambaran umum.

    - Pie Chart untuk proporsi status mahasiswa: Dropout, Enrolled, Graduate.

    - Proporsi Gender Mahasiswa, untuk melihat distribusi laki-laki vs perempuan.

    - Distribusi Usia Saat Mendaftar, memperlihatkan bahwa mayoritas siswa berada di kelompok usia 17–21 tahun.

    Dashboard ini bertujuan untuk memberikan konteks awal yang menyeluruh sebelum mengeksplorasi penyebab lebih lanjut.

2. Dropout Analysis
    Halaman ini memiliki komponen yaitu :

    - Jumlah Dropout Berdasarkan Program Studi, mengidentifikasi program-program yang memiliki tingkat dropout tertinggi.

    - Stacked Bar Gender dan Status Tempat Tinggal, menampilkan keterkaitan antara dropout, jenis kelamin, dan status tinggal (lokal vs pindahan).

    - Boxplot Admission Grade dan Previous Qualification Grade, untuk menganalisis perbedaan nilai antara siswa dropout dan non-dropout.

    Dashboard Dropout Analysis dirancang untuk membantu Jaya Jaya Institut dalam mengidentifikasi pola dan faktor utama yang berkontribusi terhadap tingginya angka dropout mahasiswa. 

3. Academic Performance

    Halaman ini memiliki komponen yaitu :

    - Scatter Plot Evaluations vs Approved Units di semester pertama, menggambarkan hubungan antara jumlah evaluasi dan jumlah unit yang disetujui.

    - Rata-rata Units Semester 1 dan 2 yang Disetujui, memperlihatkan bahwa siswa non-dropout memiliki pencapaian akademik lebih tinggi.

    - Distribusi Nilai Admission Grade, memperlihatkan bagaimana nilai awal berkorelasi dengan kemungkinan dropout.

    Tujuan dashboard ini adalah untuk menunjukkan seberapa besar peran performa akademik dalam memengaruhi dropout.

4. Socioeconomic Factors

    Halaman ini memiliki komponen yaitu :

    - Jumlah Dropout Berdasarkan Kualifikasi dan Pekerjaan Orang Tua (ayah dan ibu), untuk mengidentifikasi potensi pengaruh latar belakang sosial ekonomi terhadap dropout.

    Dashboard ini bertujuan untuk menyoroti bagaimana latar belakang keluarga, baik dari sisi pendidikan maupun pekerjaan, turut berperan dalam risiko dropout mahasiswa.

## Menjalankan Sistem Machine Learning

Sistem Machine Learning dapat dibuka melalui link : [Streamli](https://student-performance-fayrafida.streamlit.app/)

### Persiapan Awal
1. Download file project dalam bentuk `.zip`.
2. Ekstrak file zip ke folder yang diinginkan.

### Setup Menggunakan Anaconda
1. Buka Anaconda Prompt.
2. Arahkan ke folder project hasil ekstrak:
   ```bash
   cd path/ke/folder/project
   ```
3. Buat environment baru dan install dependencies:
	```bash
	conda create -n dashboard-env --file requirements.txt
	conda activate dashboard-env
	```
### Setup Menggunakan Shell/Terminal (tanpa Anaconda)

1.  Buka terminal atau command prompt.
2.  Arahkan ke folder project hasil ekstrak:
	```bash
	cd path/ke/folder/project
	```
3. Buat virtual environment dan install dependencies:
	```bash
	python -m venv venv
	source venv/bin/activate   # Linux/MacOS
	venv\Scripts\activate      # Windows
	pip install -r requirements.txt
	```
### Menjalankan Sistem 

Jalankan perintah berikut di terminal:
```bash
streamlit run dashboard.py
```

## Conclusion
Jelaskan konklusi dari proyek yang dikerjakan.

### Rekomendasi Action Items
Berikan beberapa rekomendasi action items yang harus dilakukan perusahaan guna menyelesaikan permasalahan atau mencapai target mereka.
- action item 1
- action item 2
