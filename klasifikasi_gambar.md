Rangkuman Klasifikasi Gambar
----------------------------

Berikut adalah rangkuman dari modul Klasifikasi Gambar.

Pendahuluan Klasifikasi Gambar
------------------------------

**Klasifikasi gambar** merupakan salah satu aplikasi penting dalam deep learning untuk mengidentifikasi kategori atau label dari suatu gambar berdasarkan konten visualnya. Metode ini adalah cabang **computer vision,** yang merupakan subdisiplin kecerdasan buatan berfokus pada pengenalan dan pemahaman gambar oleh komputer.

Namun, cabang dari computer vision tidak hanya klasifikasi gambar. Ada juga klasifikasi dan lokalisasi (_classification and localization_) dan deteksi objek (_object detection_). Klasifikasi adalah tentang mengenali objek dalam gambar; klasifikasi dan lokalisasi menambahkan informasi tentang letaknya; sementara deteksi objek melibatkan mengenali dan menandai semua objek dalam gambar.

Dasar-Dasar Convolutional Neural Networks (CNNs)
------------------------------------------------

CNN (_Convolutional neural networks_) merupakan salah satu terobosan besar dalam bidang pengolahan gambar. CNN menggunakan serangkaian _layer_ untuk secara bertahap memahami fitur-fitur yang semakin kompleks dari gambar. Tahapan ini memungkinkan komputer untuk belajar secara otomatis dari data gambar yang diberikan. Salah satu keunggulan utama CNN adalah kemampuannya dalam mengenali objek pada gambar, seperti kucing atau anjing dengan tingkat akurasi yang tinggi.

Arsitektur CNN mirip dengan membuat kue lapis yang kompleks bahwa setiap "lapisan" memiliki peran penting dalam memproses dan mengekstraksi fitur dari data gambar. Berikut adalah rangkuman tentang arsitektur CNN.

1.  **Input Layer**: Menerima data masukan dari dataset. Setiap neuron mewakili satu fitur dalam data.
    
2.  **Convolutional Layers**: Mengekstraksi fitur dari gambar melalui proses konvolusi. Ada CONV1D, CONV2D, dan CONV3D, tergantung pada dimensi data.
    
3.  **Activation Layers**: Menerapkan fungsi aktivasi non-linear ke output dari lapisan sebelumnya untuk memperkenalkan sifat non-linear ke jaringan.
    
4.  **Pooling Layer**: Mengurangi dimensi spasial dari representasi gambar dengan mengambil sampel dari area kecil dan menggabungkannya menjadi satu nilai, menggunakan max pooling atau average pooling.
    
5.  **Fully Connected Layers**: Terhubung dengan setiap neuron pada lapisan sebelumnya dan memiliki bobot yang dipelajari selama pelatihan untuk menghasilkan output akhir.
    
6.  **Output Layers**: Menghasilkan prediksi atau output akhir dari model, tergantung pada jenis tugas yang dilakukan oleh jaringan.
    

Dalam membangun model CNN, kita mempertimbangkan faktor-faktor, seperti jenis data, kompleksitas tugas, dan kebutuhan model untuk mempelajari pola dalam data. Terkadang, kita juga memasukkan lapisan-lapisan tambahan, seperti batch normalization, flatten, dan dropout untuk meningkatkan kinerja dan stabilitas model. 

Tahapan Klasifikasi Gambar
--------------------------

Berikut adalah rangkuman mengenai tahapan klasifikasi gambar.

### Pengumpulan Data

Pengumpulan data adalah langkah awal yang krusial dalam mempersiapkan model klasifikasi gambar. Berikut adalah beberapa sumber dan kriteria penting saat mencari dataset.

1.  **Mesin Pencari Gambar**: Google Images, Bing Images, atau Flickr menyediakan akses ke berbagai gambar dengan kata kunci tertentu. Pastikan untuk memeriksa hak cipta dan izin penggunaan.
    
2.  **Basis Data Publik**:
    
    *   ImageNet: Menyediakan jutaan gambar yang dianotasi untuk berbagai kategori.
        
    *   COCO (Common Objects in Context): Fokus pada objek-objek umum dalam konteks tertentu.
        
    *   Open Images Dataset: Proyek Google yang memberikan akses ke jutaan gambar dengan label yang bervariasi.
        
3.  **Kaggle**: Platform yang menyediakan dataset terstruktur dan berlabel untuk berbagai masalah machine learning, termasuk klasifikasi gambar.
    
4.  **UCI Machine Learning Repository**: Repositori terbuka yang menyediakan dataset untuk berbagai masalah machine learning, termasuk klasifikasi gambar.
    
5.  **Koleksi Pribadi**: Jika memiliki koleksi gambar yang sesuai, Anda dapat menggunakannya. Pastikan Anda memiliki hak untuk menggunakan gambar-gambar tersebut.
    
