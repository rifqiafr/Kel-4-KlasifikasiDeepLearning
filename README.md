# Deep Learning - Klasifikasi Sayuran menggunakan CNN

## Deskripsi Proyek

Proyek ini bertujuan untuk mengembangkan model **Deep Learning** menggunakan **Convolutional Neural Network (CNN)** untuk mengklasifikasikan berbagai jenis sayuran. Dengan pendekatan pembelajaran mendalam, model ini mampu mengenali dan mengklasifikasikan gambar sayuran dengan akurasi tinggi.

## Convolutional Neural Network (CNN)

**Convolutional Neural Network (CNN)** adalah jenis jaringan saraf tiruan yang dirancang khusus untuk pemrosesan data grid seperti gambar. CNN sangat efektif dalam pengenalan objek dan klasifikasi gambar karena kemampuannya dalam mendeteksi fitur dan pola pada data visual. CNN terdiri dari beberapa lapisan utama:

1. **Convolutional Layer**  
   Lapisan ini melakukan operasi konvolusi pada gambar input untuk mengekstraksi fitur seperti tepi, tekstur, dan pola dasar. Setiap konvolusi menghasilkan *feature maps* yang membantu mendeteksi pola dalam data.

2. **Activation Layer (ReLU)**  
   Fungsi aktivasi ReLU (Rectified Linear Unit) diterapkan setelah konvolusi untuk menghilangkan nilai negatif, yang meningkatkan non-linearitas dalam jaringan. Ini membantu model menangkap variasi yang lebih kompleks dalam data.

3. **Pooling Layer (Max Pooling)**  
   Pooling mengurangi dimensi dari *feature maps*, sehingga mempercepat proses komputasi dan mengurangi risiko overfitting. Lapisan ini mengambil nilai maksimum dari bagian kecil pada *feature maps*, yang dikenal sebagai *max pooling*.

4. **Flatten Layer**  
   Lapisan ini mengubah *feature maps* 2D dari lapisan konvolusi terakhir menjadi vektor 1D yang dapat dihubungkan ke lapisan padat. Ini adalah langkah transisi sebelum memasukkan data ke lapisan fully connected.

5. **Fully Connected Layer (Dense Layer)**  
   Di lapisan ini, setiap neuron terhubung dengan neuron di lapisan sebelumnya, memungkinkan jaringan untuk melakukan klasifikasi berdasarkan fitur yang diekstraksi. Lapisan ini biasanya ditempatkan di bagian akhir untuk menghasilkan output akhir yang mengklasifikasikan jenis gambar.

6. **Output Layer**  
   Lapisan ini adalah lapisan akhir dalam jaringan CNN yang menghasilkan prediksi. Biasanya menggunakan fungsi aktivasi seperti softmax untuk memberikan probabilitas pada setiap kelas.

Berikut adalah ilustrasi arsitektur CNN:

![image](https://github.com/user-attachments/assets/d0c99c57-5276-4006-8f5f-3a91252c6ada)

*Gambar di atas menunjukkan struktur umum dari CNN, mulai dari lapisan input hingga lapisan output.*

## Kelompok 4

Proyek ini dikembangkan oleh Kelompok 1 yang terdiri dari anggota berikut:

- Nanditha Nabiilah Putri (G1A021001)
- Gopi Mahendra (G1A021005)
- Nazir Mahmudi Lubis (G1A021013)
- Muhamad Rifqi Afriansyah (G1A021023)
- Vilda Aprilia (G1A021033)
- Erin Handayani Azzahra (G1A021049)
- Syakira Az Zahra (G1A021057)
- Muhamad Iqbal (G1A021073)
- Farhani Ilham Hidayatullah (G1A021081)
- Fajar Adhitia Suwandhi (G1A021086)

## Struktur File

- **Kel_4_DeepLearning_CNN_Vegetables_Python.ipynb**  
  Notebook ini berisi keseluruhan alur kerja pengembangan model deep learning, mulai dari pemrosesan data, pembentukan model CNN, pelatihan, evaluasi, hingga prediksi. Notebook ini dibangun menggunakan Python dan pustaka machine learning populer seperti Keras dan TensorFlow.

## Isi Notebook

### 1. Pengantar dan Tujuan
   Pada bagian ini dijelaskan latar belakang proyek, tujuan model yang dibangun, serta alasan pemilihan metode CNN untuk klasifikasi gambar.

### 2. Persiapan dan Import Library
   Berisi kode untuk mengimpor library yang dibutuhkan, seperti `tensorflow`, `keras`, `numpy`, `matplotlib`, dan lainnya.

### 3. Preprocessing Data
   Proses pemuatan dataset sayuran, yang mencakup:
   - Pemisahan data latih dan data uji.
   - Transformasi gambar agar sesuai dengan input model.
   - Augmentasi data untuk meningkatkan generalisasi model.

### 4. Arsitektur Model CNN
   Penjelasan tentang arsitektur jaringan saraf konvolusional (CNN) yang digunakan:
   - Jumlah dan tipe layer (Conv2D, MaxPooling2D, Flatten, Dense).
   - Fungsi aktivasi dan optimizer yang dipilih.

### 5. Pelatihan Model
   Tahapan pelatihan model, termasuk:
   - Konfigurasi parameter pelatihan, seperti epoch, batch size, dan loss function.
   - Monitoring akurasi dan loss pada data latih dan validasi.

### 6. Evaluasi Model
   Evaluasi model dengan menggunakan data uji. Metode evaluasi yang umum digunakan seperti akurasi, precision, recall, dan confusion matrix.

### 7. Prediksi dan Visualisasi Hasil
   Proses prediksi pada data baru dan visualisasi hasil prediksi, yang menunjukkan kemampuan model dalam mengenali jenis sayuran dengan akurat.

## Cara Menggunakan

1. **Clone repositori ini:**
   ```bash
   git clone https://github.com/rifqiafr/Kel-4-KlasifikasiDeepLearning.git
