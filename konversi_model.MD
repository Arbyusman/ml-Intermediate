Rangkuman Konversi Model Machine Learning
-----------------------------------------

Pengenalan Deployment dalam Machine Learning
--------------------------------------------

Pada tahap sebelumnya, kita telah mempelajari alur pengembangan machine learning yang melibatkan identifikasi masalah, persiapan data, pemilihan algoritma, pembangunan model, dan evaluasi kinerja. Namun, proses ini hanyalah bagian kecil dari keseluruhan sistem machine learning yang mencakup komponen-komponen yang saling berinteraksi.

### Fase Produksi dalam Machine Learning

Fase produksi adalah tahap penting untuk memastikan model prediksi dapat diakses dan digunakan secara luas, tidak hanya oleh teknisi atau programmer. Tujuan utama dari produksi adalah agar sistem machine learning dapat mengembalikan hasil prediksi secara real-time menggunakan data dari dunia nyata. Proses ini mencakup deployment, evaluasi, monitoring, dan manajemen model.

### Metode Deployment Model Machine Learning

1.  **Menggunakan Model Server**: Model di-deploy pada server yang dapat diakses oleh pengguna melalui API (REST atau gRPC). Contohnya adalah TensorFlow Serving.
    
2.  **Menggunakan Browser**: Model di-deploy langsung pada browser pengguna, memungkinkan prediksi dilakukan secara lokal tanpa mengirim data ke server. Contohnya adalah TensorFlow.js, ONNX.js.
    
3.  **Menggunakan Edge Devices**: Model di-deploy pada perangkat IoT atau mobile untuk prediksi tanpa koneksi internet. Contohnya adalah TensorFlow Lite (TFLite).
    

Format Penyimpanan Model
------------------------

1.  **SavedModel (TensorFlow):** Format standar untuk menyimpan model TensorFlow. Contoh kodenya adalah tf.saved\_model.save(model, 'mymodel/').
    
2.  **HDF5 (Keras):** Format penyimpanan model yang lebih ringan dan simpel. Contoh kodenya adalah model.save("model.h5").
    
3.  **ONNX (Open Neural Network Exchange):** Format yang mendukung interoperabilitas antar framework AI. Persiapan dimulai dari  Instal onnxruntime dan tf2onnx, lalu konversi model dengan perintah adalah !python -m tf2onnx.convert --saved-model "saved\_model" --output "model.onnx".
    

Pengenalan TensorFlow.js
------------------------

TensorFlow.js adalah framework yang memungkinkan pengembangan aplikasi machine learning di web browser menggunakan model yang diubah menjadi file JSON. Ini menyediakan dua tingkat API: Layers API (mirip Keras) dan Core API untuk operasi graf yang kompleks. TensorFlow.js memanfaatkan WebGL atau WebGPU untuk performa yang lebih baik.

Perbedaan antara TensorFlow.js dan TensorFlow Konvensional

*   **Platform**
    
    *   TensorFlow.js: Browser web atau Node.js.
        
    *   TensorFlow Konvensional: Server atau mesin lokal dengan Python.
        
*   **Bahasa Pemrograman**
    
    *   TensorFlow.js: JavaScript.
        
    *   TensorFlow Konvensional: Python.
        
*   **Kasus Penggunaan**
    
    *   TensorFlow.js: Aplikasi interaktif di browser.
        
    *   TensorFlow Konvensional: Pelatihan model skala besar dan deployment di server atau cloud.
        
*   **Instalasi dan Dependensi**
    
    *   TensorFlow.js: Mudah diintegrasikan dengan npm atau tag script di HTML.
        
    *   TensorFlow Konvensional: Instalasi melalui pip dengan konfigurasi tambahan untuk GPU atau lingkungan khusus.
        
*   **Performa**
    
    *   TensorFlow.js: Terbatas oleh kinerja JavaScript dan perangkat klien.
        
    *   TensorFlow Konvensional: Memanfaatkan sepenuhnya hardware dari mesin lokal atau server.
        
*   **Ekosistem dan Komunitas**
    
    *   TensorFlow.js: Ekosistem yang berkembang dengan alat dan plugin web.
        
    *   TensorFlow Konvensional: Mendukung berbagai alat dan pustaka tambahan dengan komunitas yang besar dan aktif.
        

### Penggunakan TensorFlow.js API pada Web Browser

TensorFlow.js memungkinkan pengembangan aplikasi machine learning langsung di web browser dengan cara yang fleksibel. Ada dua cara untuk mempersiapkan environment TensorFlow.js:

