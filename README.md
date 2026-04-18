# klasifikasi-sentimen-ulasan-shopee
Klasifikasi sentimen ulasan aplikasi Shopee di App Store.

Proyek ini bertujuan untuk melakukan **klasifikasi sentimen** pada ulasan aplikasi **Shopee** di **App Store**.  
Analisis dilakukan untuk mengelompokkan ulasan pengguna ke dalam sentimen **positif**, **netral**, dan **negatif** menggunakan beberapa algoritma machine learning dan deep learning.

## Latar Belakang

Ulasan pengguna di platform digital sangat penting untuk mengetahui kualitas layanan dan kepuasan pengguna. Dengan analisis sentimen, kumpulan ulasan dapat diolah menjadi informasi yang lebih terstruktur sehingga dapat membantu dalam evaluasi aplikasi.

Pada proyek ini, data ulasan Shopee diproses melalui tahapan scraping, cleaning, preprocessing, hingga pelatihan model klasifikasi.

## Tujuan Proyek

- Mengumpulkan data ulasan aplikasi Shopee
- Membersihkan dan memproses teks ulasan
- Melakukan klasifikasi sentimen ke dalam 3 kelas
- Membandingkan performa beberapa algoritma
- Menentukan model dengan hasil terbaik

## Kategori Sentimen

Proyek ini menggunakan **3 kelas sentimen**, yaitu:

- **Positif**
- **Netral**
- **Negatif**

## Alur Pengerjaan

1. **Scraping Data**  
   Mengambil data ulasan aplikasi Shopee dari App Store.

2. **Cleaning & Preprocessing**  
   Tahapan preprocessing yang dilakukan meliputi:
   - case folding
   - cleaning text
   - tokenizing
   - stopword removal
   - stemming

3. **Pelabelan Data**  
   Data ulasan diberi label ke dalam tiga kategori sentimen: positif, netral, dan negatif.

4. **Training Model**  
   Model yang digunakan:
   - **SVM (Support Vector Machine)**
   - **Dense Neural Network**
   - **BiLSTM**

5. **Evaluasi Model**  
   Evaluasi dilakukan dengan membandingkan performa model dalam klasifikasi sentimen 3 kelas.

## Algoritma yang Digunakan

### 1. Support Vector Machine (SVM)
SVM digunakan sebagai model klasifikasi berbasis fitur teks hasil transformasi.

### 2. Dense Neural Network
Model Dense Neural Network digunakan untuk mempelajari pola sentimen dari representasi fitur teks secara lebih kompleks.

### 3. BiLSTM
BiLSTM digunakan untuk menangkap konteks urutan kata dari teks ulasan sehingga mampu memahami pola bahasa secara lebih baik.

## Hasil Akurasi

Berdasarkan hasil pengujian, diperoleh performa model sebagai berikut:

| Model | Akurasi Training | Akurasi Testing |
|------|------------------:|----------------:|
| SVM | 96.9% | 88.93% |
| Dense Neural Network | 99.29% | 92.10% |
| BiLSTM | 98.34% | 93.4% |

## Kesimpulan

Dari hasil evaluasi, model **BiLSTM** memberikan performa terbaik pada data testing dibandingkan model lainnya.  
Model ini mampu mencapai akurasi testing sekitar **93.4%**, sehingga dinilai paling baik dalam mengklasifikasikan sentimen ulasan Shopee ke dalam tiga kelas sentimen.
