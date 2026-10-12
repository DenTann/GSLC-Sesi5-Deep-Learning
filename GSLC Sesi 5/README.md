# GSLC Deep Learning: Oxford-IIIT Pet Classification

Repositori ini berisi kode, eksperimen, dan laporan analisis perbandingan model Convolutional Neural Network (CNN) pada dataset **Oxford-IIIT Pet** (subset 10 kelas).

## Struktur Repositori
- `Bagian_A - 2802393030.pdf`: Dokumen laporan lengkap jawaban esai (Bagian A).
- `Bagian_B - 2802393030.ipynb`: Notebook utama berisi seluruh eksperimen pelatihan dan evaluasi model.
- `Bagian_C - 2802393030.pdf`: Dokumen laporan lengkap hasil analisis (Bagian C).
- `Results`: Folder penyimpanan artefak visualisasi dan hasil evaluasi model (kurva loss, *failure analysis*, dan metrics_log).
- `requirements.txt`: Daftar pustaka dependensi Python.

## Kondisi Eksperimen
1. **B1**: Pelatihan dari nol (*From Scratch*) menggunakan arsitektur ResNet-18.
2. **B2**: *Feature Extraction* murni (membekukan *backbone* ResNet-18).
3. **B3**: *Progressive Fine-Tuning* (membuka lapisan `layer4` ResNet-18).
4. **B4**: Analisis Augmentasi Data (tanpa vs dengan augmentasi).
5. **B5**: Pengujian arsitektur alternatif efisien (**MobileNetV3**).

## Cara Menjalankan
1. Unggah berkas `Bagian_B - 2802393030.ipynb` ke **Google Colab**.
2. Pastikan *runtime* menggunakan GPU (T4 / P100).
3. Jalankan sel secara berurutan (*Run All*).