6.  **Kerja Sama dengan Ahli Domain**: Jika memungkinkan, bekerja sama dengan ahli domain untuk mendapatkan gambar-gambar yang relevan.
    

### Pemisahan Data _(Data Splitting)_

Pemisahan data, atau yang sering disebut sebagai _data splitting_, adalah proses penting dalam pengelolaan dataset gambar untuk proyek klasifikasi gambar. Tujuan utamanya adalah membagi dataset menjadi subset-subset yang berbeda untuk **pelatihan, validasi, serta pengujian model atau pelatihan dan pengujian model.** Setiap subset memiliki peranannya masing-masing dalam menghasilkan model yang baik dan diuji dengan benar.

Selain itu, penting untuk dicatat bahwa tidak ada satu proporsi pemisahan data yang cocok untuk semua situasi. Oleh karena itu, Anda bisa mencoba beberapa proporsi berbeda sebagai perbandingan untuk mengevaluasi pilihan yang paling optimal sesuai dengan karakteristik dataset dan kebutuhan proyek. 

### Pra-pemrosesan Data Gambar

Pra-pemrosesan data gambar adalah tahap krusial dalam mempersiapkan data sebelum dilatih dengan model. Ini melibatkan serangkaian langkah untuk meningkatkan kualitas dan relevansi data sehingga model dapat belajar secara efisien serta memberikan hasil yang lebih baik. 

Berikut adalah beberapa langkah umum dalam pra-pemrosesan data gambar.

1.  **Pembersihan Data**Identifikasi dan hapus gambar-gambar yang buram, kabur, atau tidak relevan. Ini membantu fokus pada fitur-fitur yang penting dan mengurangi gangguan.
    
2.  **Normalisasi**Mengubah rentang nilai piksel dalam gambar sehingga distribusinya seragam. Ini membantu mencegah masalah numerik dan mempercepat konvergensi saat pelatihan model.
    
3.  **Reduksi Dimensi**Penggunaan teknik reduksi dimensi, seperti PCA untuk mengurangi dimensi gambar, terutama jika dataset memiliki dimensi yang tinggi.
    
4.  **Augmentasi Data**Memperluas dataset tanpa mengumpulkan lebih banyak data aktual dengan menerapkan variasi pada citra-citra yang ada. Ini membantu mengatasi masalah "data hungry" dalam deep learning.Jenis-Jenis Metode Augmentasi Data.
    
    1.  **Flip**: Memutar posisi citra secara vertikal atau horizontal untuk memperoleh variasi.
        
    2.  **Translasi**: Pergeseran gambar ke arah horizontal atau vertikal untuk melatih model melihat objek dalam konteks yang berbeda.
        
    3.  **Zoom**: Memperbesar atau memperkecil gambar untuk melatih model melihat detail-detail kecil atau meningkatkan invariansi terhadap skala objek.
        
    4.  **Rotation**: Memutar gambar sejumlah derajat tertentu untuk mengenalkan variasi sudut pandang pada objek.
        
    5.  **Brightness Adjustment**: Mengubah tingkat kecerahan pada gambar untuk meningkatkan invariansi terhadap kondisi pencahayaan.
        
    6.  **Contrast Adjustment**: Meningkatkan atau mengurangi kontras gambar untuk mengatasi variasi tingkat kontras dalam gambar.
        
    7.  **Cropping**: Memotong atau menghapus bagian-bagian tertentu dari gambar untuk fokus pada fitur-fitur penting.
        
    8.  **Shearing**: Meregangkan atau melenturkan gambar dalam satu arah tertentu untuk mengenalkan distorsi geometris.
        
    9.  **Resolusi**: Memilih resolusi yang sesuai dengan kompleksitas tugas dan kebutuhan komputasi.
        
    10.  **Labeling**: Memastikan setiap gambar diberi label dengan benar sesuai dengan kategori atau kelas yang tepat.
        

Pra-pemrosesan data gambar membantu memastikan kualitas data yang baik dan mempersiapkan dataset untuk melatih model computer vision dengan efektif. Melalui langkah-langkah ini, model dapat belajar dengan baik dan menghasilkan hasil yang akurat dan konsisten.

### Pembuatan Model Klasifikasi Gambar dengan CNN

Memahami kompleksitas masalah klasifikasi gambar yang dihadapi adalah langkah penting dalam merancang arsitektur CNN dengan tepat. Misalnya, jika dataset memiliki gambar-gambar dengan fitur relatif sederhana dan jelas, arsitektur CNN yang lebih dangkal mungkin sudah cukup untuk melakukan klasifikasi secara baik. Namun, jika dataset memiliki gambar-gambar dengan fitur kompleks dan variasi besar, arsitektur CNN yang lebih dalam dan kompleks mungkin diperlukan untuk menggali fitur-fitur tersebut.