1.  Menggunakan CDN (Content Distribution Network)Anda dapat menambahkan script TensorFlow.js langsung ke HTML menggunakan tag \`\`. Class TensorFlow.js bisa diakses menggunakan objek \`tf\`.</div></li><li class="slate-li"><div style="position:relative">Menggunakan package manager (npm atau yarn)Jika Anda menggunakan Node.js atau ingin manajemen dependensi yang lebih baik, instal TensorFlow.js melalui npm atau yarn.</div></li><li class="slate-li"><div style="position:relative">Membuat Model Baru dengan TensorFlow.jsTensorFlow.js menyediakan dua cara untuk membuat model machine learning di JavaScript menggunakan Layers API yaitu Sequential Model dan Functional Model.</div></li><li class="slate-li"><div style="position:relative">Konversi Model TensorFlow ke TensorFlow.jsAnda dapat mengonversi model TensorFlow ke TensorFlow.js menggunakan \`tensorflowjs\_converter\`.</div></li></ol></x-turndown>
2.  


### Memuat Model TensorFlow.js di Browser

Untuk memuat model yang telah dikonversi ke TensorFlow.js di browser, Anda dapat menggunakan \`tf.loadLayersModel()\` atau \`tf.loadGraphModel()\`. Pastikan Anda menjalankan web server lokal untuk memuat model ini dari http. Setelah dimuat, Anda dapat menggunakan model untuk melatih ulang, evaluasi, atau mengambil prediksi langsung dari data yang diberikan.

### Konversi model TensorFlow ke TensorFlow.js

1.  Konversi dari SavedModel TensorFlow ke TensorFlow.js
    
2.  Konversi dari Keras HDF5 ke TensorFlow.js
    
3.  Konversi dari Frozen Model TensorFlow ke TensorFlow.js
    
4.  Konversi dari TensorFlow Hub ke TensorFlow.jS
    
5.  Memuat Model TensorFlow.js di Browser
    

Pastikan menjalankan kode ini di server HTTP untuk memuat model TensorFlow.js. Dengan langkah-langkah ini, Anda dapat mengonversi model TensorFlow dan memuatnya di browser untuk penggunaan dalam training ulang, evaluasi, atau inferensi.

Pengenalan TensorFlow Lite
--------------------------

TensorFlow Lite (TF-Lite) adalah sebuah framework yang memungkinkan eksekusi model TensorFlow pada perangkat mobile dan IoT. TF-Lite dirancang untuk mengoptimalkan ukuran model dan meningkatkan performa inferensi pada perangkat dengan sumber daya terbatas seperti smartphone, tablet, dan perangkat IoT.

Beberapa kegunaan TensorFlow Lite termasuk.

1.  **Google Translate Instant Camera Translation**: Menerjemahkan teks langsung dari foto, membantu pengguna memahami bahasa asing secara instan tanpa koneksi internet.
    
2.  **Fitur Makeup Virtual di Aplikasi E-commerce**: Memungkinkan pengguna untuk mencoba produk makeup secara virtual, membantu dalam pemilihan warna dan tampilan produk makeup.
    

Keuntungan utama dari penggunaan TensorFlow Lite meliputi.

1.  **Penggunaan Offline**: Tidak memerlukan koneksi internet untuk melakukan prediksi, menjaga privasi pengguna.
    
2.  **Ukuran dan Latensi Kecil**: Mengoptimalkan ukuran binary model dan mengurangi konsumsi daya saat melakukan prediksi.
    

Untuk menggunakan TensorFlow Lite, prosesnya melibatkan konversi model TensorFlow ke format TensorFlow Lite (\`.tflite\`) menggunakan TFLite Converter, yang kemudian dapat dieksekusi menggunakan TensorFlow Lite Interpreter di perangkat mobile atau IoT.

Berikut adalah langkah-langkah umum untuk mengonversi model TensorFlow menjadi TensorFlow Lite (\`.tflite\`).

### Konversi Model ke TensorFlow Lite

1.  Konversi dari SavedModel TensorFlow ke TensorFlow Lite.
    
2.  Konversi dari Keras HDF5 ke TensorFlow Lite.
    

Setelah model dikonversi ke format \`.tflite\`, model ini dapat dimuat dan dieksekusi menggunakan TensorFlow Lite Interpreter di lingkungan seperti aplikasi Android atau perangkat IoT yang didukung.

Pengenalan TensorFlow Serving (TF-Serving)
------------------------------------------

TensorFlow Serving (TF-Serving) adalah sistem server yang memfasilitasi deployment model machine learning pada server dengan menyediakan fleksibilitas dalam mengelola beberapa versi model sekaligus melalui arsitektur yang terstruktur. Pengguna dapat melakukan prediksi menggunakan model yang tersedia melalui servable handler, dengan pengaturan versi model yang dikelola oleh model manager dalam TF-Serving.

### Persiapan TensorFlow Serving

1.  Instalasi Docker. 
    
2.  Menyiapkan Kebutuhan Sistem pada Docker.
    
3.  Instalasi TensorFlow Serving Python API.
    

Setelah langkah-langkah di atas selesai, sistem Anda sudah siap untuk menggunakan TensorFlow Serving untuk deployment model machine learning pada server. Langkah selanjutnya adalah berlatih menjalankan model menggunakan TensorFlow Serving.


Federated Learning (FL)
-----------------------

Federated Learning (FL) adalah pendekatan modern dalam pembelajaran mesin yang mengatasi beberapa masalah utama dari sistem tradisional yang terpusat, seperti privasi, latensi, dan keterbatasan koneksi. Dalam FL, pelatihan model dilakukan secara terdistribusi di perangkat client yang menggunakan data lokal mereka. Model yang dihasilkan dari setiap client kemudian diagregasikan dan dikumpulkan kembali ke server, tanpa perlu mengungkapkan data pribadi client.

### Tahapan dalam Federated Learning:

1.  **Pelatihan Model di Perangkat Client**: Setiap perangkat client melakukan pelatihan model dengan menggunakan data lokalnya.
    
2.  **Aggregasi Model di Server**: Model dari setiap client diagregasikan dan dikumpulkan kembali ke server.
    
3.  **Privasi dan Keamanan**: Federated Learning menerapkan beberapa teknologi keamanan, seperti enkripsi data pada perangkat, agregasi aman untuk melindungi data yang dikirimkan, dan penghapusan data setelah digunakan.
    
4.  **Federated Model Averaging**: Teknik ini digunakan untuk menghitung rata-rata parameter model dari setiap client, yang mencerminkan kontribusi dari berbagai data lokal tanpa mengungkapkan data tersebut secara langsung.
    
5.  **TensorFlow Federated (TFF)**: TensorFlow Federated menyediakan API untuk implementasi FL, termasuk pengaturan training dan evaluasi yang dapat diterapkan pada model data yang ada.
    

TensorFlow Data Services (TFDS) untuk Data Pipelines
----------------------------------------------------

TensorFlow Data Services (TFDS) membantu mengelola data pada machine learning dengan menyediakan platform yang mudah diakses untuk mengintegrasikan dataset ke dalam pipeline training TensorFlow. Ini memfasilitasi:

*   Ekstraksi data dari sumber berbeda dan transformasi menjadi format yang digunakan untuk training.
    
*   Pengelolaan dataset dengan API konsisten untuk meminimalkan perbedaan dan memudahkan penggunaan.
    
*   Mempercepat proses training dengan dukungan GPU/TPU dan fleksibilitas dalam menangani berbagai jenis data.
    

Dengan TFDS, pengguna dapat fokus pada pengembangan model dan optimisasi tanpa harus khawatir tentang masalah ekstraksi, transformasi, atau konsistensi dataset.

Export Data ke Training Pipelines
---------------------------------

### Mengubah Dataset Menjadi Format TFDS

1.  **Import Library:** Import TensorFlow, Pandas, dan library lainnya yang dibutuhkan untuk pemrosesan data.
    
2.  **Baca File CSV:** Gunakan Pandas DataFrame untuk membaca file CSV yang diunduh dari Kaggle.
    
3.  **Split Dataset:** Bagi dataset menjadi training, validation, dan test set. Definisikan kolom target (0 = low, 1 = high) berdasarkan harga berlian.
    
4.  **Bungkus DataFrame dengan tf.data:** Gunakan tf.data untuk membuat dataset dari DataFrame. Ini memungkinkan penggunaan feature column sebagai jembatan dari DataFrame menjadi fitur yang digunakan untuk training model.
    
5.  **Feature Columns:** Ada beberapa jenis feature column:
    
    *   **Numeric Column:** Representasi sederhana dari fitur numerik.
        
    *   **Bucketized Column:** Membagi nilai numerik menjadi beberapa bucket.
        
    *   **Categorical Column:** Mengubah nilai string menjadi angka.
        
    *   **Embedding Column:** Representasi categorical column dengan nilai yang beragam.
        
    *   **Hashed Feature Column:** Alternatif representasi categorical column dengan banyak jenis value.
        
    *   **Crossed Feature Column:** Menggabungkan beberapa feature column menjadi satu.
        
6.  **Buat Feature Layer:** Pilih feature column yang akan digunakan dan buat feature layer sebagai input dalam model tf.Keras.
    
7.  **Create, Compile, and Train Model:** Tulis kode untuk membuat, meng-compile, dan melatih model menggunakan TensorFlow.
    

### Mempublikasi Model ke TensorHub

1.  **Membuat dan Mengekspor Model:** Simpan model yang sudah dilatih dalam format .pb dan simpan dalam direktori penyimpanan model yang sesuai.
    
2.  **Packaging Model:** Kompres model dalam format .tar.gz untuk menghemat traffic jaringan.
    
3.  **Menulis Dokumentasi:** Buat file markdown yang menjelaskan model, termasuk metadata penting seperti asset-path, module-type, fine-tunable, dan format model.
    
4.  **Membuat Permintaan Publikasi:** Lakukan push file model ke repositori TensorFlow Hub melalui Git CLI atau GitHub GUI, dan buat pull request untuk mempublikasikan model.
    

Pengenalan TensorBoard
----------------------

TensorBoard adalah alat visualisasi data dan parameter dalam pembelajaran mesin yang berfungsi untuk memantau dan memahami model machine learning. TensorBoard dapat menampilkan metrik seperti loss dan akurasi, visualisasi grafik model, histogram parameter, proyeksi embedding, visualisasi gambar, teks, dan data audio. TensorBoard juga memungkinkan kolaborasi tim dan publikasi eksperimen melalui Tensorboard.dev.

### Elemen Fungsional pada TensorBoard

1.  **Scalars**: Menampilkan perubahan loss dan metrik lainnya selama training. Membantu dalam memantau overfitting dan waktu training.
    
2.  **Graphs**: Memvisualisasikan struktur model dan detail layer.
    
3.  **Distributions dan Histograms**: Memantau perubahan parameter seperti bias dan bobot selama training.
    

### Setup TensorBoard

1.  **Mengaktifkan TensorBoard**: Gunakan %load\_ext tensorboard di Notebook atau Colab.
    
2.  **Membuat File Log**:
    
    *   Buat direktori log dengan datetime untuk nama unik.
        
    *   Buat file log dengan tf.summary.create\_file\_writer("./logs/").
        
3.  **Callback TensorBoard**: Tambahkan tf.keras.callbacks.TensorBoard() pada model.fit() untuk menghasilkan log selama training.
    

### TensorBoard Lokal

*   Jalankan %tensorboard --logdir logs/fit untuk menampilkan TensorBoard di dalam Colab.
    

### Tensorboard.dev

*   Unggah log ke Tensorboard.dev dengan !tensorboard dev upload --logdir logs/fit.
    

### Menampilkan Gambar

*   **Gambar Tunggal**: Gunakan tf.summary.image() untuk menampilkan gambar dari dataset.
    
*   **Banyak Gambar**: Gunakan tf.summary.image() dengan max\_outputs untuk menampilkan beberapa gambar sekaligus.
    
*   **Gambar dari Plot**: Gunakan fungsi plot\_to\_image untuk mengonversi plot Matplotlib ke gambar yang bisa dilog oleh TensorBoard.
    

### Menampilkan Confusion Matrix

1.  Buat plot confusion matrix dengan plot\_confusion\_matrix().
    
2.  Log matrix setiap epoch menggunakan callback LambdaCallback.
    

Memonitor Model
---------------

Model monitoring penting untuk memantau kinerja model dalam fase produksi. Ini melibatkan pemantauan akurasi, latensi, penggunaan memori/CPU, dan penurunan kinerja model seiring waktu (model drift). Dua jenis penurunan kinerja adalah sudden degradation dan slow degradation. Pemantauan dilakukan oleh tim DevOps dan data scientist.

### Metode Evaluasi Model

*   **Type 1 Error (False Positive)**: Kesalahan prediksi positif.
    
*   **Type 2 Error (False Negative)**: Kesalahan prediksi negatif.
    
*   **Akurasi**: Proporsi prediksi yang benar.
    
*   **Presisi**: Proporsi identifikasi kelas positif yang benar.
    
*   **Recall**: Proporsi kelas positif yang diklasifikasi dengan benar.
    
*   **Mean Squared Error (MSE)**: Rerata loss pada setiap baris data.
    

Pembaruan Model
---------------

*   **Manual Retraining**: Training ulang model secara manual.
    
*   **Continuous Learning**: Training ulang otomatis berdasarkan data baru.
    
*   **Pengujian A/B**: Membandingkan dua versi model untuk menentukan yang lebih baik.
    
*   **Multi Armed Bandit (MAB)**: Pengujian A/B yang dinamis untuk mengoptimalkan kinerja model secara terus-menerus.
    

### Prinsip Kunci dalam Pemantauan Model

1.  Monitor perubahan dependency.
    
2.  Monitor perbedaan data training dan live data.
    
3.  Monitor fitur pada training dan penyajian model.
    
4.  Monitor perbaruan model.
    
5.  Monitor kestabilan model.
    
6.  Optimalkan penggunaan resource seperti RAM dan latency.
    

Dengan memahami dan menerapkan langkah-langkah ini, kita dapat memastikan kinerja model machine learning tetap optimal dan relevan dengan perubahan data serta lingkungan operasional.