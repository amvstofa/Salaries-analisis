# Salaries-Analisis

Analisis data gaji berdasarkan dataset yang berisi berbagai faktor seperti jabatan, pengalaman kerja, lokasi, dan ukuran perusahaan. Proyek ini dibuat menggunakan Jupyter Notebook untuk melakukan eksplorasi data, pembersihan, visualisasi, dan analisis pola distribusi gaji.

## 📊 Business Understanding
Industri teknologi dan bisnis saat ini sangat kompetitif, sehingga pemahaman terhadap struktur gaji menjadi hal penting baik bagi perusahaan maupun pencari kerja.  
Proyek ini bertujuan untuk:
- Mengidentifikasi pola distribusi gaji berdasarkan level pengalaman, jabatan, lokasi, dan ukuran perusahaan.
- Memberikan gambaran tren gaji yang dapat digunakan untuk negosiasi maupun perencanaan karier.
- Menyediakan insight yang dapat mendukung pengambilan keputusan strategis HR dan manajemen.

## 📂 Cakupan Informasi Dataset
Dataset gaji (salary dataset) biasanya mencakup informasi berikut:
- **work_year**: Tahun data gaji dikumpulkan.
- **experience_level**: Tingkat pengalaman karyawan (misalnya entry, mid, senior, executive).
- **employment_type**: Jenis kontrak kerja (FT, PT, kontrak, freelance).
- **job_title**: Jabatan atau posisi karyawan.
- **salary**: Jumlah gaji dalam mata uang asli.
- **salary_in_usd**: Gaji yang dikonversi ke USD untuk perbandingan global.
- **employee_residence**: Lokasi tempat tinggal karyawan.
- **remote_ratio**: Persentase kerja jarak jauh (0 = onsite, 50 = hybrid, 100 = full remote).
- **company_location**: Lokasi kantor utama perusahaan.
Link Dataset: https://www.kaggle.com/datasets/adilshamim8/salaries-for-data-science-jobs

### Persiapan
Dataset yang digunakan dalam proyek ini diperoleh dari repositori Kaggle. Dataset ini berisi informasi mengenai job_title, salary, experience_level, dll. Yang dapat dimanfaatkan untuk menganalisis faktor-faktor menganalisis faktor-faktor yang memengaruhi tingkat salary di berbagai faktor.
link dataset: https://github.com/dicodingacademy/dicoding_dataset/blob/main/students_performance/data.csv


1. Prasyarat
    - Bash/Terminal
    - Tableau Public (untuk visualisasi dashboard): [Tableau Public](https://public.tableau.com/app/profile/ahmad.musthofanur/viz/Jobssalariesdashboard_17548494349360/Dashboard1)
2. Remote CSV loading via `pandas`
Menggunakan link dataset yang tertera pada Tab *pengantar* di intruksi submission
     ```python
    url = '/content/drive/MyDrive/dataset/Data Science_AI & ML_Job_Salaries_ in_2025/salaries.csv'
    df = pd.read_csv(url)
    df.head()
    ```
3. Setup environment virtual di terminal VSCode menggunakan Bash
    ```python
    # Pastikan pipenv terpasang
    pip install pipenv
    # Buat virtual env & instal library dari Pipfile/requirements
    pipenv install
    # Masuk ke virtual env
    pipenv shell
    # Menginstal semua dependencies yang dibutuhkan saat pengerjaan proyek
    pip install -r requirements.txt
    ```
--- 
# Visualisasi Dashboard
Business dashboard yang telah dibuat dirancang untuk membantu Institusi Jaya guna melihat faktor-faktor apa saja yang memengaruhi tingginya angka Dropout. Dashboard ini memberikan wawasan tentang pola, hubungan antar variabel, dan faktor risiko utama yang memengaruhi keputusan mahasiswa untuk keluar.

1. Top 10 Employee Residence
- Bagian ini menampilkan jumlah tempat tinggal karyawan 10 teratas
2. Employment Type
- Bagian ini melihat jumlah distribusi tipe pekerjaan yang didominasi oleh karyawan Full-time 
3. Total Company By Size
- Bagian ini melihat jumlah distribusi ukuran company yang mayoritas ada pada company yang berukuran Medium
4. Experience Level
- Dari total Experience Level yang ada, hasil analisis menunjukkan bahwa posisi dengan Senior-Level mendominasi, yaitu sebesar 57.90% dari total data. Disusul oleh Mid-Level sebesar 30.28%, Entry-Level sebesar 9.30%, dan Executive-Level sebesar 2.52%.
5. Rata rata Salary di beberapa Negara
 - Analisis rata-rata gaji per negara ditampilkan dalam bentuk peta, di mana warna yang lebih pekat menunjukkan gaji yang lebih tinggi. Negara seperti Amerika Serikat, Kanada, dan China tercatat memiliki rata-rata gaji tertinggi
6. Rata-rata Salary bedasarkan ukuran Company
- Rata-rata salary tertinggi ditemukan pada perusahaan berukuran Large, disusul oleh Medium, dan yang terendah terdapat pada perusahaan Small.
7. Avg salay (USD) By job title and experience level
- Visualisasi tersebut menunjukkan bahwa semakin tinggi tingkat pengalaman, semakin besar gaji yang diperoleh, dengan peran di bidang AI seperti AI Architect, AI Data Scientist, dan AI Developer menempati jajaran gaji tertinggi, sementara jabatan non-AI cenderung lebih rendah namun tetap meningkat seiring pengalaman

---
Link Dashboard: Tableau Public (untuk visualisasi dashboard): [Tableau Public](https://public.tableau.com/app/profile/ahmad.musthofanur/viz/Jobssalariesdashboard_17548494349360/Dashboard1)