Penting untuk memperhatikan bahwa semakin dalam dan kompleks arsitektur CNN, semakin banyak parameter yang perlu diatur selama proses pelatihan. Ini dapat mengakibatkan waktu pelatihan lebih lama dan memerlukan sumber daya komputasi lebih besar. Oleh karena itu, penting untuk menyeimbangkan kompleksitas arsitektur dengan sumber daya yang tersedia dan batasan waktu yang dimiliki.

### Compile dan Fit Model

Setelah mendefinisikan arsitektur convolutional neural network (CNN), langkah berikutnya adalah compile dan melatih (_fit_) model tersebut. Proses ini melibatkan pemilihan optimizer, loss function, dan metrik evaluasi, serta pelatihan model menggunakan data yang telah disiapkan.

1.  **Compile Model**Compile model adalah langkah penting sebelum pelatihan. Dalam langkah ini, kita menentukan:
    
    *   Optimizer: Algoritma yang digunakan untuk meng-update bobot model berdasarkan gradient loss function.
        
    *   Loss Function: Fungsi yang digunakan untuk mengukur seberapa baik model memprediksi target.
        
    *   Metrics: Metrik yang digunakan untuk mengevaluasi performa model selama pelatihan dan validasi.
        
2.  **Melatih Model**Setelah model di-compile, kita melatih model menggunakan metode fit(). Proses ini melibatkan proses memasukkan data pelatihan dan validasi, serta menentukan parameter pelatihan, seperti jumlah epochs dan batch size.Dalam proses pelatihan model CNN, pemantauan dan pengaturan pelatihan model adalah kunci untuk memastikan model yang optimal. Dua komponen penting dalam proses ini adalah **ModelCheckpoint** dan **EarlyStopping callbacks.**
    
    *   **ModelCheckpoint**: Digunakan untuk menyimpan model dengan performa terbaik selama pelatihan.
        
    *   **EarlyStopping**: Digunakan untuk menghentikan pelatihan lebih awal jika tidak ada peningkatan dalam performa pada data validasi.
        

Jadi, proses pelatihan model CNN diinisiasi dan dijalankan dengan tujuan menghasilkan model yang optimal dalam mengklasifikasikan gambar.

### Evaluasi Model

Setelah melatih model CNN, evaluasi dilakukan untuk mengukur performanya pada data pengujian yang belum pernah dilihat. Ini penting untuk memastikan model dapat melakukan generalisasi dengan baik.

**Proses Evaluasi**

*   Metode: Menggunakan evaluate() pada model.
    
*   Generator: Menggunakan generator data pengujian.
    
*   Steps: Dihitung dari jumlah sampel pengujian dibagi ukuran batch.
    

**Hasil Evaluasi**

*   Loss: Menunjukkan kesalahan prediksi model.
    
*   Accuracy: Menunjukkan tingkat ketepatan prediksi model.
    

Penanganan Overfitting dalam Klasifikasi Gambar
-----------------------------------------------

Overfitting adalah masalah ketika model belajar terlalu detail dari data pelatihan, termasuk _noise_ yang tidak relevan sehingga performanya menurun pada data baru. Berikut adalah beberapa teknik untuk mengatasi overfitting.

1.  **Data Augmentation**Menciptakan variasi tambahan dari gambar pelatihan melalui rotasi, flipping, cropping, zooming, dan perubahan brightness. Ini membantu model menjadi lebih _robust_ dan _generalizable_.
    
2.  **Regularization**
    
    *   **Dropout:** Secara acak menonaktifkan neuron selama pelatihan untuk mencegah model bergantung pada neuron tertentu, membuat model lebih _robust_.
        
    *   **L2 Regularization (Weight Decay):** Menambahkan penalti pada bobot besar untuk membuat model lebih sederhana dan menghindari pembelajaran berlebih.
        
3.  **Early Stopping**Penghentian pelatihan saat performa pada set validasi mulai menurun, mencegah model belajar detail yang tidak relevan dari data pelatihan.
    
4.  **Menggunakan Model yang Lebih Sederhana**Cara yang dapat dilakukan sebagai berikut.
    
    *   Mengurangi jumlah layer atau neuron dalam jaringan.
        
    *   Menggunakan model pre-trained dengan fine-tuning minimal pada layer terakhir.
        
    *   Menurunkan resolusi gambar masukan.
        
5.  **Cross-Validation**Pembagian data pelatihan menjadi beberapa bagian dan pelatihan serta pengujian model secara bergantian. Ini memastikan model dapat bekerja dengan baik pada seluruh dataset.
    
