# Rice Leaves Disease

# 📄 Dokumentasi Proyek: Deteksi Penyakit Tanaman Padi Menggunakan CNN

## 1. Latar Belakang
Padi merupakan komoditas utama bagi ketahanan pangan nasional dan sumber penghidupan bagi jutaan petani, termasuk di Kabupaten Pringsewu, Lampung. Namun, serangan penyakit seperti **Blast**, **Brown Spot**, **Bacterial Blight**, dan **Tungro** dapat menurunkan produktivitas secara drastis. Di era digital, dibutuhkan solusi cerdas berbasis teknologi untuk membantu petani melakukan deteksi dini terhadap penyakit tanaman.

Teknologi **Convolutional Neural Network (CNN)** sebagai bagian dari kecerdasan buatan (AI) terbukti efektif dalam klasifikasi gambar dan kini dimanfaatkan dalam pertanian untuk mengidentifikasi penyakit tanaman padi secara otomatis dan akurat.

## 2. Tujuan Proyek
- Membangun sistem deteksi penyakit tanaman padi berbasis **CNN**.
- Mengklasifikasikan daun padi ke dalam 4 kategori penyakit: **Blast**, **Brown Spot**, **Bacterial Blight**, dan **Tungro**.
- Mendukung petani dalam pengambilan keputusan cepat untuk pengendalian penyakit.
- Mendorong produktivitas pertanian yang berkelanjutan dan inklusif di Pringsewu.

## 3. Dataset
Dataset yang digunakan terdiri dari **5923** gambar daun padi yang telah dikategorikan ke dalam 4 kelas:
- **Bacterial Blight**
- **Blast**
- **Brown Spot**
- **Tungro**

Setiap gambar direpresentasikan dalam format RGB dan diubah ukurannya menjadi (224, 224) piksel untuk pemrosesan model.

## 4. Arsitektur CNN
Model CNN yang digunakan terdiri dari:
- **Conv2D layers** dengan activation ReLU dan padding 'same'
- **MaxPooling2D layers** untuk reduksi dimensi
- **Dropout** untuk mengurangi overfitting
- **Flatten layer** untuk mengubah hasil conv menjadi vektor
- **Dense layer** dengan output 4 neuron (jumlah kelas)

Model dikompilasi menggunakan:
- **Loss Function**: `categorical_crossentropy`
- **Optimizer**: Adam
- **Metric**: Accuracy

## 5. Hasil Evaluasi
Setelah pelatihan, model diuji pada data validasi dengan hasil berikut:

- 📊 **Akurasi Validasi**: **90.44%**
- 📉 **Loss Validasi**: **0.2906**

Evaluasi lebih lanjut pada data uji menunjukkan:

- **Akurasi Akhir**: **89.54%**
- **Loss Akhir**: **0.3034**

Model ini cukup andal untuk klasifikasi penyakit tanaman padi dalam praktik nyata.

## 6. Keterkaitan dengan SDGs 2: Zero Hunger
Proyek ini selaras dengan **Tujuan Pembangunan Berkelanjutan (SDGs) nomor 2: Mengakhiri Kelaparan**, karena:
- Membantu petani meningkatkan produktivitas.
- Mencegah kerugian hasil panen melalui deteksi dini penyakit.
- Mendukung pertanian cerdas dan efisien di daerah seperti Pringsewu.

## 7. Dampak Ekonomi dan Keberlanjutan
Penerapan sistem ini berpotensi:
- Mengurangi biaya produksi akibat penyakit yang terlambat terdeteksi.
- Meningkatkan hasil panen dan pendapatan petani.
- Mendorong transformasi digital di sektor pertanian lokal untuk ekonomi yang inklusif dan berkelanjutan.