6.  **Penggunaan Teknik Transfer Learning**Penggunaan model yang sudah dilatih pada dataset besar dan umum, seperti ImageNet, serta penyesuaian untuk tugas yang lebih spesifik dengan dataset yang lebih kecil.
    

Dengan penerapan teknik-teknik ini, model dapat menggeneralisasi lebih baik pada data baru, meningkatkan performa dan keandalan dalam klasifikasi gambar.

Pengenalan Transfer Learning
----------------------------

**Analogi Navigasi:** mirip seperti menggunakan aplikasi navigasi yang sudah memiliki peta lengkap, transfer learning menggunakan model yang sudah dilatih pada dataset besar dan umum, menghemat waktu dan usaha.

**Efisiensi:** menggunakan model pre-trained untuk menghindari kebutuhan melatih model dari awal; memanfaatkan pengetahuan yang sudah ada tentang fitur dasar, seperti tepi, bentuk, dan pola.

### Proses Transfer Learning

1.  **Menggunakan Model Pre-trained**: Gunakan model yang sudah dilatih pada dataset besar, seperti ImageNet (misalnya ResNet atau VGG).
    
2.  **Modifikasi Model**
    
    *   Remove Top Layers: Hapus lapisan atas yang digunakan untuk klasifikasi sebelumnya.
        
    *   Add New Layers: Tambahkan lapisan baru untuk tugas spesifik Anda.
        
3.  **Fine-Tuning**
    
    *   Training with New Data: Latih ulang model dengan dataset Anda, biarkan beberapa bagian menyesuaikan dengan data baru.
        
    *   Preserve Pre-trained Knowledge: Model menyesuaikan diri dengan data baru sambil mempertahankan pengetahuan yang sudah ada.
        

Transfer learning memungkinkan model untuk melakukan generalisasi dengan baik pada dataset kecil dan spesifik dengan menggunakan pengetahuan dari model yang dilatih dalam dataset besar.

Beberapa Model untuk Transfer Learning
--------------------------------------

Transfer learning memanfaatkan pengetahuan dari model yang sudah dilatih pada dataset besar, seperti ImageNet untuk menghemat waktu dan usaha dalam melatih model baru. Model pre-trained ini sudah mengenali fitur dasar dalam gambar sehingga tidak perlu memulai dari awal.

### Model Populer untuk Transfer Learning

Berikut adalah beberapa model untuk transfer learning yang populer.

1.  **VGG (Visual Geometry Group)**
    
    *   Arsitektur: Sederhana namun efektif, terdiri dari lapisan konvolusi, max pooling, dan fully connected.
        
    *   Versi Terkenal: VGG16 dan VGG19.
        
    *   Kelebihan: Kemampuan baik dalam mengenali berbagai objek.
        
2.  **ResNet (Residual Network)**
    
    *   Arsitektur: Sangat dalam dengan blok residual untuk pembelajaran efisien.
        
    *   Versi Terkenal: ResNet50, ResNet101, dan ResNet152.
        
    *   Kelebihan: Performa tinggi dalam pengenalan gambar.
        
3.  **Inception (GoogLeNet)**
    
    *   Arsitektur: Menggunakan modul Inception untuk ekstraksi fitur pada berbagai skala.
        
    *   Versi Terkenal: InceptionV3 dan InceptionV4.
        
    *   Kelebihan: Tingkat akurasi tinggi.
        
4.  **MobileNet**
    
    *   Arsitektur: Dirancang untuk aplikasi mobile dan perangkat dengan sumber daya terbatas.
        
    *   Versi Terkenal: MobileNetV1, MobileNetV2, dan MobileNetV3.
        
    *   Kelebihan: Ringan dan efisien, performa baik dalam pengenalan gambar.
        
5.  **Xception**
    
    *   Arsitektur: Berdasarkan Inception, menggunakan depthwise separable convolution.
        
    *   Kelebihan: Efisien secara komputasi.
        
6.  **DenseNet**
    
    *   Arsitektur: Koneksi langsung antara setiap lapisan, mengurangi hilangnya informasi.
        
    *   Versi Terkenal: DenseNet121, DenseNet169, dan DenseNet201.
        
    *   Kelebihan: Performa baik dalam pengenalan gambar.
        

### Proses Transfer Learning

1.  **Modifikasi Model**Gunakan model pre-trained, hapus lapisan klasifikasi teratas, dan tambahkan lapisan baru yang sesuai dengan tugas klasifikasi spesifik.
    
2.  **Fine-Tuning**Latih ulang model dengan dataset Anda sendiri, menyesuaikan beberapa bagian model sementara mempertahankan pengetahuan yang ada.Melalui penggunaan model-model ini untuk transfer learning, kita dapat meningkatkan kinerja model lebih efisien, bahkan dengan dataset yang lebih kecil.