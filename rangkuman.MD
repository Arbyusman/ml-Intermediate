Rangkuman Kelas
---------------

Rangkuman Pengenalan Deep Learning
----------------------------------

### Dasar-Dasar Neural Network

Pada zaman komputasi modern ini, neural network telah menjadi salah satu komponen inti dari kecerdasan buatan. Konsep ini terinspirasi dari jaringan saraf biologis manusia dan dapat mengubah cara komputer belajar dalam berbagai tugas kompleks.  

### Taksonomi AI

Taksonomi AI menggambarkan evolusi konsep dan teknologi dalam bidang kecerdasan buatan, mulai dari artificial intelligence hingga deep learning (DL).

1.  **Artificial Intelligence (AI)**Pada tingkat paling dasar, AI mencakup penggunaan komputer atau mesin untuk melakukan tugas yang membutuhkan kecerdasan manusia, seperti pengambilan keputusan, pengenalan pola, dan pemecahan masalah.
    
2.  **Machine Learning (ML)**Cabang AI, yakni komputer belajar dari data tanpa pemrograman eksplisit, mengenal pola, dan membuat prediksi.
    
3.  **Neural Network (NN)**Model yang terinspirasi dari jaringan saraf manusia, terdiri dari neuron buatan dalam lapisan-lapisan yang memproses dan belajar dari data.
    
4.  **Deep Learning (DL)**Subbidang ML, yakni penggunaan neural network dengan banyak lapisan untuk memahami data yang lebih kompleks. DL telah memajukan pengenalan gambar, pemrosesan bahasa alami, dan aplikasi AI lainnya.
    

### Struktur Artificial Neural Network

Neural network yang paling sederhana atau minimal terdiri dari satu unit perceptron tunggal, juga dikenal sebagai single perceptron. Perceptron ini memproses input dengan mengalikan nilai input (x) dengan bobot (w), kemudian menjumlahkannya dengan bias (b). Hasil dari operasi ini disebut net input (z) dan kemudian akan diproses melalui fungsi aktivasi (f) untuk menghasilkan output (y) dari perceptron tersebut. 

### Cara Kerja Artificial Neural Network

Cara kerja artificial neural network (ANN) mengambil inspirasi dari struktur jaringan saraf manusia. Pada sebuah ANN, ada jutaan atau bahkan miliaran "neuron" buatan yang terorganisir dalam lapisan-lapisan. Setiap neuron menerima input dari neuron-neuron dalam lapisan sebelumnya, melakukan operasi matematika pada input ini, dan menghasilkan output yang akan diteruskan ke neuron-neuron dalam lapisan berikutnya.

Mirip dengan kerja jaringan saraf manusia, setiap koneksi antar neuron dalam ANN memiliki bobot atau nilai yang memengaruhi pentingnya informasi dari neuron sebelumnya. Selama proses pembelajaran, bobot-bobot ini diatur ulang agar ANN dapat belajar memahami pola-pola yang ada dalam data.

### Perceptron

Perceptron adalah unit dasar dalam neural network yang memproses input untuk menghasilkan output. Input diberi bobot masing-masing dan ditambah dengan bias. Hasil ini kemudian diproses melalui fungsi aktivasi untuk menghasilkan output yang dibutuhkan. Perceptron sendiri kurang efektif untuk tugas kompleks, tetapi ketika banyak perceptron dihubungkan dalam jaringan, mereka bisa memproses data dengan lebih baik.

### Neural Network

Neural network adalah kumpulan dari banyak perceptron yang saling terhubung. Setiap perceptron melakukan komputasi dengan inputnya sendiri, lalu informasi dari satu perceptron mengalir ke yang lain, memungkinkan jaringan untuk mempelajari pola kompleks dalam data. Kemampuan menyesuaikan bobot dan bias selama pelatihan membuat neural network sangat akurat dan adaptif terhadap masalah rumit.

Berikut adalah komponen dari perceptron dan fungsinya.

1.  Input (xi): Ini menerima angka-angka sebagai masukan.
    
2.  Bobot atau weights (wi) dan bias (w0): Setiap input dikalikan dengan bobot masing-masing dan ditambah dengan bias.
    
3.  Penjumlahan atau sum (∑): Hasil penjumlahan ini disebut weighted sum.
    
4.  Fungsi aktivasi atau non linearity function (⎰): Weighted sum diproses melalui fungsi aktivasi untuk menyesuaikan nilai hasil.
    
5.  Output (y): Ini menghasilkan bilangan numerik sebagai output.
    

Fungsi matematis perceptron adalah keluaran (ŷ) yang merupakan bias (w0) ditambah jumlah dari setiap input (xi) dikali dengan bobot masing-masing (wi), kemudian diproses oleh fungsi aktivasi (g).

Dengan jaringan neural network yang lebih besar dan kompleks, performanya dapat terus meningkat, menjadikannya alat efektif untuk berbagai aplikasi, seperti pengenalan pola, klasifikasi, dan prediksi.

### Multilayer Perceptron

Multilayer Perceptron (MLP) atau feedforward neural network adalah jenis neural network yang terdiri dari banyak perceptron (neuron) yang terhubung dalam beberapa lapisan. MLP memiliki tiga jenis lapisan utama.

1.  **Input Layer**
    
    *   Fungsi: Menerima data atau input dari luar.
        
    *   Struktur: Setiap neuron mewakili satu fitur atau variabel dari data yang masuk.
        
2.  **Hidden Layer**
    
    *   Fungsi: Memproses input dari input layer dengan operasi matematika menggunakan bobot (weights) dan fungsi aktivasi.
        
    *   Struktur: Terdiri dari satu atau lebih lapisan yang berada antara input layer dan output layer. Berfungsi sebagai penyaring atau extractor fitur untuk mempelajari pola-pola kompleks dalam data.
        
3.  **Output Layer**
    
    *   Fungsi: Menghasilkan output berdasarkan hasil pemrosesan oleh hidden layer.
        
    *   Struktur: Jumlah neuron bergantung pada tipe tugas. Untuk klasifikasi biner, output layer mungkin memiliki satu neuron yang menghasilkan nilai antara 0 dan 1. Untuk klasifikasi multiclass, setiap neuron bisa mewakili probabilitas kelas tertentu.
        

MLP memungkinkan jaringan neural untuk mempelajari dan memproses pola kompleks dalam data, menjadikannya alat yang efektif dalam berbagai aplikasi, seperti pengenalan pola, klasifikasi, dan prediksi.

### Terms pada Neural Network

Inilah beberapa istilah umum yang penting dalam pengembangan kecerdasan buatan menggunakan neural network, yaitu activation function, loss function, dan optimizer.

Berikut adalah rangkuman tentang beberapa istilah penting dalam pengembangan neural network.

1.  **Activation Function (Fungsi Aktivasi)**Fungsi aktivasi adalah fungsi matematika yang menentukan neuron akan aktif atau tidak berdasarkan inputnya. Fungsi ini memungkinkan jaringan saraf mengenali pola non-linier dalam data. Ada dua jenis utama fungsi aktivasi, yaitu linear dan non-linear.Inilah jenis-jenis fungsi aktivasi.
    
    *   **Linear:** Output proporsional secara linear terhadap input. Jarang digunakan pada hidden layer karena tidak bisa menangani non-linearitas.
        
    *   **ReLU (Rectified Linear Activation):** Output adalah input jika positif atau nol jika negatif. Sederhana dan efisien, sering digunakan pada hidden layer.
        
    *   **Leaky ReLU:** Modifikasi ReLU yang memperkenalkan gradien kecil pada bagian negatif untuk mencegah "neuron mati".
        
    *   **Sigmoid:** Mengubah input menjadi nilai antara 0 dan 1, cocok untuk klasifikasi biner, tetapi rentan terhadap gradien yang menghilang.
        
    *   **Tanh:** Mengubah input menjadi nilai antara -1 dan 1, lebih simetris dibanding sigmoid dan sering digunakan pada hidden layer.
        
    *   **Softmax:** Mengubah input menjadi distribusi probabilitas, digunakan pada output layer untuk klasifikasi multiclass.
        
2.  **Loss Function**Loss function mengukur seberapa baik atau buruk kinerja model pada data pelatihan dengan memberikan representasi numerik tentang kesalahan prediksi. Berikut contoh umumnya.
    
    *   **Mean Square Error (MSE):** Mengukur rata-rata dari kuadrat selisih antara prediksi model dan nilai sebenarnya.
        
    *   **Cross-Entropy Loss:** Umum digunakan untuk klasifikasi, mengukur perbedaan antara distribusi prediksi dan distribusi target.
        
3.  **Optimizer**Optimizer adalah komponen yang mengoptimalkan bobot dan bias jaringan untuk mengurangi kesalahan prediksi dengan cara memperbarui parameter berdasarkan gradien dari loss function. Fungsi utama optimizer adalah untuk menghitung gradien dan memperbarui parameter. Berikut adalah contoh optimizer.
    
    *   **Stochastic Gradient Descent (SGD):** Ini menggunakan gradien dari subset data untuk memperbarui parameter.
        
    *   **RMSprop:** Ini menyesuaikan learning rate untuk setiap parameter berdasarkan sejarah gradien.
        
    *   **Adam:** Optimizer adaptif yang menggabungkan momentum dan RMSprop untuk mengatur learning rate secara adaptif.
        

Pemilihan optimizer memengaruhi kecepatan konvergensi, kualitas model, dan kemampuan untuk menghindari masalah optimisasi, seperti “terjebak” dalam optimum lokal atau gradien yang menghilang.

### Forward Propagation dan Backpropagation

#### Forward Propagation

Forward propagation adalah proses menghitung output dari neural network berdasarkan input yang diberikan. Berikut adalah langkah-langkah dalam forward propagation.

1.  **Input Data**Data dimasukkan ke jaringan, bisa berupa gambar (piksel), teks (token), atau nilai numerik (fitur seperti luas tanah atau jumlah kamar).
    
2.  **Neuron dan Bobot**Setiap neuron menerima input yang dikalikan dengan bobotnya dan ditambahkan bias. Bobot menentukan seberapa penting input tersebut, kemudian bias membantu neuron untuk tetap aktif dalam berbagai kondisi.
    
3.  **Perhitungan di Neuron**Hasil perkalian input dan bobot ditambah bias dimasukkan ke fungsi aktivasi (seperti ReLU atau sigmoid). Fungsi aktivasi menentukan bahwa neuron tersebut aktif atau tidak.
    
4.  **Output**Aktivasi dari neuron pada lapisan sebelumnya menjadi input untuk neuron dalam lapisan berikutnya, berulang hingga mencapai lapisan output yang menghasilkan prediksi akhir.
    

#### Backpropagation

Backpropagation adalah proses mengoptimalkan bobot dan bias jaringan untuk meminimalkan error pada prediksi. Berikut adalah langkah-langkah dalam backpropagation.

1.  **Perhitungan Error**Output prediksi dibandingkan dengan nilai target sebenarnya menggunakan fungsi kerugian (loss function), seperti mean squared error (MSE) atau cross-entropy loss.
    
2.  **Backward Pass**Penghitungan gradien dari loss function terhadap setiap bobot menggunakan aturan rantai (_chain rule_). Gradien menunjukkan kontribusi setiap bobot terhadap total error.
    
3.  **Perubahan Bobot**Bobot diperbarui dengan menggerakkannya melawan arah gradien menggunakan algoritma optimasi, seperti gradient descent. Laju pembelajaran (learning rate) menentukan seberapa besar perubahan bobot dalam setiap iterasi.
    
4.  **Iterasi**Langkah forward propagation, perhitungan error, backward propagation, dan optimasi bobot diulang untuk setiap batch data latihan hingga bobot konvergen ke nilai optimal. Proses ini melibatkan banyak iterasi (_epochs_) untuk memastikan model belajar dari data secara efektif. 
    

Dengan forward propagation, jaringan menghasilkan prediksi berdasarkan input, sedangkan backpropagation mengoptimalkan bobot untuk mengurangi kesalahan prediksi. Kombinasi keduanya memungkinkan neural network belajar dari data dan meningkatkan akurasinya secara iteratif.

### Definisi Deep Learning

Deep learning adalah cabang dari kecerdasan buatan yang menggunakan algoritma terinspirasi dari cara otak manusia bekerja. Metode ini diimplementasikan melalui jaringan saraf tiruan yang disebut artificial neural networks (ANN).

Keunggulan utama deep learning terletak pada kemampuannya untuk belajar secara mandiri dari data besar dan kompleks. Proses pembelajaran melibatkan penyesuaian bobot dan parameter jaringan secara iteratif melalui proses pelatihan, yakni ketika model diuji dan diperbaiki berdasarkan umpan balik dari data.

Aplikasi dan Metode dalam Deep Learning

1.  **Convolutional Neural Networks (CNNs):** Ini digunakan untuk analisis gambar. CNNs efektif dalam mendeteksi fitur visual dan pola dalam gambar.
    
2.  **Recurrent Neural Networks (RNNs):** Cocok untuk data berurutan, seperti teks atau sinyal suara. RNNs mempertimbangkan konteks temporal atau urutan data.
    

Tantangan dalam Deep Learning

1.  Pelatihan model deep learning membutuhkan data dalam jumlah besar untuk menghasilkan prediksi yang akurat.
    
2.  Mengatur parameter model yang kompleks memerlukan pemahaman mendalam dan sering kali eksperimen berulang.
    

Deep learning membawa terobosan besar dalam berbagai bidang, yaitu pengenalan wajah, mobil otonom, penelitian medis, dan banyak lagi. Dengan deep learning, kita dapat membuat komputer "belajar" dari data besar untuk membuat prediksi yang lebih cerdas dan akurat, mirip seperti cara manusia belajar dari pengalaman.

### Arsitektur Deep Learning

Arsitektur deep learning adalah struktur jaringan saraf buatan yang kompleks dan terdiri dari berbagai lapisan yang memproses data masukan dan menghasilkan output. Setiap lapisan dalam arsitektur memiliki fungsi khusus dan bertanggung jawab untuk mengekstrak fitur-fitur yang semakin abstrak dan kompleks. Dengan kedalaman lebih besar, arsitektur deep learning dapat mempelajari pola yang lebih rumit dari data dan memberikan hasil lebih baik.

#### Jenis-Jenis Layer dalam Arsitektur Deep Learning

1.  **Input Layer**Input layer adalah bagian pertama dari jaringan neural yang menerima data masukan, seperti gambar, teks, atau data numerik lainnya. Fungsi utamanya adalah meneruskan data masukan ke lapisan-lapisan selanjutnya dalam jaringan.
    
2.  **Hidden Layer**Hidden layers adalah lapisan-lapisan antara input layer dan output layer yang bertugas mengekstrak fitur-fitur dari data masukan.Berikut adalah jenis-jenis hidden layers yang umum digunakan.
    
    *   **Fully Connected Layer (Dense Layer)**: membantu dalam mempelajari hubungan yang kompleks antara fitur-fitur input.
        
    *   **Convolutional Layer (Conv Layer)**: digunakan dalam convolutional neural networks (CNNs) untuk pengenalan gambar atau segmentasi objek.
        
    *   **Batch Normalization Layer**: digunakan untuk mempercepat konvergensi pelatihan dengan memungkinkan penggunaan learning rate yang lebih tinggi.
        
    *   **Recurrent Layer (RNN, LSTM, GRU)**: digunakan untuk memproses data berurutan, seperti teks, audio, atau video.
        
    *   **Dropout Layer**: digunakan di antara lapisan-lapisan tersembunyi untuk membuat jaringan lebih _robust_ dan mengatasi _overfitting_.
        
    *   **Pooling Layer**: digunakan setelah convolutional layers dalam CNN untuk mengurangi _overfitting_ dan menghemat komputasi.
        
    *   **Flatten Layer**: digunakan untuk mengubah representasi data spasial menjadi representasi linear.
        
    *   **Output Layer**: digunakan untuk lapisan terakhir dalam jaringan neural yang menghasilkan prediksi atau output akhir berdasarkan data yang telah diproses oleh hidden layers.
        

Hidden layers memiliki peran krusial dalam pembelajaran jaringan neural. Setiap jenis layer memiliki karakteristik dan fungsi khusus untuk membantu jaringan mempelajari representasi yang lebih abstrak dari data. Kombinasi yang tepat dari hidden layers dalam arsitektur jaringan neural memungkinkan jaringan untuk belajar dan menggeneralisasi pola kompleks dari data; ini menghasilkan prediksi yang akurat.

### Pengenalan Arsitektur Deep Learning yang Populer 

Arsitektur deep learning terdiri dari berbagai struktur jaringan saraf buatan dirancang untuk memproses dan mentransformasikan data masukan menjadi keluaran yang diinginkan. Beberapa arsitektur populer yang digunakan dalam deep learning sebagai berikut.

1.  **Convolutional Neural Network**Convolutional neural network (CNN) dirancang khusus untuk memproses data gambar dan visual. CNN terdiri dari lapisan konvolusi yang menggunakan filter untuk mengekstrak fitur-fitur lokal dari gambar; lapisan pooling untuk mengurangi dimensi spasial; lapisan aktivasi, seperti ReLU, untuk memperkenalkan non-linearitas; dan lapisan fully connected untuk klasifikasi akhir berdasarkan fitur yang diekstraksi. CNN sering digunakan untuk pengenalan gambar dan objek, klasifikasi citra, dan segmentasi gambar.
    
2.  **Recurrent Neural Network**Recurrent neural network (RNN) dirancang untuk memproses data berurutan, seperti teks, audio, atau data time series. RNN memiliki loop rekursif yang memungkinkan jaringan untuk mengingat informasi dari iterasi sebelumnya. Variasi canggih dari RNN, seperti LSTM dan GRU, memiliki sel memori yang memungkinkan jaringan untuk mengingat informasi dalam jangka panjang. RNN umum digunakan dalam pemrosesan bahasa alami, pengenalan suara, dan prediksi time series.
    
3.  **Long Short-Term Memory**Long short-term memory (LSTM) adalah jenis RNN dengan mekanisme gate untuk mengatasi masalah hilangnya informasi jangka panjang. LSTM memiliki gate, seperti forget gate untuk melupakan informasi tidak relevan dan input gate untuk mengontrol aliran informasi baru yang disimpan dalam memori jangka panjang. LSTM digunakan dalam pemrosesan bahasa alami yang memerlukan pemahaman konteks lebih dalam, seperti generasi teks alami dan pengenalan wicara.
    
4.  **Generative Adversarial Network**Generative adversarial network (GAN) terdiri dari dua jaringan neural berlawanan, yaitu generator dan diskriminator. Generator menghasilkan data sintetis dari distribusi laten, sementara diskriminator mencoba membedakan antara data asli dan sintetis. GAN digunakan untuk menghasilkan gambar sintetis, augmentasi dataset, dan aplikasi kreatif lainnya.
    
5.  **Transformer**Transformer adalah arsitektur berbasis atensi yang digunakan terutama dalam pemrosesan bahasa alami untuk mengatasi masalah ketergantungan jarak panjang. Transformer menggunakan mekanisme _self-attention_. Ini memungkinkan model memberikan bobot yang tepat pada kata-kata penting dalam teks. Ia juga memiliki blok encoder dan decoder untuk tugas seperti penerjemahan mesin dan pemodelan bahasa.
    
6.  **Autoencoder**Autoencoder adalah arsitektur yang digunakan untuk reduksi dimensi atau generasi data sintetis. Autoencoder terdiri dari encoder yang menghasilkan representasi tersembunyi dari data input dan decoder yang memulihkan data asli dari representasi tersembunyi. Autoencoder digunakan untuk reduksi dimensi data, denoising, dan menghasilkan data sintetis.Arsitektur-arsitektur ini telah membuka berbagai kemungkinan dalam pemrosesan data yang kompleks dan memungkinkan deep learning untuk mencapai hasil luar biasa dalam berbagai bidang aplikasi.
    

### Pengenalan Convolutional Neural Network

Convolutional neural network (CNN) adalah tipe jaringan saraf yang umum digunakan untuk memproses data gambar. CNN digunakan untuk mendeteksi dan mengenali objek dalam gambar, terinspirasi dari cara manusia memproses informasi visual. 

Secara umum, CNN memiliki struktur mirip seperti jaringan saraf biasa, dengan neuron yang memiliki bobot, bias, dan fungsi aktivasi. Namun, pembeda CNN dengan lainnya adalah lapisan konvolusi, terdiri dari neuron-neuron yang tersusun dalam filter dengan dimensi panjang dan tinggi (piksel).

Berikut adalah langkah-langkah CNN bekerja.

1.  Memecah gambar menjadi bagian-bagian lebih kecil atau jendela-jendela gambar yang disebut "patches”.
    
2.  Memasukkan setiap gambar yang lebih kecil ke jaringan saraf yang lebih sederhana (small neural network).
    
3.  Menyimpan hasil dari masing-masing gambar kecil yang telah melewati proses konvolusi pada sebuah array baru. 
    
4.  Pengurangan dimensi atau resolusi dari representasi fitur yang telah diperoleh.
    
5.  Membuat prediksi berdasarkan representasi fitur.
    

### Pengenalan Recurrent Neural Network

Recurrent neural network (RNN) adalah jenis arsitektur jaringan saraf yang dirancang untuk memproses data berurutan, yakni ketika hubungan antar elemen dalam urutan memiliki arti atau konteks temporal. RNN biasanya digunakan pada data teks (sekuens kata), audio (gelombang suara), deret waktu (data berurutan terkait waktu), dan lainnya. Keunggulan utama RNN adalah kemampuannya untuk "mengingat" atau mempertahankan informasi tentang sejarah (konteks) dari urutan data yang diproses.

Ada empat tipe RNN berdasarkan panjang input dan output yang berbeda.

1.  One-to-one adalah jaringan neural sederhana yang umum digunakan untuk masalah pembelajaran mesin dengan satu input dan satu output.
    
2.  One-to-many memiliki satu input dan banyak output. Ini biasanya digunakan untuk menghasilkan deskripsi gambar.
    
3.  Many-to-one mengambil urutan multiple inputs dan memprediksi satu output. Populer dalam klasifikasi sentimen, yaitu ketika inputnya berupa teks dan output-nya adalah kategori.
    
4.  Many-to-many menggunakan multiple inputs dan outputs. Aplikasi paling umumnya adalah terjemahan mesin.
    

Berikut adalah langkah-langkah RNN bekerja.

1.  RNN menerima input berurutan, seperti kata-kata dalam sebuah kalimat atau frame pada video. Setiap elemen input direpresentasikan dengan vektor fitur numerik. 
    
2.  Setiap unit (_neuron_) dalam RNN menghitung aktivasi berdasarkan input saat ini dan status internal (_state_) dari unit pada waktu sebelumnya. 
    
3.  Setiap unit RNN memiliki status internal yang menyimpan informasi dari elemen-elemen sebelumnya dalam urutan data.
    
4.  Pada setiap langkah waktu, RNN menghasilkan output berdasarkan aktivasi saat ini atau status internal terakhir.
    

Rangkuman Membuat dan Melatih Neural Network dengan TensorFlow dan Keras
------------------------------------------------------------------------

### Pengenalan TensorFlow dan Keras untuk Deep Learning

TensorFlow dan Keras merupakan framework yang sangat terkenal di kalangan praktisi machine learning, tetapi hal ini bukan berarti framework lainnya kurang bagus, ya. Hasil ini merupakan riset yang dilakukan oleh Jeff Hale pada tahun 2018 mengenai deep learning. Riset tersebut menggunakan 11 sumber data pada 7 kategori yang berbeda untuk mengukur popularitas _framework_ berdasarkan ketertarikan pengguna. Hasilnya TensorFlow menang telak, bukan? Hal ini terjadi karena kedua framework ini memiliki beberapa kelebihan, seperti _Open-source_, mudah untuk _debugging_, _compatibility_ yang baik, _scalability_ yang fleksibel, komunitas yang luas dan masih banyak lagi. 

Dengan demikian, tentu Anda semakin bersemangat dan penasaran untuk mempelajari materi ini. Supaya tidak makin penasaran, mari kita mulai perjalanan yang romantis dengan TensorFlow dan Keras.

#### TensorFlow 

TensorFlow (TF) adalah _end-to-end open source platform_ yang dikembangkan oleh Google Brain dan sangat populer untuk pengembangan machine learning berskala besar. TensorFlow memiliki ekosistem tools, library, dan sumber daya komunitas yang komprehensif dan fleksibel, sehingga memungkinkan para peneliti dan pengembang membangun serta menerapkan aplikasi machine learning dengan mudah.

Secara umum, TensorFlow memiliki banyak kelebihan seperti yang sudah disebutkan di atas. Tentunya Anda penasaran terkait kelebihan tersebut, bukan? Mari kita bahas kelebihan TensorFlow satu per satu agar Anda lebih terpacu untuk menyelesaikan misi menjadi praktisi machine learning yang andal.

1.  _Open-source_Sebagai sebuah _frameworkopen-source_ tentunya penggunaan TensorFlow tidak mengeluarkan biaya dan bisa digunakan oleh semua orang mulai dari pelajar, guru, dosen, peneliti, data scientist, machine learning engineer, dan lainnya. Selain itu, hal ini juga memungkinkan untuk menggunakan TensorFlow kapan saja serta di mana saja sesuai kebutuhan pengguna tanpa harus memikirkan pengeluaran sedikit pun.
    
2.  _Scalability_Hingga saat ini, TensorFlow tidak terbatas hanya pada satu _platform_ saja. Kelebihan ini tentu menguntungkan bagi pengguna karena kita dapat membangun sebuah sistem AI menggunakan TensorFlow di berbagai platform dengan komputasi atau performa yang sama. Selain itu, model yang dihasilkan TensorFlow juga dapat menyesuaikan komputasi yang digunakan berdasarkan jumlah _requests_. Sangat menarik, bukan? 
    
3.  _Compatibility_Saat ini, kompatibilitas/kecocokan merupakan salah satu faktor yang paling penting. Nah, pada kasus ini, TensorFlow kompatibel dengan berbagai macam bahasa pemrograman, seperti Python, C++, JavaScript, Kotlin, dan lain sebagainya.
    
4.  _Parallelism_Hal krusial lainnya yang mampu ditangani TensorFlow adalah _hardware acceleration_ Mungkin sebagian dari Anda bertanya, “Apa itu _hardware acceleration_?” Ini merupakan sebuah library yang memberikan TensorFlow kemampuan untuk membagikan ketersediaan hardware seperti CPU atau GPU pada proses pelatihan maupun prediksi.
    
5.  _Graph_Untuk meningkatkan pengalaman developer ketika membangun sebuah machine learning, tentunya kita juga memerlukan pengukuran yang lebih mudah dengan menggunakan visualisasi. Hal itu akan meringankan beban kognitif yang dibebankan kepada otak kita. Setelah memikirkan banyak hal pada setiap tahapan pembangunan machine learning, tentunya kita juga memerlukan sebuah alat yang dapat mempermudah perhitungan performa model.
    
6.  _Architectural Support_TensorFlow didukung oleh beberapa hardware yang dapat melakukan proses pelatihan, mulai dari CPU, GPU, hingga TPU. Pada tahap eksplorasi, CPU dapat dikatakan sangat cukup untuk melakukan pelatihan machine learning maupun deep learning. Namun, untuk beberapa kasus seperti dataset yang sangat besar atau data unstructured (gambar, suara, video, dan lain sebagainya), GPU akan memproses pelatihan dengan lebih cepat. Hal ini dikarenakan GPU memiliki sebuah arsitektur yang dapat melakukan proses yang sangat banyak secara bersamaan.
    
7.  _Library Management_Sebagai salah satu framework yang dikembangkan oleh Google, tentunya TensorFlow memiliki update yang sangat baik. TensorFlow sendiri melakukan pembaruan dalam waktu yang sangat cepat agar dapat memberikan pengalaman yang maksimal kepada seluruh developernya. Hingga saat ini, pembaruan TensorFlow masih terus dikembangkan. Hal ini dibuktikan dengan rilisnya versi 2.16.1 pada 8 Maret 2024. Tentunya dengan pembaruan ini membuat para praktisi machine learning tidak perlu merasa takut dengan framework yang deprecated sehingga kreatifitas developer bisa tetap tersalurkan..
    

Kelebihan di atas merupakan _highlight_ yang perlu kita perhatikan. Selain itu, masih ada banyak sekali kelebihan TensorFlow yang akan Anda rasakan ketika membangun model machine learning menggunakan framework tersebut. Sampai di sini tentunya Anda sudah paham alasan TensorFlow menjadi sangat populer di kalangan praktisi machine learning, ‘kan?

#### Keras

Keras adalah API untuk mengembangkan jaringan saraf tiruan. Dengan Keras, kita akan lebih mudah dalam membuat sebuah _multilayer perceptron_ dan _convolutional neural network_. Aplikasi dari Keras sangat luas dan memungkinkan kita untuk membangun jaringan saraf tiruan dengan tujuan klasifikasi gambar, pemrosesan bahasa alami, pengenalan suara, dan prediksi _time series_.

Komponen inti pembangun sebuah jaringan saraf tiruan dalam Keras adalah layer. Sebuah layer pada Keras, sama dengan sebuah layer pada MLP yang memiliki beberapa perceptron. Terdengar sangat kompleks, bukan? Namun, penggunaan Keras saat ini sangatlah mudah.

### Pra-pemrosesan Data untuk Model

Tahap pemrosesan data merupakan perubahan dari data mentah yang dibersihkan dan diatur untuk tahap pemrosesan berikutnya. Selama tahapan pemrosesan data, data mentah harus diperiksa dengan sangat cermat agar kita dapat memahami karakteristik dataset yang akan dilatih.

Dataset untuk setiap masalah tentunya berbeda. Contohnya pada dataset untuk klasifikasi gambar dan dataset untuk pemrosesan bahasa alami atau NLP. Pada dataset untuk klasifikasi gambar, sampelnya berupa kumpulan gambar atau matriks hasil representasi sebuah gambar seperti gambar berikut. 

Berbeda dengan dataset NLP, sampelnya tentu berupa kalimat-kalimat yang terdiri dari sejumlah kata tertentu seperti gambar di bawah.

Tidak seperti manusia yang bisa mengenali gambar atau memahami kalimat secara langsung, kita perlu melakukan pemrosesan dahulu agar data tersebut siap diterima oleh model. 

Secara umum, ada empat tahapan yang perlu kita lakukan dalam memproses data.

1.  Ubah dataset ke dalam bentuk larik/array. _Yup_, larik berisi angka-angka adalah format data yang dapat diterima oleh model kita. Sama seperti pada kelas Belajar Machine Learning untuk Pemula, model kita menerima gambar sebagai matriks atau larik 2 dimensi.
    
2.  Pisahkan atribut dan label pada data. Model kita akan mempelajari korelasi antara atribut dan label pada dataset.
    
3.  Ubah skala data dalam skala yang seragam. Nama teknik ini adalah normalization. Normalization dilakukan karena NN akan memproses nilai yang berada di antara 0 dan 1  sehingga membuat komputasi lebih optimal.
    
4.  Terakhir, pisahkan dataset ke dalam data latih dan data uji. Betul, kita memerlukan data uji untuk mengevaluasi kinerja dari model yang telah kita latih.
    

### Menggunakan Model untuk Melakukan Prediksi

Anda dapat melakukan prediksi dengan menggunakan kode berikut.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   model.predict([4, 5])   `

Ketika kita menjalankan kode di atas, hasil yang kita dapat seharusnya adalah 13 dan 14 di mana f(4) = 4 + 9 dan f(5) = 5 + 9. Namun, ketika kita menjalankan kode tersebut, output yang dihasilkan adalah seperti di bawah ini.

1/1 \[==============================\] - 0s 40ms/step

array(\[\[12.999903\],

       \[13.999887\]\], dtype=float32)

Jika Anda amati secara saksama, nilai yang dihasilkan ketika menjalankan fungsi prediksi hanya mendekati angka 13 dan 14 tidak 100% presisi. Kenapa demikian? Karena neural  network tidak memprediksi kepastian melainkan menghitung probabilitas yang terjadi. Pada kasus kita, neural network mempelajari bahwa pola yang terdapat pada dataset kemungkinan adalah x + 9 sehingga prediksi yang dihasilkan adalah probabilitas yang mendekati angka 13 dan 14. Semakin banyak data yang dilatih maka tingkat error training juga semakin rendah sehingga prediksi dari neural network akan semakin mendekati 13 dan 14.

Karena kita memiliki nilai loss yang sangat kecil, Anda dapat menggunakan fungsi **.round()** agar mengembalikan nilai dengan lebih presisi. Namun, tentunya ini akan menjadi resiko ketika kita memiliki loss function yang besar karena akan menjadi _noise_ pada hasil prediksi yang kita lakukan sehingga hasilnya akan mengembalikan nilai sesuai dengan input yang sebelumnya kita latih.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   model.predict([4, 5]).round()######################Output1/1 [==============================] - 0s 41ms/steparray([[13.],       [14.]], dtype=float32)   `

Hasil yang diberikan pada kode di atas sangat membuat developer lega karena dapat menghitung fungsi dengan sangat baik. Ke depannya, ketika Anda mendapatkan soal yang sama dengan jumlah yang sangat banyak, cukup panggil fungsi predict, lalu model machine learning akan mengembalikan nilai sesuai dengan jawabannya. 

### Model Sekuensial dengan Beberapa Layer

Pada kode di bawah, kita memanggil fungsi dense sebanyak empat kali yang menunjukkan bahwa model kita memiliki empat buah layer. Layer pertama hanya memiliki 20 buah perceptron, layer kedua memiliki 15 buah perceptron, layer ketiga memiliki tiga buah perceptron, dan layer terakhir memiliki satu buah perceptron. Ingat, layer pertama dari model sequential harus memiliki parameter input\_shape agar model bisa mengenali bentuk input yang akan diterimanya.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   model = tf.keras.Sequential([    tf.keras.layers.Dense(units=20, input_shape=[1]),    tf.keras.layers.Dense(units=15),    tf.keras.layers.Dense(units=10),    tf.keras.layers.Dense(units=1)    ])   `

Selanjutnya, mari kita lakukan pelatihan sesuai dengan materi sebelumnya sehingga menghasilkan loss seperti berikut.

Silakan coba kode di atas pada latihan yang telah kita kerjakan pada materi sebelumnya dan lihat perbedaannya. Lalu, mari kita bandingkan loss yang dihasilkan ketika menggunakan satu buah layer dan empat buah layer pada tabel berikut.

**Satu Layer**

**Empat Layer**

Loss

2.6231e-07

2.0464e-13

Loss

0.00000026231

0.00000000000020464

Perhatikan tabel di atas, tentunya dengan cepat kita dapat melihat perbedaan loss dari kedua kasus tersebut. Sekarang, Anda dapat membuat sebuah model neural network dengan jumlah layer lebih dari satu. Selanjutnya, lakukanlah eksplorasi mandiri untuk melihat hasil lainnya dari perbedaan jumlah layer dan parameter di dalamnya.

### Plot Loss dan Akurasi dari Trained Model

Untuk melihat bagaimana plot bekerja mari kita kerjakan latihan berikut. Kita akan menggunakan dataset dan model yang sama dengan latihan sebelumnya. Anda dapat menggunakan latihan sebelumnya dan menambahkan kode-kode berikut di bawah latihan sebelumnya.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   import matplotlib.pyplot as plt   `

**Matplotlib.pyplot** merupakan sebuah modul dalam library Matplotlib yang menyediakan antarmuka untuk membuat visualisasi data dalam bentuk grafik atau plot. Pada latihan ini kita akan membuat sebuah plot dari objek history. Objek history menampung informasi dari akurasi dan loss model pada setiap epoch di proses pelatihan dengan tipe data dictionary sehingga kita bisa membuat plot akurasi atau loss. 

Masih ingatkan cara memanggil key pada dictionary? Untuk mengakses loss kita bisa memanggil fungsi history pada objek history dan menentukan metrik loss yang akan diambil.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   plt.plot(hist.history['loss'])plt.title('Model loss')plt.ylabel('Loss')plt.xlabel('Epoch')plt.legend(['Train'], loc='upper right')plt.show()   `

Dari hasil plot loss di atas, Anda dapat melihat bahwa loss model berkurang sangat signifikan dari epoch pertama sampai epoch ke-100. Lalu, bagaimana dengan plot akurasi? Karena kita sudah menampung akurasi pada model history, kita bisa memilih metrik accuracy pada fungsi history dengan kode yang sama.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   plt.plot(hist.history['accuracy'])plt.title('Model accuracy')plt.ylabel('Accuracy')plt.xlabel('Epoch')plt.legend(['Train'], loc='lower right')plt.show()   `

Dari hasil plot di atas, Anda dapat melihat bahwa akurasi model stagnan pada epoch di sekitar 20 dan juga kembali stagnan pada epoch di atas 80. Dengan menyimpan informasi pada tahap pelatihan model, kita dapat melihat performa model dengan jauh lebih nyaman bukan? Mari bandingkan jika kita tidak menggunakan plot sebagai visualisasi performa model.

Seperti yang dapat Anda lihat pada gambar di atas, kita perlu melihat setiap epochs dan membandingkan satu demi satu metrik yang ada. Tentunya ini akan sangat melelahkan dan menghabiskan waktu. Oleh karena itu, plot hadir untuk meminimalisasi hal tersebut dan mempermudah pekerjaan kita sebagai engineer untuk melakukan evaluasi pada model yang dibangun.

### Mencegah Overfitting dengan Dropout dan Batch Normalization.

Overfitting pada machine learning dapat terjadi ketika data pelatihan yang kita miliki terlalu sedikit dan tidak merepresentasikan semua kemungkinan dari nilai sesungguhnya. Kondisi lainnya adalah ketika kita memiliki data pelatihan yang sangat banyak, tetapi memiliki informasi yang tidak relevan dengan data di lapangan. Hal ini menyebabkan model harus mempelajari data yang kompleks tetapi tidak memiliki pola yang berguna.

Penyebab di atas juga berlaku pada jaringan saraf tiruan. Terus, apa solusinya dan bagaimana kita mengetahui kualitas dari model neural network? Tenang saja, Anda sudah berada di jalur yang tepat. Pada latihan sebelumnya, kita sudah memisahkan data latih dan data uji sehingga kualitas model melalui evaluasi yang sudah dilakukan dapat terlihat.

#### Dropout

Salah satu cara mencegah overfitting adalah dengan menggunakan dropout. Dropout adalah fungsi standar yang umum digunakan industri untuk mencegah overfitting. Seperti yang kita ketahui, semakin kompleks sebuah model machine learning, semakin tinggi kemungkinan model tersebut mengalami overfitting. Dropout bekerja dengan cara mengurangi kompleksitas model neural network tanpa mengubah arsitektur model tersebut.

Untuk mengimplementasikan dropout sendiri sangatlah mudah jika menggunakan Keras. Anda cukup menambahkan layer dropout pada hidden layer di model yang sedang dibuat. Agar lebih jelas perhatikan contoh berikut.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   from keras.layers import Dense, Dropoutmodel = Sequential([                    Dense(64, activation='relu', input_shape=(4,)),                    Dense(64, activation='relu'),                    Dropout(0,5),                    Dense(3, activation='softmax')])   `

Untuk menggunakan dropout, kita cukup menambahkan fungsi **layer tf.keras.layers.Dropout()** dan mengisi parameter berupa persentase yang kita inginkan seperti di atas. Dropout akan otomatis menghilangkan jumlah neuron yang aktif pada layer sebelumnya.

#### Batch Normalization

BatchNormalization adalah layer yang digunakan dalam jaringan saraf tiruan (neural network) untuk mempercepat konvergensi pelatihan dan mengurangi sensitivitas terhadap inisialisasi parameter. Layer ini bekerja dengan melakukan normalisasi input dari layer sebelumnya pada setiap batch sehingga memungkinkan pelatihan yang lebih stabil dan cepat.

Untuk mengimplementasikan BatchNormalization sendiri sangatlah dengan menggunakan Keras. Anda cukup menambahkan layer BatchNormalization pada model neural network. Agar lebih jelas lihatlah contoh di bawah.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   from keras.layers import Dense, Dropout, BatchNormalizationmodel = Sequential([                    Dense(64, activation='relu', input_shape=(4,)),                    Dense(64, activation='relu'),                    Dropout(0,5),                    BatchNormalization(momentum=0.99),                    Dense(3, activation='softmax')])   `

Pada contoh di atas, kita menggunakan salah satu parameter yaitu momentum. Momentum pada BatchNormalization mengacu pada parameter yang dapat mengontrol perhitungan nilai rata-rata dan varians yang dihitung pada setiap batch selama proses pelatihan model. Dengan menggunakan momentum, nilai rata-rata dan varians dihitung berdasarkan gabungan dari nilai-nilai rata-rata dan varians dari mini-batch saat ini dan nilai-nilai sebelumnya yang telah disesuaikan.

Ketika melakukan normalisasi, kita tidak hanya menggunakan nilai dari satu batch saja, tetapi juga mempertimbangkan nilai beberapa batch sebelumnya untuk mendapatkan estimasi yang lebih stabil dari rata-rata dan varians. Ini membantu mengurangi fluktuasi yang mungkin terjadi dalam statistik batch dan meningkatkan konsistensi normalisasi.

Nilai momentum ini sering kali disetel di antara 0,1 dan 0,999. Nilai yang lebih tinggi menunjukkan bahwa kita lebih bergantung pada nilai sebelumnya daripada nilai dari batch saat ini. Sebagai contoh, jika momentum diatur ke 0,9, 90% informasi dari batch sebelumnya akan digunakan dan hanya 10% dari statistik batch saat ini yang akan dipertimbangkan.

Penggunaan momentum pada BatchNormalization membantu menghasilkan data yang lebih stabil dan dapat meningkatkan kinerja pelatihan pada model jaringan saraf tiruan. 

Meskipun BatchNormalization dapat membantu mengurangi overfitting, ini bukan jaminan bahwa model tidak akan mengalami overfitting. Overfitting masih dapat terjadi jika model terlalu kompleks untuk jumlah data pelatihan yang sedikit. Selain itu, ada kemungkinan juga terdapat banyak noise pada data, atau jika ada masalah lainnya dengan proses pelatihan.

### Optimasi Pelatihan menggunakan Callbacks

Fungsi callbacks membantu kita untuk memberi tahu model agar berhenti melakukan pelatihan ketika sudah mencapai target tertentu. Nah, langsung saja kita praktik menggunakan callbacks. Kita masih menggunakan dataset dan model dari latihan klasifikasi iris pada materi sebelumnya. Kode utuhnya seperti di bawah ini.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   import pandas as pdfrom sklearn import preprocessingfrom sklearn.model_selection import train_test_splitfrom keras.models import Sequentialfrom keras.layers import Dense, Dropout, BatchNormalizationimport tensorflow as tfdf = pd.read_csv('https://drive.google.com/uc?id=1roJ83AbgzDcvRr0Gwud0BmdUQx-oSG-w')df = df.drop(columns='Id')category = pd.get_dummies(df.Species, dtype=int)new_df = pd.concat([df, category], axis=1)new_df = new_df.drop(columns='Species')dataset = new_df.values# Pilih 4 kolom pertama untuk dijadikan sebagai atributX = dataset[:,0:4]# Pilih 3 kolom terakhir sebagai labely = dataset[:,4:7]# Normalisasimin_max_scaler = preprocessing.MinMaxScaler()X_scale = min_max_scaler.fit_transform(X)X_scaleX_train, X_test, Y_train, Y_test = train_test_split(X_scale, y, test_size=0.3)from keras.layers import Dense, Dropout, BatchNormalizationmodel = Sequential([                    Dense(64, activation='relu', input_shape=(4,)),                    Dense(64, activation='relu'),                    Dropout(0,5),                    BatchNormalization(momentum=0.99),                    Dense(3, activation='softmax')])model.compile(optimizer='Adam',              loss='categorical_crossentropy',              metrics=['accuracy'])hist = model.fit(X_train, Y_train, epochs=100)   `

Setelah semuanya siap, kita perlu membuat sebuah kelas bernama **myCallback()**. Perhatikan baik-baik. Parameter pertama pada kelas callbacks di atas harus memiliki sifat inherit **tf.keras.callbacks.Callback**. Selanjutnya, kita buat fungsi yang paling penting yaitu **on\_epoch\_end()**. Fungsi inilah yang akan berperan untuk memberi tahu model agar berhenti melakukan pelatihan ketika telah mencapai target.

Kode **if(logs.get(‘accuracy’)>0.9)** sangat intuitif menunjukkan kalau kode itu memiliki arti “jika akurasi lebih besar dari 0.9, maka eksekusi perintah berikutnya”. Kita juga dapat menulis kode **print(“\\nAkurasi telah mencapai >90%!”)** untuk ditampilkan ketika callbacks aktif.

Kode **self.model.stop\_training = True** adalah kode yang memberi tahu model untuk menghentikan pelatihan. Setelah kelas ini dibuat, buatlah objek dari kelas tersebut. Berikut kode lengkap untuk membuat callbacks.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   class myCallback(tf.keras.callbacks.Callback):  def on_epoch_end(self, epoch, logs={}):    if(logs.get('accuracy')>0.9):      print("\nAkurasi telah mencapai >90%!")      self.model.stop_training = Truecallbacks = myCallback()   `

Setelah membuat sebuah objek callbacks, selanjutnya kita harus menambahkan _hyperparameter_ tersebut pada saat melakukan proses pelatihan. Untuk menggunakan callbacks sangat gampang, kita hanya perlu menambahkan parameter callbacks dan mengisi objek callbacks yang telah kita buat pada parameter tersebut.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   hist = model.fit(X_train, Y_train, epochs=100, callbacks = [callbacks])   `

Hasil dari menjalankan kode tersebut pada model sederhana dapat dilihat pada gambar di bawah ini.

Dari latihan di atas dapat dilihat model berhasil menghentikan pelatihan ketika telah mencapai akurasi yang kita tentukan pada epoch ke 5 dari 100. Kita telah menghemat waktu eksekusi sebanyak 96 epoch. Keren, bukan?

### Menggunakan Dataset dari TensorFlow

Seperti yang telah kita lakukan pada materi sebelumnya, TensorFlow juga menyediakan dataset yang siap dipakai yang dapat digunakan untuk belajar/eksplorasi. Anda dapat mengunjungi tautan [TensorFlow Datasets](https://www.tensorflow.org/api_docs/python/tf/keras/datasets) untuk melihat dataset apa saja yang tersedia dari library TensorFlow. 

Ada dua cara untuk mengakses dataset yang sudah disediakan TensorFlow yaitu melalui **tf.data.Datasets** dan juga **TensorFlow Datasets.** Keduanya memiliki fungsi yang sangat mudah digunakan tetapi memiliki variasi data yang berbeda.

#### Menggunakan tf.data.Datasets

_As usual_, hal pertama yang kita lakukan adalah melakukan impor library TensorFlow agar dapat mengakses seluruh fungsi yang ada.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   import tensorflow as tf   `

Kemudian kita buat objek untuk menampung dataset kita dan masukkan fungsi **tf.keras.datasets.** pada objek tersebut. Karena pada kasus ini menggunakan dataset mnist, kode yang digunakan sebagai berikut.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   mnist = tf.keras.datasets.mnist   `

Selanjutnya, kita perlu membagi dataset yang sudah ada menjadi dua bagian yaitu pelatihan dan uji menggunakan fungsi **load\_data()**. Fungsi **load\_data()** dari objek dataset mengembalikan bentuk dataset yang telah dibagi menjadi atribut latih, label latih, atribut uji, dan label uji. Sangat gampang, bukan? Hanya dengan beberapa baris kode kita sudah memiliki data latih dan data uji yang siap dipakai.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   (gambar_latih, label_latih), (gambar_testing, label_testing) = mnist.load_data()   `

#### Menggunakan TensorFlow Datasets

TensorFlow menyediakan kumpulan dataset siap pakai untuk dilatih dengan TensorFlow, Jax, dan framework machine learning lainnya. TensorFlow Dataset (TFDS) bertugas untuk melakukan pengunduhan dan menyiapkan data secara deterministik dengan menggunakan **tf.data.Dataset** (atau np.array).

Sebelumnya, kita sudah mempelajari tf.data.Datasets, sekarang kita mengenal rivalnya yaitu TFDS. Namanya, cukup mirip, ya? Jangan bingung antara TFDS (library ini) dengan tf.data.Datasets (API dari TensorFlow). 

TFDS adalah _wrapper_ tingkat tinggi di sekitar tf.data. Jika Anda tidak terbiasa dengan API ini, kami menyarankan Anda untuk membaca panduan resmi dari TensorFlow pada tautan berikut: [tf.data](https://www.tensorflow.org/guide/data).

Di sisi lain, TFDS juga menyediakan lebih banyak datasets yang siap digunakan. Tanpa berlama-lama, mari kita mulai perjalanan ini dengan melakukan impor library yang akan digunakan.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   import matplotlib.pyplot as pltimport numpy as npimport tensorflow as tfimport tensorflow_datasets as tfds   `

Setelah berhasil menginstal library TFDS, kita dapat melihat _list_ atau daftar dari dataset yang tersedia pada TFDS. Untuk melihat seluruh dataset yang tersedia, kita bisa menggunakan fungsi **tfds.list\_builders()** atau dapat dilihat pada katalog [TensorFlow Datasets](https://www.tensorflow.org/datasets/catalog/overview).

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   tfds.list_builders()   `

Seperti yang Anda lihat pada gambar di atas, ada banyak sekali dataset yang tersedia ketika kita menggunakan TFDS, baik itu untuk pembelajaran maupun eksplorasi mandiri. Setelah melihat banyak sekali dataset, tentunya kita harus menentukan dataset mana yang akan digunakan, bukan? Tenang saja, caranya sangat mudah. Kita hanya perlu menggunakan fungsi **tfds.load()** seperti berikut.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   ds = tfds.load('mnist', split='train', shuffle_files=True)assert isinstance(ds, tf.data.Dataset)   `

Kode di atas memuat dataset MNIST menggunakan TensorFlow Datasets. Mari kita jelaskan satu per satu detail dari kode di atas.

*   Fungsi load() memungkinkan Anda untuk menggunakan dataset yang telah disediakan oleh TensorFlow Datasets. 
    
*   Parameter pertama ('mnist') menunjukkan nama dataset yang ingin dimuat. 
    
*   Parameter kedua ('split='train'') menunjukkan bahwa kita hanya memuat bagian pelatihan dari dataset MNIST. 
    
*   Parameter ketiga ('shuffle\_files=True') mengindikasikan bahwa file-file dataset akan diacak sebelum dimuat, sehingga urutan data tidak akan tetap sama setiap kali dataset dimuat ulang. 
    

Pada hakikatnya masih ada argumen umum yang sering digunakan ketika melakukan load dataset menggunakan tfds. Untuk mengetahui lebih detail, Anda dapat melihat pada website resminya [TensorFlow Loads](https://www.tensorflow.org/datasets/api_docs/python/tfds/load), ya.

### Penggunaan Batch Loading

Batch loading adalah proses pelatihan ketika neural network melakukan pembaruan parameternya (_weight_) setelah membaca sejumlah sampel data tertentu. Misal dataset kita berisi 800 buah gambar pizza. Tanpa batch size, proses pembaruan parameter terjadi untuk seluruh sampel pada dataset. Sehingga, ketika tanpa menggunakan batch size, pada 1 epoch terdapat 800 kali pembaruan weight. Ketika 1 ukuran batch adalah 32 buah gambar pizza, terdapat 25 buah batch pada dataset. Pada batch loading, model baru melakukan pembaruan parameter setelah membaca satu batch atau 32 buah gambar pizza. Sehingga, proses pembaruan parameter pada 1 epoch hanya sebanyak 25 kali.

Apakah Anda sudah menyadari apa fungsi dari batch loading? _Yup_ benar, dengan batch loading proses pelatihan data akan menjadi lebih cepat. Kita akan melihat langsung kegunaan dari batch loading pada latihan berikut.

Untuk dataset, kita akan menggunakan dataset mnist dan model yang sama dengan materi sebelumnya.  

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   import tensorflow as tfmnist = tf.keras.datasets.mnist(training_images, training_labels), (test_images, test_labels) = mnist.load_data()training_images  = training_images / 255.0test_images = test_images / 255.0model = tf.keras.models.Sequential([tf.keras.layers.Flatten(input_shape=(28,28)),                                     tf.keras.layers.Dense(128, activation=tf.nn.relu),                                     tf.keras.layers.Dense(10, activation=tf.nn.softmax)])model.compile(optimizer = tf.optimizers.Adam(),              loss = 'sparse_categorical_crossentropy',              metrics=['accuracy'])   `

Selanjutnya, buatlah fungsi **fit()** untuk melakukan pelatihan. Perlu Anda perhatikan, di sini kita mulai menggunakan batch loading. Untuk menggunakan batch loading, kita hanya menambahkan satu parameter ‘batch\_size’ pada fungsi **fit()**. 

Tahukah Anda bahwa fungsi **fit()** secara _default_ menggunakan batch loading dengan batch size sebesar 32. Sehingga, ketika kita tidak mendefinisikan nilai parameter batch\_size, ukuran batch akan diisi sebesar 32 secara _default_. Perhatikan bahwa pada setiap epoch memakan waktu selama sekitar 3 atau 4 detik.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   model.fit(training_images, training_labels, batch_size=32, epochs=5)   `

Agar lebih paham, sekarang kita akan menggunakan batch\_size yang lebih besar yaitu 128. Dapat kita lihat bahwa semakin besar batch size, waktu eksekusi tiap epoch akan semakin cepat. 

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   model.fit(training_images, training_labels, batch_size=128, epochs=5)   `

Seperti yang Anda lihat di atas, waktu pelatihan yang dilakukan memakan waktu yang lebih singkat. Silakan Anda bereksperimen menggunakan batch size yang lain untuk pengalaman belajar yang lebih maksimal. Bagaimana hasilnya? Silakan beri kesimpulan sendiri, ya. 

Pada latihan ini, kita telah memahami bahwa dengan menggunakan batch loading dapat mempercepat pelatihan. Untuk pemilihan batch size sendiri tidak ada aturan bakunya, tetapi yang umum dipakai adalah 32, 64, dan 128. Anda harus bereksperimen sendiri guna menemukan batch size yang cocok dengan masalah atau model yang sedang dibangun.

Rangkuman Natural Language Processing (NLP) dengan Tensorflow
-------------------------------------------------------------

### Pengenalan Natural Language Processing

_Natural language processing_ (NLP) adalah salah satu cabang ilmu komputer yang mempelajari cara komputer berinteraksi dengan penggunaan bahasa dalam kehidupan sehari-hari. NLP bertujuan mengembangkan teknik-teknik agar komputer dapat memahami **bahasa alami manusia.**

### Peran NLP dalam Kehidupan Sehari-hari

1.  Search Engine (Mesin Pencari)
    
2.  Asisten Virtual
    
3.  Penerjemahan Otomatis
    
4.  Analisis Sentimen Media Sosial
    
5.  Deteksi Spam
    
6.  Pemeriksaan Tanda Baca, Tata Bahasa, dan Parafrase
    
7.  Chatbot dalam Layanan Pelanggan
    

### TensorFlow + NLP, Mengapa?

TensorFlow dan NLP adalah pasangan yang kuat dalam dunia teknologi karena kombinasi kemampuan komputasi numerik TensorFlow dan fokus NLP untuk memahami bahasa manusia. TensorFlow, sebagai framework machine learning dan deep learning yang populer, menawarkan efisiensi dalam komputasi numerik yang sangat dibutuhkan dalam operasi matriks kompleks seperti yang digunakan dalam model NLP seperti neural networks. 

### Text Preprocessing

Langkah-langkah pra-pemrosesan teks dalam NLP sangat penting untuk mengubah teks menjadi bentuk numerik yang dapat dipahami oleh komputer. Algoritma dan komputer secara alami memahami data dalam bentuk numerik, seperti vektor atau matriks. 

#### Case Folding

Proses mengubah semua huruf dalam teks menjadi huruf kecil atau huruf besar agar konsisten. Misalnya, mengubah "TeKS" menjadi "teks" atau "TEKS".

#### Removal Special Characters

Menghapus karakter khusus atau simbol yang tidak relevan atau tidak diinginkan dari teks. 

*   **Menghapus Angka:** Menghilangkan semua angka dari teks.
    
*   **Menghapus Tanda Baca:** Menghapus semua tanda baca dari teks.
    
*   **Menghapus White Space:** Menghapus spasi tambahan atau karakter spasi ganda dari teks.
    
    *   **Menggunakan strip():** Menggunakan metode strip() dalam pemrograman untuk menghapus spasi tambahan di awal dan akhir teks.
        
    *   **Menggunakan replace():** Menggunakan metode replace() untuk mengganti spasi tambahan dengan string kosong sehingga menghapusnya dari seluruh teks.
        

#### Stopword Removal (Filtering)

Menghapus kata-kata yang umumnya tidak memberikan nilai tambah dalam analisis teks, seperti "dan", "atau", "yang", dll.

*   **Stopword NLTK (Natural Language Toolkit):** Menggunakan koleksi kata-kata stopword yang disediakan oleh NLTK untuk menghapus stopword dari teks.
    
*   **Stopword Sastrawi:** Penghapusan kata-kata stopword menggunakan kamus stopword yang disediakan oleh Sastrawi, pustaka pemrosesan bahasa alami bahasa Indonesia.
    

#### Tokenizing

Proses membagi teks menjadi bagian-bagian lebih kecil yang disebut token.

*   **Tokenisasi Kata (Word Tokenization)**: Memecah teks menjadi token berdasarkan kata-kata individual.
    
*   **Tokenisasi Kalimat (Sentence Tokenization)**: Memecah teks menjadi token berdasarkan kalimat-kalimat.
    
*   **Tokenisasi Frasa (Phrase Tokenization)**: Memecah teks menjadi token berdasarkan frasa-frasa atau unit-unit tertentu.
    
*   **Tokenisasi Berdasarkan Aturan (Rule-based Tokenization)**: Memecah teks menjadi token berdasarkan aturan tertentu, seperti pemisahan berdasarkan tanda baca.
    
*   **Tokenisasi Berdasarkan Model (Model-based Tokenization)**: Memecah teks menjadi token menggunakan model linguistik atau machine learning.
    

#### Stemming

Proses menghapus imbuhan dari kata untuk mengembalikannya ke bentuk dasarnya. Misalnya, mengubah "berlari", "berlarian", "lari" menjadi "lar".

#### Lemmatization

Proses mengubah kata-kata ke bentuk dasarnya (lema) dengan mempertimbangkan konteks dan struktur bahasa. Misalnya, mengubah "menyanyikan" menjadi "nyanyi".

### Ekstraksi Fitur

Ekstraksi fitur pada teks adalah kunci untuk mengubah teks menjadi bentuk yang dapat dipahami oleh algoritma machine learning, yaitu **numerik**. Saat kita berurusan dengan teks, seperti ulasan pelanggan, artikel berita, atau dokumen bisnis, kita perlu **mengubahnya menjadi representasi numerik** yang dapat diinterpretasikan oleh komputer. Tujuannya tidak hanya memproses teks, tetapi juga untuk mengekstrak informasi berharga yang tersembunyi di dalamnya. 

Berikut adalah beberapa teknik umum yang digunakan untuk ekstraksi fitur pada teks.

1.  Word Embedding
    
2.  Term Frequency-Inverse Document Frequency (TF-IDF)
    
3.  Bag of Words (BoW)
    
4.  N-gram
    
5.  POS Tagging (Part of Speech Tagging)
    
6.  Entity Recognition
    
7.  Pola atau Pola Kata (Pattern Matching)
    

#### Word Embedding

_Word embedding_ adalah teknik dalam NLP untuk **merepresentasikan distribusi kata-kata di ruang vektor**. Tujuan utama dari word embedding adalah menangkap hubungan semantik dan sintaktis antarkata dalam teks. 

Ada beberapa teknik word embedding yang populer digunakan dalam NLP.

1.  **Word2Vec**: Word2Vec memodelkan kata-kata sebagai vektor numerik berdasarkan hubungan kata-kata yang muncul bersama dalam teks. Ada dua pendekatan utama dalam Word2Vec.
    
    *   **Skip-gram**: Model Word2Vec skip-gram melatih neural network untuk memprediksi kata target berdasarkan kata-kata sekitarnya (konteks) dalam suatu kalimat.
        
    *   **Continuous Bag of Words (CBOW)**: Pendekatan CBOW adalah kebalikan dari skip-gram. Alih-alih memprediksi kata target berdasarkan context, skip-gram justru berupaya memprediksi kata-kata di sekitar (context) berdasarkan kata tertentu (kata target). 
        
2.  **GloVe (Global Vectors for Word Representation)**: GloVe adalah metode word embedding untuk menghasilkan vektor representasi kata-kata berdasarkan statistik dari matriks frekuensi kemunculan kata dalam teks (_co-occurrence matrix_). 
    
3.  **FastText**: FastText adalah ekstensi dari Word2Vec yang dikembangkan oleh Facebook AI Research (FAIR).
    

#### Term Frequency-Inverse Document Frequency (TF-IDF)

TF-IDF (_term frequency-inverse document frequency_) adalah sebuah metode  pengolahan teks untuk mengevaluasi seberapa penting sebuah kata pada suatu dokumen dalam konteks korpus atau kumpulan dokumen yang lebih besar. 

#### Bag of Words (BoW)

_Bag of Words_ (BoW) adalah sebuah pendekatan sederhana dalam pemrosesan teks yang digunakan untuk mewakili teks sebagai kumpulan kata-kata terurut tanpa memperhatikan tata urutan atau struktur kalimat.

#### N-gram

_N-gram_ adalah sekumpulan n kata berurutan yang diambil dari sebuah teks atau urutan data. N-gram digunakan pada pemrosesan teks dan pengenalan pola untuk memahami hubungan antar kata dalam teks. Nilai n dalam "n-gram" menunjukkan jumlah kata yang diambil pada satu kali pengambilan. Contoh umum n-gram yaitu unigram (1-gram), bigram (2-gram), trigram (3-gram), dan seterusnya.

### Binary vs Multiclass vs Multilabel Classification pada Text

Binary classification adalah sebuah teknik dalam machine learning untuk memisahkan data pada **dua kelas atau kategori** yang saling eksklusif berdasarkan pemberian fitur atau atribut. Dalam binary classification, ada dua kelas yang mungkin untuk diprediksi, biasanya disebut sebagai kelas positif dan kelas negatif. 

Multiclass classification adalah jenis masalah klasifikasi dalam machine learning bahwa model harus memprediksi kelas atau label dari data dalam **lebih dari dua kategori** yang berbeda. Dalam konteks ini, setiap contoh data dapat diklasifikasikan ke salah satu dari beberapa kelas dan setiap kelas mewakili kategori yang berbeda.

Multi-label classification adalah jenis masalah klasifikasi pada machine learning bahwa **setiap instance data dapat dikategorikan dalam lebih dari satu label atau kelas sekaligus**. Dengan kata lain, beberapa label atau kategori yang relevan dapat diberikan kepada satu instance data.

### Algoritma RNN (Recurrent Neural Network)

RNN adalah jenis arsitektur deep learning yang dirancang khusus untuk mengolah data sekuensial. Keunggulan utama RNN adalah kemampuannya untuk menangani urutan input variabel dalam panjang dan mengingat informasi dari langkah-langkah sebelumnya, yang membuatnya sangat berguna dalam berbagai tugas seperti pemrosesan bahasa alami, pemodelan waktu, dan banyak lagi.

#### Mekanisme Dasar RNN

*   Loop internal: RNN memiliki loop internal yang menghubungkan neuron pada layer tersembunyi, memungkinkan informasi dari input sebelumnya untuk disimpan dan digunakan dalam pemrosesan input selanjutnya.
    
*   State: RNN memiliki state internal yang diperbarui dengan setiap input baru, mewakili informasi yang diingat dari input sebelumnya.
    

#### Struktur RNN

*   Input: Urutan data seperti kata-kata, sampel sinyal waktu, atau piksel dalam gambar.
    
*   Recurrent Unit: Memproses input saat ini dan keadaan tersembunyi sebelumnya untuk menghasilkan output dan keadaan tersembunyi baru.
    
*   Output: Hasil akhir yang diinginkan, seperti kata berikutnya dalam kalimat atau nilai berikutnya dalam sinyal waktu.
    

#### Tantangan RNN

RNN menghadapi kesulitan dalam mempertahankan informasi jangka panjang dan mengatasi masalah gradien yang melemah (vanishing gradient problem). Untuk mengatasi masalah ini, varian seperti Long Short-Term Memory (LSTM) dan Gated Recurrent Unit (GRU) telah dikembangkan.

### Long Short-Term Memory (LSTM)

LSTM adalah jenis ANN dalam kategori RNN yang dirancang untuk mengatasi keterbatasan RNN konvensional dalam menangani data sekuensial dengan ketergantungan jangka panjang. LSTM memiliki fitur sel memori dan mekanisme gating untuk mengontrol aliran informasi.

#### Keunggulan Utama LSTM

*   Memori Jangka Panjang: Dapat menyimpan informasi penting dalam jangka waktu yang lama.
    
*   Mengatasi Vanishing Gradient: Tidak mudah terpengaruh oleh masalah gradien menghilang.
    
*   Fleksibel: Dapat dimodifikasi untuk berbagai aplikasi.
    

#### Komponen LSTM

*   Sel Memori: Menyimpan informasi penting.
    
*   Gate:
    
    *   **Forget Gate:** Mengatur informasi yang akan dihapus.
        
    *   **Input Gate:** Mengatur informasi baru yang akan ditambahkan.
        
    *   **Output Gate:** Mengatur informasi yang akan dikeluarkan.
        

### Gated Recurrent Unit (GRU)

GRU adalah varian RNN yang lebih sederhana dan efisien secara komputasi dibandingkan LSTM, dengan hanya dua gate (update gate dan reset gate).

#### Keunggulan Utama GRU

*   Komputasi Lebih Ringan: Struktur lebih sederhana membutuhkan lebih sedikit sumber daya.
    
*   Training yang Lebih Cepat: Proses pelatihan lebih cepat.
    
*   Pencegahan Vanishing Gradient: Mengatasi masalah gradien yang melemah.
    
*   Penghematan Memori: Membutuhkan lebih sedikit parameter.
    

#### Komponen GRU

*   Reset Gate: Mengontrol seberapa banyak informasi dari status tersembunyi sebelumnya yang akan disimpan.
    
*   Update Gate: Mengontrol seberapa banyak informasi baru yang akan ditambahkan ke hidden state.
    

Rangkuman Berkenalan dengan Time Series
---------------------------------------

### Pengenalan Time Series

Secara singkat time series merupakan penerapan teknik dari ekstrapolasi, sedangkan regression adalah penerapan dari interpolasi. _Hmmm_, apa _tuh bang_?

Interpolasi dan ekstrapolasi merupakan sebuah teknik statistik yang dapat menebak atau memprediksi suatu nilai data dengan memperhatikan data lain yang kita miliki. Interpolasi adalah sebuah teknik yang dapat mencari suatu nilai variabel pada rentang data yang diketahui, sedangkan ekstrapolasi merupakan teknik menemukan nilai suatu variabel di luar rentang data yang sudah diketahui.

Time series dan regresi merupakan metode yang dapat melakukan analisis prediktif, tetapi keduanya memiliki asumsi, teknik, dan implementasi yang berbeda. Secara singkat, time series membutuhkan data yang tersusun dan bergantung pada suatu rentang waktu, sedangkan regresi memiliki data yang independen dan bersifat acak. Selain itu, time series lebih cocok untuk meramalkan dan mendeteksi pola pada data temporal, sedangkan regresi lebih cocok untuk memperkirakan dan menjelaskan pengaruh atau hubungan variabel terhadap suatu hasil.

Dengan kondisi yang serupa tapi tak sama, lantas kapan kita harus menggunakan metode time series? Ketika memilih sebuah metode analisis prediktif yang tepat, penting untuk kita mempertimbangkan karakteristik dan tujuan dari data yang dimiliki. Berikut pertimbangan yang dapat Anda pikirkan untuk memilih metode prediktif.

1.  Pastikan terlebih dahulu apakah data yang Anda miliki tersusun dengan baik dan bergantung pada suatu waktu atau independen dan acak? 
    
2.  Pertimbangkan apakah Anda ingin menyelesaikan permasalahan dengan rentang waktu tertentu atau memperkirakan efek variabel pada satu waktu?
    
3.  Anda harus memperhatikan pola, tren, atau hubungan dalam data tersebut. Selain itu, Anda juga perlu memperhatikan banyak data, keandalan dan konsistensi data.
    

Perhatikan batasan dan sudut pandang dari setiap metode serta kecocokan dari output yang diberikan dengan hasil yang diinginkan.

### Machine Learning pada Time Series

Seiring berkembangnya teknologi, sekarang manusia dapat melakukan forecasting menggunakan machine learning atau deep learning tanpa harus melakukan perhitungan secara manual. Oleh karena itu, kita dapat melakukan pekerjaan dengan lebih cepat dan efektif.

Machine learning forecasting memiliki beberapa kelebihan salah satunya adalah hasil yang lebih akurat karena dapat terhindar dari kesalahan manusia (_human error_) dalam melakukan perhitungan.

Namun, dengan menggunakan machine learning tentunya ada _trade-off_ juga. Kekurangan dari machine learning adalah membutuhkan resource yang cukup mahal karena kita harus membeli sebuah perangkat yang dapat memproses banyak data dalam waktu yang singkat. 

Tentunya, semakin mahal sumber daya yang Anda gunakan, semakin cepat juga proses perhitungan yang dilakukan oleh komputer. Sehingga dengan harga yang dikeluarkan akan sebanding atau bahkan lebih banyak benefit yang diterima.

Dengan menggunakan machine learning, kita dapat memproses nilai menggunakan algoritma yang dapat mempelajari pola data dan melakukan prediksi dalam rentang waktu tertentu. Machine learning akan memproses data yang Anda miliki menyesuaikan dengan algoritma yang sudah ditentukan.

### Tipe-Tipe Time Series

Secara umum time series terbagi menjadi dua kelompok besar yaitu _univariate_ dan _multivariate_. Mari kita bahas keduanya secara lebih mendalam.

1.  _**Univariate Time Series**_Univariate time series biasanya digunakan ketika Anda ingin membuat suatu nilai prediksi dari satu variabel, terutama ketika ada data historis yang tersedia untuk variabel tersebut. Teknik ini sangat umum dan mendasar karena sering diterapkan secara umum di berbagai bidang seperti ekonomi, keuangan, prakiraan cuaca, prakiraan permintaan dalam manajemen rantai pasokan, dan lain sebagainya.
    
2.  _**Multivariate Time Series**_Seperti namanya, multivariate time series memiliki lebih dari satu variabel data pada dataset time series yang akan di analisis. Setiap variabel tidak hanya bergantung pada nilai masa lalunya (histori), tetapi juga memiliki ketergantungan atau hubungan dengan variabel lainnya. Hubungan ini digunakan untuk melakukan prediksi atau meramalkan nilai-nilai yang akan datang. Kedengarannya rumit, ya? Mari kita perjelas lagi.Contoh sebelumnya pada kasus univariate, kita hanya menggunakan suhu sebagai data yang akan diprediksi tanpa mempertimbangkan faktor lainnya. Hal ini menyebabkan akurasi yang dihasilkan hanya berfokus pada pola suhu yang terjadi berdasarkan histori yang ada. Untuk melakukan forecasting yang lebih kompleks dan banyak variabel atau faktor eksternal yang memiliki dampak teknik, multivariate akan lebih menghasilkan prediksi yang lebih baik.
    

Selain univariate dan multivariate, time series juga dapat dibedakan lagi berdasarkan pola datanya. Pola pertama dikenal sebagai tren di mana data-data pada time series bergerak pada arah yang spesifik seperti tren menaik atau menurun.

Pola lainnya disebut time series musiman (_seasonal_). Pada time series, pola ini terdapat pola yang berulang pada interval tertentu. Contoh time series ini adalah data temperatur setiap harinya. Pada musim dingin temperatur berada di titik terendah; beranjak ke musim hujan temperatur semakin naik; sementara pada musim panas temperatur berada pada posisi tertinggi.

Lalu, ada _Noisy time series_. Time series seperti ini banyak mengandung noise atau data random yang tidak membantu dalam proses analisis. Kenapa demikian? Sederhana saja karena tidak ada pola yang dapat dibaca dan dipelajari dengan pasti dari time series seperti ini.

Kemudian ada time series _stationary_ dan _non-stationary_. Pada time series bertipe stationary, pola-polanya seragam. Contohnya pada grafik Hukum Moore, pola pada time series terus menaik dan tidak pernah turun.

Namun, pada time series non stationary, pola-pola pada time series tidak seragam. Contohnya pada data indeks pasar saham DOW di bawah. Perubahan pola tersebut dapat disebabkan oleh suatu skandal atau gelembung ekonomi (_economic bubble_) yang pecah.

### Data Preprocessing untuk Time Series

Data processing adalah tahapan penting dalam pembangunan model time series forecasting. Tujuan utamanya adalah untuk membersihkan, menyusun, dan mempersiapkan data sehingga model forecasting dapat bekerja dengan baik. Berikut beberapa tujuan dan manfaat dari data processing untuk time series forecasting.

1.  **Membersihkan data:** data mentah sering kali memiliki noise, nilai yang hilang, atau outlier yang dapat mempengaruhi kualitas prediksi. Dengan melakukan data processing, Anda dapat membersihkan data ini untuk meningkatkan keakuratan model.
    
2.  **Menyusun data:** data time series sering kali memiliki format yang kompleks, seperti tanggal dan waktu, yang perlu diatur dengan benar agar sesuai dengan kebutuhan model. Data processing membantu menyusun data ini menjadi format yang sesuai untuk analisis.
    
3.  **Menangani nilai yang hilang:** kadang-kadang data time series memiliki nilai yang hilang sehingga dapat mengganggu analisis dan prediksi. Data processing memungkinkan Anda untuk menangani nilai yang hilang dengan cara yang sesuai, seperti interpolasi atau pengisian nilai rata-rata.
    
4.  **Menyederhanakan data:** terkadang, data time series dapat memiliki dimensi yang besar atau variabel yang tidak relevan. Dengan melakukan data processing, Anda dapat menyederhanakan data ini untuk fokus pada informasi yang paling penting untuk forecasting.
    
5.  **Normalisasi dan penskalaan:** proses normalisasi dan penskalaan dapat membantu memperbaiki performa model, terutama jika fitur-fitur dalam data memiliki skala yang berbeda-beda.
    
6.  **Ekstraksi fitur:** data processing dapat melibatkan ekstraksi fitur dari data time series yang dapat membantu meningkatkan kemampuan prediktif model. Misalnya, ekstraksi pola, tren, atau musiman dari data.
    
7.  **Pemilihan fitur:** memilih fitur-fitur yang paling relevan dapat membantu meningkatkan kinerja model dan mengurangi kompleksitasnya.
    
8.  **Validasi dan pembagian data:** data processing juga melibatkan validasi data untuk memastikan keandalan dan konsistensinya. Selain itu, membagi data menjadi set pelatihan dan pengujian yang sesuai adalah langkah penting dalam proses ini.
    

Dengan melakukan data processing yang tepat, Anda dapat mempersiapkan data time series dengan baik sehingga model forecasting dapat memberikan hasil prediksi yang akurat dan berguna.

Hal pertama yang perlu kita lakukan setelah data siap adalah membagi data time series menjadi data training dan testing. Pembagian data pada time series dilakukan dengan membaginya menjadi ke dalam 2 periode yakni periode training dan periode validation. Dengan membagi data seperti ini, kita mendapat gambaran prediksi dari model.

_For your information_, saat membagi data pada time series yang bersifat seasonal, kita perlu membagi sesuai musim yang ada. Contohnya data penjualan bulanan. Untuk periode training dan validation, datanya harus dalam satuan bulanan bukan mingguan atau harian. Misalnya untuk periode validasi, gunakan data dua bulan terakhir, bukan data tiga minggu terakhir. 

Kemudian, sama seperti kasus machine learning pada umumnya, kita harus membagi data kita menjadi atribut dan label. Bagaimana kita melakukannya pada data time series? Pertama, kita mengambil sebagian kecil dari data yang dapat disebut _window_ atau biasa disebut _windowed dataset_. 

Sebuah window dapat berisi sebanyak N data, atau ukuran window dapat kita tentukan sebesar interval waktu tertentu misalnya satu minggu, empat hari, dan lain sebagainya. Sebelum kita masuk ke kode, mari kita asumsikan memiliki sebuah deret data dan ingin melakukan prediksi dengan menggunakan data tujuh hari sebelumnya untuk memprediksi satu hari selanjutnya seperti berikut.

\[0, 1, 2, 3, 4, 5, 6\] -> \[7\]

\[1, 2, 3, 4, 5, 6, 7\] -> \[8\]

\[2, 3, 4, 5, 6, 7, 8\] -> \[9\]

Ketika kita menggunakan data yang lebih banyak, tentunya akan sulit untuk melihat pergeseran secara menyeluruh. Dengan menggunakan windowing data sebanyak n akan terus bergeser setiap langkah yang sudah ditentukan atau biasa disebut dengan _stride_. _Stride_ memiliki nama lain pada time series yaitu _window slide_. Teknik ini digunakan untuk melakukan analisis data time series dengan membagi data ke dalam window dan memproses setiap window secara independen. Hal ini sangat berguna untuk tugas-tugas seperti forecasting yang mengharuskan Anda untuk memperhitungkan hubungan antara titik-titik data yang berdekatan. 

Seperti yang Anda lihat pada gambar di atas, data yang “dibungkus” menjadi windowed dataset akan bergeser sebanyak x langkah. Tentunya hal tersebut dapat diatur sesuai dengan kebutuhan dan eksplorasi yang Anda lakukan. Jika Anda penasaran proses dari data time series secara utuh, perhatikan gambar berikut.

Gambar di atas bertujuan untuk mengambil sebagian kecil dari data yang dapat berisi sebanyak N data, atau ukuran window dapat kita tentukan sebesar interval waktu tertentu, seperti satu minggu, tiga hari, dan lain sebagainya. 

Catatan:

_**Horizon**_: jumlah langkah waktu masa depan yang ingin kita prediksi.

_**Window Size**_: jumlah langkah waktu yang akan kita gunakan untuk memprediksi masa depan (horizon).

Misalnya, kita ingin menentukan ukuran window (window size) sebesar tujuh buah data. Nah, fitur-fitur pada window tersebut adalah setiap nilai yang ada pada window dan labelnya adalah nilai selanjutnya (horizon). Contohnya, kita memiliki tujuh buah data 1,2,3,4,5,6,7. Lalu, ukuran window yang kita pilih adalah tiga. Fitur dan label untuk window tersebut ditampilkan pada tabel di bawah. Perhatikan bahwa fitur 6 dan 7 tidak dimasukkan karena keduanya tidak ada nilai setelah 7.

_To be honest_, ada dua pendekatan utama untuk melakukan forecasting pada data time series. Sebelumnya kita sudah mempelajari tentang sliding window, sekarang saatnya kita melebarkan sayap dengan mempelajari pendekatan lainnya, yaitu _expanding window_! 

Dalam konteks time series, expanding window merupakan perhitungan statistik yang menghitung rata-rata dari data time series melalui ukuran window yang akan diperluas setiap waktunya. Berbeda dengan sliding window yang menggunakan analisis dengan ukuran tetap, expanding window ini akan terus memperbesar ukuran window mencakup semua analisis hingga titik waktu terakhir. Perhatikan gambar berikut.

Dari sini, cukup jelas ya perbedaan dari sliding windows dan expanding windows? Untuk memperkuat ingatan, mari kita sedikit rekap perbedaannya menjadi seperti berikut.

*   **Sliding Windows:** dalam pendekatan ini window akan bergerak maju dalam data time series dengan interval yang tetap. Setiap kali window bergeser maka data window baru dibuat dengan data yang berikutnya, dan data window lama diabaikan. 
    
*   **Expanding Windows:** dalam pendekatan expanding windows, window akan diperluas secara bertahap saat data time series berkembang. Setiap kali window diperluas, ia akan mencakup semua data sebelumnya ditambah satu titik data terbaru.
    

Perbedaan ini dapat diilustrasikan dengan contoh sederhana. Misalkan kita memiliki data time series harian tentang penjualan selama 100 hari.

*   Dengan sliding windows, kita mungkin membuat window akan bergeser 30 hari. Jadi, kita akan memiliki 71 window dengan masing-masing window berisi 30 data.
    
*   Dengan expanding window, kita mungkin membuat jendela mulai dari data hari pertama hingga data di hari ke 100. Jadi, kita akan memiliki 100 jendela dengan ukuran bertambah setiap harinya.
    

Kedua pendekatan ini memiliki kegunaan dan aplikasi yang berbeda. Sliding windows sering digunakan dalam pemodelan dan prediksi untuk mengamati pola dan tren baru dalam data, sedangkan expanding windows sering digunakan dalam analisis retrospektif untuk menghitung statistik yang berkembang seiring waktu. 

Namun, pada dunia machine learning tidak ada hal yang pasti sehingga kedua pendekatan ini perlu kita coba juga ya agar mendapatkan pengalaman dan hasil yang maksimal di setiap kasus yang sedang kita hadapi.

### Matrik Evaluasi untuk Time Series

Untuk mengevaluasi model time series, kita dapat menghitung error yang dibuat pada model seperti kita mengevaluasi model regresi. Yup, kita bisa mendapatkan error dengan menghitung jarak antara nilai prediksi model dan nilai sebenarnya.

Ada beberapa metrik yang dapat dipakai dalam evaluasi model time series, seperti MSE, RMSE, MAE, MAPE, dan lain sebagainya. Namun, hal paling sederhana yang dapat kita lakukan adalah dengan menghitung error secara langsung.

Mari kita asumsikan memiliki sebuah data aktual dan hasil prediksi (forecast) sebagai berikut.

ActualForecast

4.216

4.266

5.36

5.415

5.374

5.437

5.388

5.338

Dengan data di atas, mari kita lihat penggunaan contoh paling sederhana menghitung error secara manual menggunakan rumus berikut.

error = forecast - actual

Dengan menghitung secara manual seperti di atas, bukanlah itu terlihat sangat mudah? Mari kita hitung satu data.

error = forecast - actual

error = 4.266 - 4.216

error = 0.050

Seperti yang Anda lihat bahwa error yang kita dapatkan sangatlah kecil yaitu 0.05. Jika kita hitung terhadap seluruh data contoh yang ada, hasilnya seperti berikut.

ActualForecastError

4.216

4.266

0.050

5.36

5.415

0.055

5.374

5.437

0.063

5.388

5.338

\-0.05

Tentunya dengan segala kemudahan yang ada, metrik evaluasi di atas memiliki sebuah kelemahan yaitu rentan terhadap hasil negatif (minus) dan juga outlier. Lalu, bagaimana dengan metrik evaluasi yang lainnya? Yuk, kita bahas satu per satu.

#### Mean Absolute Error

Mean Absolute Error (MAE) berfungsi untuk mengukur seberapa dekat hasil prediksi suatu model dengan nilai sebenarnya. MAE mengukur rata-rata dari selisih absolut antara prediksi model dan nilai sebenarnya dari data yang diamati. Alih-alih membiarkan nilai apa adanya, pada MAE setiap nilai yang diambil sifatnya absolut sehingga nilai negatif hilang. Berikut adalah penjelasan detail tentang Mean Absolute Error.

MAE dihitung dengan menjumlahkan selisih absolut antara setiap prediksi individu dan nilai sebenarnya, kemudian dibagi dengan jumlah total observasi yang dapat direpresentasikan sebagai berikut.

Keterangan:

*   n adalah jumlah total observasi atau sampel.
    
*   yi adalah nilai aktual atau nilai sebenarnya dari observasi ke-i.
    
*   Ŷi adalah nilai prediksi model untuk observasi ke-i.
    

Dengan menggunakan MAE, kita memiliki beberapa keuntungan seperti berikut.

*   Interpretasi yang Sederhana: MAE memiliki interpretasi yang sederhana dan mudah dimengerti.
    
*   Robust terhadap Outlier: MAE tidak terlalu sensitif terhadap outlier dalam data karena menggunakan nilai absolut.
    

Diferensial: MAE dapat dengan mudah dihitung dan diferensial, membuatnya cocok untuk digunakan dalam proses optimasi.

#### Mean Square Error

Mean Square Error (MSE) adalah salah satu metrik evaluasi yang umum digunakan dalam statistik dan machine learning. Fungsi dari MSE adalah untuk mengukur seberapa baik suatu model dalam memetakan nilai prediksi ke nilai sebenarnya dengan menggunakan kuadrat kesalahan sebagai dasar perhitungan. MSE merupakan metrik yang sangat populer di kalangan machine learning engineer. 

Pada MSE, kita memangkatkan seluruh error, kemudian menghitung rata-ratanya. Kenapa dipangkatkan? Karena error yang bernilai negatif dapat diubah menjadi positif. Bayangkan jika kita memiliki error katakanlah 2 dan -2. Jika kita menjumlahkan kedua error tersebut, hasilnya adalah 0 yang menunjukkan bahwa tidak ada error. Dengan memangkatkan 2 dan -2, nilai tersebut menjadi 4 dan 4. Ketika menjumlahkannya, error kita bukan 0 melainkan 8. Berikut rumus yang digunakan untuk menghitung MSE.

Keterangan:

*   n adalah jumlah total observasi atau sampel.
    
*   yi adalah nilai aktual atau nilai sebenarnya dari observasi ke-i.
    
*   Ŷi adalah nilai prediksi model untuk observasi ke-i.
    

Keuntungan menggunakan MSE yaitu memiliki perhitungan derivatif yang mudah. MSE memiliki turunan matematis yang mudah dan membuatnya cocok untuk digunakan dalam proses optimasi.

Namun, MSE memiliki sebuah kekurangan yaitu MSE sangat sensitif terhadap outlier dalam data karena kuadrat kesalahan dapat memberikan bobot yang sangat besar pada nilai yang jauh dari rata-rata.

#### Root Mean Square error

Root Mean Square Error (RMSE) adalah salah satu metrik evaluasi yang sering digunakan dalam pemodelan statistik dan machine learning, Fungsi dari RMSE adalah untuk mengukur seberapa baik suatu model memetakan nilai prediksi ke nilai sebenarnya dengan menghitung akar kuadrat dari rata-rata dari kuadrat kesalahan. RMSE dihitung dengan mengambil akar kuadrat dari rata-rata dari kuadrat selisih antara setiap prediksi individu dan nilai sebenarnya.

Keterangan:

*   n adalah jumlah total observasi atau sampel.
    
*   yi adalah nilai aktual atau nilai sebenarnya dari observasi ke-i.
    
*   Ŷi adalah nilai prediksi model untuk observasi ke-i.
    

Kurang lebihnya RMSE memiliki karakteristik yang mirip dengan MSE sehingga memiliki kelebihan dan kekurangan yang serupa juga. Mari kita langsung beranjak ke contoh perhitungan menggunakan RMSE sebagai metrik evaluasi.

#### Mean Absolute Percentage Error

Mean Absolute Percentage Error (MAPE) adalah metrik evaluasi yang digunakan untuk mengukur seberapa baik suatu model memprediksi dengan mengevaluasi rata-rata persentase kesalahan absolut dari semua prediksi terhadap nilai sebenarnya. MAPE umumnya digunakan dalam konteks ramalan atau prediksi di mana penting untuk memahami seberapa besar kesalahan relatif dari prediksi terhadap nilai sebenarnya. MAPE dihitung dengan menjumlahkan persentase kesalahan absolut dari setiap prediksi data dan nilai sebenarnya, kemudian dibagi dengan jumlah total observasi

Keterangan

*   n adalah jumlah total observasi atau sampel.
    
*   yi adalah nilai aktual atau nilai sebenarnya dari observasi ke-i.
    
*   Ŷi adalah nilai prediksi model untuk observasi ke-i.
    

Keuntungan menggunakan MSE yaitu memiliki interpretasi yang mudah dimengerti dalam bentuk persentase sehingga mudah untuk dicerna dan dievaluasi oleh developer.

Namun, dengan menggunakan MAPE, ada sebuah kelemahan yaitu MAPE tidak stabil ketika terdapat nilai sebenarnya yang mendekati nol karena pembaginya adalah nilai sebenarnya. Kesimpulannya, penggunaan MAPE mungkin tidak cocok untuk kasus ketika nilai sebenarnya memiliki variabilitas yang rendah atau mendekati nol.

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
        
3.  Fine-Tuning
    
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
    

Rangkuman Sistem Rekomendasi
----------------------------

#### Pengenalan Sistem Rekomendasi

Apa sebenarnya sistem rekomendasi itu? Frank Kane, salah satu pionir Sistem Rekomendasi dalam course [Building Recommender Systems with Machine Learning and AI](https://learning.oreilly.com/videos/building-recommender-systems/9781789803273/)  mendefinisikannya sebagai berikut.

“_A system that predicts ratings or preferences a user might give to a product. Often these are sorted and presented as “top-N'' recommendations. Also known as recommender engines, recommendation systems, and recommendation platforms_”

Sistem rekomendasi memprediksi rating atau preferensi pengguna terhadap item tertentu. Rekomendasi ini dibuat berdasarkan perilaku pengguna di masa lalu atau perilaku pengguna lainnya. Jadi, sistem ini akan merekomendasikan sesuatu terhadap pengguna berdasarkan data perilaku atau preferensi dari waktu ke waktu. 

Secara umum, ada dua buah jenis rekomendasi yang sering digunakan, yaitu rekomendasi beranda dan rekomendasi produk terkait. 

Rekomendasi beranda adalah rekomendasi yang umum kita temui sehari-hari. Contohnya seperti ketika Anda membuka halaman Google Play Store, di sana akan terlihat aplikasi yang mungkin menarik minat Anda. Begitu juga pada layanan streaming seperti Netflix. Ketika mengunjungi beranda, terdapat film-film yang mungkin menarik untuk Anda tonton. 

Di lain sisi, rekomendasi produk terkait preferensi pengguna sering kali kita temui pada _e-commerce_. Contohnya, jika Anda menggunakan Tokopedia dan mencari sebuah item, di sana akan terlihat produk lain yang terkait dengan produk yang sedang atau pernah Anda cari. 

Sebagai informasi, ada dua pendekatan utama dalam membangun sebuah sistem rekomendasi, yaitu _Content-Based Filtering_ (CBF) dan _Collaborative Filtering_ (CF). Perbedaan utama antara CF dan CBF adalah dalam sumber informasi yang digunakan untuk memberikan rekomendasi. CF menggunakan informasi dari aktivitas pengguna (misalnya, penilaian atau histori pembelian), sementara CBF menggunakan informasi dari fitur-fitur atau karakteristik item tersebut (misalnya, genre untuk film atau atribut-atribut produk untuk barang dagangan).

#### Collaborative Filtering

Collaborative filtering merupakan sebuah pendekatan yang menggunakan informasi dari aktivitas pengguna untuk memberikan rekomendasi. CF mencoba menemukan pola dan hubungan antara pengguna dan item. Secara umum terdapat dua jenis CF:

1.  **Collaborative Filtering Berbasis Pengguna (**_**User-Based**_ **CF):** mengidentifikasi pengguna yang memiliki preferensi serupa dengan pengguna yang aktif saat ini, lalu merekomendasikan item yang disukai oleh pengguna tersebut. Pendekatan ini bergantung pada kesamaan antar pengguna.
    
2.  **Collaborative Filtering Berbasis Item (**_**Item-Based**_ **CF):** mengidentifikasi item yang sering disukai oleh pengguna yang memiliki preferensi serupa dengan pengguna yang aktif saat ini, lalu merekomendasikan item tersebut. Pendekatan ini bergantung pada kesamaan antar item.(a). user based; (b). item based 
    

#### Content Based Filtering

Content-Based Filtering (CBF) adalah pendekatan dalam sistem rekomendasi yang menggunakan karakteristik atau fitur dari item serta profil preferensi pengguna untuk memberikan rekomendasi.

Dalam CBF, item-item direkomendasikan kepada pengguna berdasarkan kesamaan antara item yang ada dan item yang disukai pengguna sebelumnya. Ini berarti jika seorang pengguna menyukai item tertentu, sistem akan mencoba merekomendasikan item lain yang memiliki fitur atau karakteristik yang mirip dengan item yang disukai tersebut.

Misalnya, dalam sistem rekomendasi gim, fitur-fitur seperti genre, sudut pandang pemain, pembuat, dan plot dapat digunakan untuk menggambarkan setiap gim. Ketika seorang pengguna menyukai gim tertentu, sistem akan mencari gim lain yang memiliki fitur-fitur yang mirip dengan gim yang disukai oleh pengguna tersebut. Jika seorang pengguna menyukai gim FPS dengan genre tertentu, sistem akan mencoba merekomendasikan gim FPS lain yang juga memiliki pembuat yang sama atau genre yang serupa.

Keuntungan dari CBF adalah tidak memerlukan informasi dari pengguna lain, hanya memerlukan informasi tentang item itu sendiri. Ini membuat CBF lebih cocok untuk situasi di mana data pengguna terbatas atau di mana privasi pengguna menjadi perhatian utama.

Namun, kelemahan dari CBF adalah kurangnya kemampuan untuk merekomendasikan item yang tidak memiliki fitur yang sama dengan item yang disukai pengguna sebelumnya. Ini dapat menghasilkan kurangnya variasi dalam rekomendasi dan membuat pengguna kehilangan kesempatan untuk menemukan item baru yang mungkin tidak memiliki fitur yang sama dengan item yang disukai sebelumnya.

Rangkuman Reinforcement Learning
--------------------------------

### Pengenalan Reinforcement Learning

**Reinforcement Learning (RL)** adalah cabang pembelajaran mesin yang berfokus pada cara agen belajar mengambil tindakan dalam lingkungan untuk memaksimalkan hadiah (reward) yang diterima. Agen belajar melalui percobaan dan kesalahan, memperbarui pengetahuannya tentang tindakan yang lebih baik berdasarkan hasil dari tindakan tersebut.

### Perbedaan RL dengan Supervised dan Unsupervised Learning

*   **Supervised Learning**: Agen belajar dari contoh data yang telah dilabeli (input-output pairs). Contoh: mengenali gambar kucing dari gambar-gambar yang sudah dilabeli "kucing".
    
*   **Unsupervised Learning**: Agen tidak diberikan label dan bertujuan menemukan pola tersembunyi dalam data. Contoh: pengelompokan data (clustering).
    
*   **Reinforcement Learning**: Agen belajar dari pengalaman interaktif dengan lingkungan, menerima reward atau hukuman berdasarkan tindakan yang diambil, dan belajar strategi terbaik untuk memaksimalkan hadiah.
    

### Contoh Sederhana: Agen yang Belajar Bermain Game

**Permainan Tic-Tac-Toe**: Agen adalah pemain yang belajar cara terbaik untuk menang. Papan permainan adalah lingkungan dan tindakan adalah penempatan tanda dalam kotak yang tersedia. Hadiah diberikan berdasarkan hasil permainan: menang (reward positif), kalah (reward negatif), atau seri (tidak ada perubahan). Agen belajar dari bermain berulang kali, baik melawan lawan atau dirinya sendiri, dan secara bertahap mengembangkan strategi yang lebih baik untuk menang melalui percobaan dan kesalahan, mirip dengan cara manusia belajar.

### Komponen-komponen Utama dalam Reinforcement Learning (RL)

1.  **Agent (Agen)**: Agen adalah entitas yang belajar dan bertindak untuk mencapai tujuan tertentu. Contohnya seorang pelajar yang belajar bermain catur.
    
2.  **Environment (Lingkungan)**: Dunia tempat agen beroperasi dan berinteraksi. Contohnya papan catur tempat permainan berlangsung.
    
3.  **Action (Tindakan)**: Langkah-langkah yang dapat diambil agen dalam lingkungannya untuk mencapai tujuan. Contohnya gerakan atau keputusan dalam permainan catur, seperti memindahkan bidak atau melakukan strategi tertentu. 
    
4.  **Rewards (Hadiah)**: Umpan balik kepada agen berdasarkan tindakan yang diambilnya. Contohnya hasil dari pertandingan catur, seperti kemenangan (reward positif) yang memberikan pujian atau rasa bangga, atau kekalahan (reward negatif) yang memberikan rasa kecewa atau kesempatan untuk belajar dari kesalahan.
    

### Markov Decision Process (MDP)

**MDP** adalah kerangka kerja pengambilan keputusan yang memodelkan suatu lingkungan dengan komponen-komponen yang membantu agen dalam membuat keputusan optimal meskipun ada ketidakpastian.

**Komponen Utama MDP**

1.  **State (Keadaan)**:
    
    *   Representasi situasi atau kondisi saat ini di lingkungan.
        
    *   Contoh: Posisi bidak dalam permainan catur atau lokasi dan orientasi robot dalam navigasi.
        
2.  **Action (Tindakan)**:
    
    *   Langkah yang dapat diambil oleh agen dalam suatu state.
        
    *   Contoh: Langkah bidak dalam catur atau gerakan robot seperti maju, berbelok, atau berhenti.
        
3.  **Transition Model (Model Transisi)**:
    
    *   Fungsi yang menentukan probabilitas berpindah dari satu state ke state lain setelah tindakan tertentu diambil.
        
    *   Contoh: Probabilitas langkah yang mungkin jika bidak dipindahkan dalam catur atau kemungkinan berpindah ke lokasi berbeda setelah langkah robot.
        
4.  **Reward (Hadiah)**:
    
    *   Nilai yang diterima agen setelah melakukan tindakan tertentu dan berpindah dari satu state ke state lainnya.
        
    *   Contoh: Kemenangan atau kekalahan dalam catur atau pencapaian tujuan dalam navigasi robot.
        
5.  **Policy (Kebijakan)**:
    
    *   Strategi atau aturan yang menentukan tindakan yang harus diambil oleh agen dalam setiap state.
        
    *   Contoh: Aturan penentu langkah dalam catur atau algoritma yang menentukan langkah robot untuk mencapai tujuan.
        

**Cara Kerja MDP**

1.  **Representasi Environment**: Mendefinisikan dan memetakan lingkungan dalam serangkaian state yang mungkin terjadi. Transisi dari satu state ke state lain hanya bergantung pada state saat ini dan tindakan yang diambil, mematuhi prinsip Markov.
    
2.  **Penentuan Action atau Aksi**: Agen memutuskan tindakan yang akan diambil pada setiap state, mempertimbangkan kebijakan yang didefinisikan atau menggunakan algoritma pencarian tindakan optimal.
    
3.  **Evaluasi Transisi**: Setelah memilih tindakan, agen melakukan langkah ke state baru berdasarkan model transisi yang menentukan probabilitas berpindah dari satu state ke state lain.
    
4.  **Perhitungan Reward**: Agen menerima reward terkait transisi ke state baru, memberikan umpan balik atas keberhasilan atau kegagalan tindakan. Reward dapat positif, negatif, atau nol.
    
5.  **Pembaruan Kebijakan**: Agen memperbarui kebijakan atau strategi berdasarkan reward yang diterima untuk meningkatkan kinerja dan memaksimalkan reward jangka panjang, menggunakan algoritma pembelajaran seperti Q-learning atau metode pembelajaran berbasis kebijakan.
    
6.  **Pengambilan Keputusan Berulang**: Proses berulang ketika agen berinteraksi dengan lingkungan: memilih tindakan, menerima reward, memperbarui kebijakan, dan memperbaiki kinerja berdasarkan pengalaman baru.
    
7.  **Mencari Kebijakan Optimal**: Agen mencoba menemukan kebijakan optimal yang memberikan reward terbesar dalam jangka panjang menggunakan metode seperti iterasi nilai (value iteration) atau iterasi kebijakan (policy iteration).
    

Dengan memahami komponen dan cara kerja MDP, kita dapat merancang agen yang mampu membuat keputusan optimal dalam berbagai konteks, mulai dari permainan hingga robotika dan manajemen operasional.

### Q-Learning

**Q-Learning** adalah algoritma dalam pembelajaran penguatan yang mengajarkan agen cara membuat keputusan optimal saat berinteraksi dengan lingkungan. Tujuan utamanya adalah mempelajari nilai-nilai Q yang memperkirakan manfaat dari tindakan tertentu dalam keadaan tertentu, sehingga agen dapat memilih tindakan yang paling menguntungkan.

**Komponen Utama Q-Learning**

1.  **State (Keadaan)**: Representasi dari situasi atau kondisi saat ini dalam lingkungan.
    
2.  **Action (Tindakan)**: Langkah yang dapat diambil oleh agen dalam keadaan tertentu.
    
3.  **Reward (Hadiah)**: Nilai numerik yang mencerminkan keuntungan atau kerugian setelah agen mengambil tindakan tertentu dalam keadaan tertentu.
    
4.  **Q-table**: Tabel dua dimensi yang menyimpan nilai-nilai Q, di mana setiap sel mewakili pasangan keadaan-tindakan dan berisi estimasi manfaat dari tindakan tersebut.
    
5.  **Exploration vs Exploitation**: Strategi memilih tindakan; eksplorasi mencoba tindakan baru untuk menjelajahi lingkungan, sementara eksploitasi memilih tindakan dengan nilai Q tertinggi berdasarkan pengetahuan yang ada.
    

**Cara Kerja Q-Learning**

1.  **Inisialisasi Tabel Q**: Tabel Q diinisialisasi dengan nilai acak atau default.
    
2.  **Memilih Tindakan**: Agen memilih tindakan berdasarkan strategi ε-greedy, yaitu memilih tindakan secara acak dengan probabilitas ε untuk eksplorasi dan tindakan dengan nilai Q tertinggi dengan probabilitas (1-ε) untuk eksploitasi.
    
3.  **Melakukan Tindakan**: Agen melaksanakan tindakan yang dipilih di lingkungan.
    
4.  **Mengukur Hadiah**: Agen menerima hadiah dari lingkungan berdasarkan tindakan yang dilakukan.
    
5.  **Memperbarui Tabel Q**: Agen memperbarui nilai Q menggunakan rumus Q-learning yang memperhitungkan hadiah yang diterima, tingkat pembelajaran (α), dan faktor diskon (γ).
    
6.  **Pengambilan Keputusan Berulang**: Proses di atas diulang terus menerus, memungkinkan agen untuk belajar dari pengalaman dan menyempurnakan nilai Q dalam tabel.
    
7.  **Mencari Kebijakan Optimal**: Dengan menggunakan metode seperti iterasi nilai atau iterasi kebijakan, agen mencoba menemukan kebijakan optimal yang memaksimalkan total reward dalam jangka panjang.
    

**Policies and Value Functions dalam MDP**:

*   **Policies (Kebijakan)**:
    
    *   **Deterministic Policy (π)**: Menetapkan tindakan tertentu untuk setiap state.
        
    *   **Stochastic Policy (π)**: Menentukan probabilitas berbagai tindakan pada setiap state.
        
*   **Value Functions (Fungsi Nilai)**:
    
    *   **State Value Function (V(s))**: Mengevaluasi seberapa bernilai suatu state jika mengikuti kebijakan π dari state tersebut.
        
    *   **Action Value Function (Q(s, a))**: Mengevaluasi seberapa bernilai tindakan tertentu diambil pada suatu state jika kemudian mengikuti kebijakan π.
        

Value functions mempertimbangkan faktor diskonto (γ) yang menentukan pentingnya reward di masa depan dibandingkan reward saat ini, membantu agen mengevaluasi berbagai tindakan untuk memaksimalkan total reward yang diharapkan.

### Exploration vs Exploitation pada Markov Decision Processes (MDPs)

Saat beroperasi dalam MDPs, ada dua strategi utama yang sering dibahas: eksplorasi dan eksploitasi. Eksplorasi melibatkan upaya untuk mengeksplorasi lingkungan dengan mencoba tindakan baru dalam memahami lebih baik tentang dampaknya. Di sisi lain, eksploitasi terfokus pada penggunaan pengetahuan yang sudah ada dalam memilih tindakan untuk memberikan hasil terbaik berdasarkan pengalaman sebelumnya.

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

1.  Menggunakan CDN (Content Distribution Network)Anda dapat menambahkan script TensorFlow.js langsung ke HTML menggunakan tag \`\`. Class TensorFlow.js bisa diakses menggunakan objek \`tf\`.</div></li><li class="slate-li"><div style="position:relative">Menggunakan package manager (npm atau yarn)Jika Anda menggunakan Node.js atau ingin manajemen dependensi yang lebih baik, instal TensorFlow.js melalui npm atau yarn.</div></li><li class="slate-li"><div style="position:relative">Membuat Model Baru dengan TensorFlow.jsTensorFlow.js menyediakan dua cara untuk membuat model machine learning di JavaScript menggunakan Layers API yaitu Sequential Model dan Functional Model.</div></li><li class="slate-li"><div style="position:relative">Konversi Model TensorFlow ke TensorFlow.jsAnda dapat mengonversi model TensorFlow ke TensorFlow.js menggunakan \`tensorflowjs\_converter\`.</div></li></ol><p class="slate-paragraph"> </p><h3 class="slate-h3">Memuat Model TensorFlow.js di Browser</h3><p class="slate-paragraph">Untuk memuat model yang telah dikonversi ke TensorFlow.js di browser, Anda dapat menggunakan \`tf.loadLayersModel()\` atau \`tf.loadGraphModel()\`. Pastikan Anda menjalankan web server lokal untuk memuat model ini dari http. Setelah dimuat, Anda dapat menggunakan model untuk melatih ulang, evaluasi, atau mengambil prediksi langsung dari data yang diberikan.</p><p class="slate-paragraph"></p><h3 class="slate-h3">Konversi model TensorFlow ke TensorFlow.js</h3><ol class="slate-ol"><li class="slate-li"><div style="position:relative">Konversi dari SavedModel TensorFlow ke TensorFlow.js</div></li><li class="slate-li"><div style="position:relative">Konversi dari Keras HDF5 ke TensorFlow.js</div></li><li class="slate-li"><div style="position:relative">Konversi dari Frozen Model TensorFlow ke TensorFlow.js</div></li><li class="slate-li"><div style="position:relative">Konversi dari TensorFlow Hub ke TensorFlow.jS</div></li><li class="slate-li"><div style="position:relative">Memuat Model TensorFlow.js di Browser</div></li></ol><p class="slate-paragraph">Pastikan menjalankan kode ini di server HTTP untuk memuat model TensorFlow.js. Dengan langkah-langkah ini, Anda dapat mengonversi model TensorFlow dan memuatnya di browser untuk penggunaan dalam training ulang, evaluasi, atau inferensi.</p><p class="slate-paragraph"></p><h2 class="slate-h2">Pengenalan TensorFlow Lite</h2><p class="slate-paragraph">TensorFlow Lite (TF-Lite) adalah sebuah framework yang memungkinkan eksekusi model TensorFlow pada perangkat mobile dan IoT. TF-Lite dirancang untuk mengoptimalkan ukuran model dan meningkatkan performa inferensi pada perangkat dengan sumber daya terbatas seperti smartphone, tablet, dan perangkat IoT.</p><p class="slate-paragraph">Beberapa kegunaan TensorFlow Lite termasuk.</p><ol class="slate-ol"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Google Translate Instant Camera Translation</strong>: Menerjemahkan teks langsung dari foto, membantu pengguna memahami bahasa asing secara instan tanpa koneksi internet.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Fitur Makeup Virtual di Aplikasi E-commerce</strong>: Memungkinkan pengguna untuk mencoba produk makeup secara virtual, membantu dalam pemilihan warna dan tampilan produk makeup.</div></li></ol><p class="slate-paragraph">Keuntungan utama dari penggunaan TensorFlow Lite meliputi.</p><ol class="slate-ol"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Penggunaan Offline</strong>: Tidak memerlukan koneksi internet untuk melakukan prediksi, menjaga privasi pengguna.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Ukuran dan Latensi Kecil</strong>: Mengoptimalkan ukuran binary model dan mengurangi konsumsi daya saat melakukan prediksi.</div></li></ol><p class="slate-paragraph">Untuk menggunakan TensorFlow Lite, prosesnya melibatkan konversi model TensorFlow ke format TensorFlow Lite (\`.tflite\`) menggunakan TFLite Converter, yang kemudian dapat dieksekusi menggunakan TensorFlow Lite Interpreter di perangkat mobile atau IoT.</p><p class="slate-paragraph">Berikut adalah langkah-langkah umum untuk mengonversi model TensorFlow menjadi TensorFlow Lite (\`.tflite\`).</p><p class="slate-paragraph"></p><h3 class="slate-h3">Konversi Model ke TensorFlow Lite</h3><ol class="slate-ol"><li class="slate-li"><div style="position:relative">Konversi dari SavedModel TensorFlow ke TensorFlow Lite.</div></li><li class="slate-li"><div style="position:relative">Konversi dari Keras HDF5 ke TensorFlow Lite.</div></li></ol><p class="slate-paragraph">Setelah model dikonversi ke format \`.tflite\`, model ini dapat dimuat dan dieksekusi menggunakan TensorFlow Lite Interpreter di lingkungan seperti aplikasi Android atau perangkat IoT yang didukung.</p><p class="slate-paragraph"></p><h2 class="slate-h2">Pengenalan TensorFlow Serving (TF-Serving)</h2><p class="slate-paragraph">TensorFlow Serving (TF-Serving) adalah sistem server yang memfasilitasi deployment model machine learning pada server dengan menyediakan fleksibilitas dalam mengelola beberapa versi model sekaligus melalui arsitektur yang terstruktur. Pengguna dapat melakukan prediksi menggunakan model yang tersedia melalui servable handler, dengan pengaturan versi model yang dikelola oleh model manager dalam TF-Serving.</p><p class="slate-paragraph"></p><h3 class="slate-h3">Persiapan TensorFlow Serving</h3><ol class="slate-ol"><li class="slate-li"><div style="position:relative">Instalasi Docker. </div></li><li class="slate-li"><div style="position:relative">Menyiapkan Kebutuhan Sistem pada Docker.</div></li><li class="slate-li"><div style="position:relative">Instalasi TensorFlow Serving Python API.</div></li></ol><p class="slate-paragraph">Setelah langkah-langkah di atas selesai, sistem Anda sudah siap untuk menggunakan TensorFlow Serving untuk deployment model machine learning pada server. Langkah selanjutnya adalah berlatih menjalankan model menggunakan TensorFlow Serving. </p><p class="slate-paragraph"> </p><h2 class="slate-h2">Federated Learning (FL)</h2><p class="slate-paragraph">Federated Learning (FL) adalah pendekatan modern dalam pembelajaran mesin yang mengatasi beberapa masalah utama dari sistem tradisional yang terpusat, seperti privasi, latensi, dan keterbatasan koneksi. Dalam FL, pelatihan model dilakukan secara terdistribusi di perangkat client yang menggunakan data lokal mereka. Model yang dihasilkan dari setiap client kemudian diagregasikan dan dikumpulkan kembali ke server, tanpa perlu mengungkapkan data pribadi client.</p><p class="slate-paragraph"></p><h3 class="slate-h3">Tahapan dalam Federated Learning:</h3><ol class="slate-ol"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Pelatihan Model di Perangkat Client</strong>: Setiap perangkat client melakukan pelatihan model dengan menggunakan data lokalnya.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Aggregasi Model di Server</strong>: Model dari setiap client diagregasikan dan dikumpulkan kembali ke server.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Privasi dan Keamanan</strong>: Federated Learning menerapkan beberapa teknologi keamanan, seperti enkripsi data pada perangkat, agregasi aman untuk melindungi data yang dikirimkan, dan penghapusan data setelah digunakan.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Federated Model Averaging</strong>: Teknik ini digunakan untuk menghitung rata-rata parameter model dari setiap client, yang mencerminkan kontribusi dari berbagai data lokal tanpa mengungkapkan data tersebut secara langsung.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">TensorFlow Federated (TFF)</strong>: TensorFlow Federated menyediakan API untuk implementasi FL, termasuk pengaturan training dan evaluasi yang dapat diterapkan pada model data yang ada.</div></li></ol><p class="slate-paragraph"></p><h2 class="slate-h2">TensorFlow Data Services (TFDS) untuk Data Pipelines</h2><p class="slate-paragraph">TensorFlow Data Services (TFDS) membantu mengelola data pada machine learning dengan menyediakan platform yang mudah diakses untuk mengintegrasikan dataset ke dalam pipeline training TensorFlow. Ini memfasilitasi:</p><ul class="slate-ul"><li class="slate-li"><div style="position:relative">Ekstraksi data dari sumber berbeda dan transformasi menjadi format yang digunakan untuk training.</div></li><li class="slate-li"><div style="position:relative">Pengelolaan dataset dengan API konsisten untuk meminimalkan perbedaan dan memudahkan penggunaan.</div></li><li class="slate-li"><div style="position:relative">Mempercepat proses training dengan dukungan GPU/TPU dan fleksibilitas dalam menangani berbagai jenis data.</div></li></ul><p class="slate-paragraph">Dengan TFDS, pengguna dapat fokus pada pengembangan model dan optimisasi tanpa harus khawatir tentang masalah ekstraksi, transformasi, atau konsistensi dataset.</p><p class="slate-paragraph"> </p><h2 class="slate-h2">Export Data ke Training Pipelines</h2><h3 class="slate-h3">Mengubah Dataset Menjadi Format TFDS</h3><ol class="slate-ol"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Import Library: </strong>Import TensorFlow, Pandas, dan library lainnya yang dibutuhkan untuk pemrosesan data.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Baca File CSV: </strong>Gunakan Pandas DataFrame untuk membaca file CSV yang diunduh dari Kaggle.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Split Dataset: </strong>Bagi dataset menjadi training, validation, dan test set. Definisikan kolom target (0 = low, 1 = high) berdasarkan harga berlian.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Bungkus DataFrame dengan tf.data: </strong>Gunakan tf.data untuk membuat dataset dari DataFrame. Ini memungkinkan penggunaan feature column sebagai jembatan dari DataFrame menjadi fitur yang digunakan untuk training model.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Feature Columns: </strong>Ada beberapa jenis feature column:</div><ul class="slate-ul"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Numeric Column:</strong> Representasi sederhana dari fitur numerik.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Bucketized Column:</strong> Membagi nilai numerik menjadi beberapa bucket.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Categorical Column:</strong> Mengubah nilai string menjadi angka.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Embedding Column:</strong> Representasi categorical column dengan nilai yang beragam.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Hashed Feature Column:</strong> Alternatif representasi categorical column dengan banyak jenis value.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Crossed Feature Column:</strong> Menggabungkan beberapa feature column menjadi satu.</div></li></ul></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Buat Feature Layer: </strong>Pilih feature column yang akan digunakan dan buat feature layer sebagai input dalam model tf.Keras.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Create, Compile, and Train Model: </strong>Tulis kode untuk membuat, meng-compile, dan melatih model menggunakan TensorFlow.</div></li></ol><p class="slate-paragraph"></p><h3 class="slate-h3">Mempublikasi Model ke TensorHub</h3><ol class="slate-ol"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Membuat dan Mengekspor Model: </strong>Simpan model yang sudah dilatih dalam format .pb dan simpan dalam direktori penyimpanan model yang sesuai.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Packaging Model: </strong>Kompres model dalam format .tar.gz untuk menghemat traffic jaringan.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Menulis Dokumentasi: </strong>Buat file markdown yang menjelaskan model, termasuk metadata penting seperti asset-path, module-type, fine-tunable, dan format model.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Membuat Permintaan Publikasi: </strong>Lakukan push file model ke repositori TensorFlow Hub melalui Git CLI atau GitHub GUI, dan buat pull request untuk mempublikasikan model.</div></li></ol><p class="slate-paragraph"> </p><h2 class="slate-h2">Pengenalan TensorBoard</h2><p class="slate-paragraph">TensorBoard adalah alat visualisasi data dan parameter dalam pembelajaran mesin yang berfungsi untuk memantau dan memahami model machine learning. TensorBoard dapat menampilkan metrik seperti loss dan akurasi, visualisasi grafik model, histogram parameter, proyeksi embedding, visualisasi gambar, teks, dan data audio. TensorBoard juga memungkinkan kolaborasi tim dan publikasi eksperimen melalui Tensorboard.dev.</p><p class="slate-paragraph"></p><h3 class="slate-h3">Elemen Fungsional pada TensorBoard</h3><ol class="slate-ol"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Scalars</strong>: Menampilkan perubahan loss dan metrik lainnya selama training. Membantu dalam memantau overfitting dan waktu training.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Graphs</strong>: Memvisualisasikan struktur model dan detail layer.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Distributions dan Histograms</strong>: Memantau perubahan parameter seperti bias dan bobot selama training.</div></li></ol><p class="slate-paragraph"></p><h3 class="slate-h3">Setup TensorBoard</h3><ol class="slate-ol"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Mengaktifkan TensorBoard</strong>: Gunakan %load\_ext tensorboard di Notebook atau Colab.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Membuat File Log</strong>:</div><ul class="slate-ul"><li class="slate-li"><div style="position:relative">Buat direktori log dengan datetime untuk nama unik.</div></li><li class="slate-li"><div style="position:relative">Buat file log dengan tf.summary.create\_file\_writer("./logs/").</div></li></ul></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Callback TensorBoard</strong>: Tambahkan tf.keras.callbacks.TensorBoard() pada model.fit() untuk menghasilkan log selama training.</div></li></ol><h3 class="slate-h3">TensorBoard Lokal</h3><ul class="slate-ul"><li class="slate-li"><div style="position:relative">Jalankan %tensorboard --logdir logs/fit untuk menampilkan TensorBoard di dalam Colab.</div></li></ul><h3 class="slate-h3">Tensorboard.dev</h3><ul class="slate-ul"><li class="slate-li"><div style="position:relative">Unggah log ke Tensorboard.dev dengan !tensorboard dev upload --logdir logs/fit.</div></li></ul><h3 class="slate-h3">Menampilkan Gambar</h3><ul class="slate-ul"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Gambar Tunggal</strong>: Gunakan tf.summary.image() untuk menampilkan gambar dari dataset.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Banyak Gambar</strong>: Gunakan tf.summary.image() dengan max\_outputs untuk menampilkan beberapa gambar sekaligus.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Gambar dari Plot</strong>: Gunakan fungsi plot\_to\_image untuk mengonversi plot Matplotlib ke gambar yang bisa dilog oleh TensorBoard.</div></li></ul><h3 class="slate-h3">Menampilkan Confusion Matrix</h3><ol class="slate-ol"><li class="slate-li"><div style="position:relative">Buat plot confusion matrix dengan plot\_confusion\_matrix().</div></li><li class="slate-li"><div style="position:relative">Log matrix setiap epoch menggunakan callback LambdaCallback.</div></li></ol><p class="slate-paragraph"></p><h2 class="slate-h2">Memonitor Model</h2><p class="slate-paragraph">Model monitoring penting untuk memantau kinerja model dalam fase produksi. Ini melibatkan pemantauan akurasi, latensi, penggunaan memori/CPU, dan penurunan kinerja model seiring waktu (model drift). Dua jenis penurunan kinerja adalah sudden degradation dan slow degradation. Pemantauan dilakukan oleh tim DevOps dan data scientist.</p><p class="slate-paragraph"></p><h3 class="slate-h3">Metode Evaluasi Model</h3><ul class="slate-ul"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Type 1 Error (False Positive)</strong>: Kesalahan prediksi positif.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Type 2 Error (False Negative)</strong>: Kesalahan prediksi negatif.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Akurasi</strong>: Proporsi prediksi yang benar.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Presisi</strong>: Proporsi identifikasi kelas positif yang benar.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Recall</strong>: Proporsi kelas positif yang diklasifikasi dengan benar.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Mean Squared Error (MSE)</strong>: Rerata loss pada setiap baris data.</div></li></ul><p class="slate-paragraph"></p><h2 class="slate-h2">Pembaruan Model</h2><ul class="slate-ul"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Manual Retraining</strong>: Training ulang model secara manual.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Continuous Learning</strong>: Training ulang otomatis berdasarkan data baru.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Pengujian A/B</strong>: Membandingkan dua versi model untuk menentukan yang lebih baik.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Multi Armed Bandit (MAB)</strong>: Pengujian A/B yang dinamis untuk mengoptimalkan kinerja model secara terus-menerus.</div></li></ul><p class="slate-paragraph"></p><h3 class="slate-h3">Prinsip Kunci dalam Pemantauan Model</h3><ol class="slate-ol"><li class="slate-li"><div style="position:relative">Monitor perubahan dependency.</div></li><li class="slate-li"><div style="position:relative">Monitor perbedaan data training dan live data.</div></li><li class="slate-li"><div style="position:relative">Monitor fitur pada training dan penyajian model.</div></li><li class="slate-li"><div style="position:relative">Monitor perbaruan model.</div></li><li class="slate-li"><div style="position:relative">Monitor kestabilan model.</div></li><li class="slate-li"><div style="position:relative">Optimalkan penggunaan resource seperti RAM dan latency.</div></li></ol><p class="slate-paragraph">Dengan memahami dan menerapkan langkah-langkah ini, kita dapat memastikan kinerja model machine learning tetap optimal dan relevan dengan perubahan data serta lingkungan operasional.</p><h2 class="slate-h2">Rangkuman The Game Changer: Generative AI</h2><p class="slate-paragraph"></p><h3 class="slate-h3">Pengenalan Generative AI</h3><p class="slate-paragraph">Generative AI adalah sebuah subbidang dari machine learning yang fokus pada kemampuan mesin untuk menghasilkan konten baru yang kreatif dan realistis. Teknologi ini memungkinkan mesin untuk menciptakan teks, gambar, musik, dan bahkan video yang belum pernah ada sebelumnya, seolah-olah dibuat oleh manusia.</p><p class="slate-paragraph"></p><p class="slate-paragraph">Generative AI menggunakan berbagai teknik canggih, termasuk yang telah kita pelajari dalam deep learning, seperti jaringan saraf tiruan, tetapi dengan pendekatan yang sedikit berbeda. Salah satu pendekatan paling populer adalah penggunaan <em class="slate-italic">Generative Adversarial Networks </em>(GAN), <em class="slate-italic">Variational Autoencoders</em> (VAEs) dan<em class="slate-italic"> Large Language Models </em>(LLMs). Ketiga pendekatan tersebut akan kita pelajari lebih pada materi ini.</p><p class="slate-paragraph">Sebelum masuk ke detail teknis, mari kita lihat beberapa contoh nyata dari aplikasi Generative AI:</p><ul class="slate-ul"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Pembuatan Konten Teks:</strong> model seperti GPT (Generative Pre-trained Transformer) yang dapat menghasilkan artikel, cerita pendek, dan bahkan kode pemrograman dengan sedikit atau tanpa campur tangan manusia.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Generasi Gambar dan Video:</strong> penggunaan GAN dalam menciptakan gambar realistis dari deskripsi teks atau memperbaiki kualitas video yang buram.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Musik dan Seni:</strong> AI yang mampu menggubah musik baru dalam gaya komposer terkenal atau membuat karya seni yang menginspirasi.</div></li></ul><p class="slate-paragraph"></p><h3 class="slate-h3">Discriminative AI vs Generative AI</h3><p class="slate-paragraph">Machine learning memiliki posisi sebagai payung besar yang mencakup berbagai metode untuk membuat komputer belajar dari data. Discriminative AI dan deep learning adalah dua pendekatan yang termasuk dalam payung besar ini, sedangkan deep learning adalah bagian dari machine learning yang menggunakan jaringan saraf tiruan yang dalam untuk menganalisis data. </p><p class="slate-paragraph">Lalu, apa itu discriminative AI? Discriminative AI adalah pendekatan dalam machine learning yang fokus pada klasifikasi dan pemisahan data ke dalam kelas-kelas tertentu. Model-model discriminative dapat diterapkan dalam konteks deep learning dengan menggunakan deep neural networks untuk tugas-tugas klasifikasi yang kompleks. </p><p class="slate-paragraph"></p><p class="slate-paragraph">Sebelum membahas tentang Generative AI, mari kita <em class="slate-italic">recall </em>materi tentang AI secara umum. AI adalah salah satu istilah yang menarik, tetapi sering kali samar-samar atau bahkan tertukar dengan machine learning beserta turunannya. Lalu, apa sebenarnya AI?</p><p class="slate-paragraph">Secara keseluruhan artificial intelligence adalah bidang yang luas di mana machine learning dan deep learning adalah pendekatan-pendekatan spesifik yang digunakan untuk menyelesaikan berbagai masalah berdasarkan jenis data dan tujuan analisis. Dengan perkembangan teknologi yang sangat cepat, kini hadir sebuah metode yang dapat membuat sebuah konten berdasarkan history yang sudah ada, yaitu Generative AI. </p><p class="slate-paragraph">Generative AI adalah cabang dari kecerdasan buatan (AI) yang berfokus pada pembuatan atau generasi konten baru yang menyerupai data asli yang digunakan untuk melatih model tersebut. Tidak seperti discriminative AI yang berfokus pada pemodelan keputusan untuk mengklasifikasikan data, generative AI mencoba memahami dan meniru distribusi data yang mendasari sehingga bisa menciptakan data baru yang realistis.</p><p class="slate-paragraph">Secara garis besar teknologi ini memungkinkan mesin untuk menciptakan berbagai jenis data yang menyerupai data yang ada sebelumnya, termasuk teks, gambar, musik, video, dan bahkan kode pemrograman.</p><p class="slate-paragraph"></p><p class="slate-paragraph">Inti dari generative AI adalah kemampuannya untuk memahami dan mereplikasi distribusi data yang kompleks sehingga dapat menggunakan pengetahuan tersebut untuk menciptakan data baru. </p><p class="slate-paragraph">Saat materi ini dibuat, Generative AI merupakan teknologi yang sangat ramai diperbincangkan karena dapat meningkatkan produktivitas mulai dari mencari informasi hingga inspirasi untuk membuat suatu hal. Salah satu contohnya adalah GitHub Copilot yang dapat membantu seorang software developer untuk membangun sebuah sistem mulai dari membuat kerangka kode hingga membantu <em class="slate-italic">debugging</em> kode yang sudah dibangun.</p><p class="slate-paragraph"></p><h3 class="slate-h3">Penerapan Generative AI</h3><p class="slate-paragraph">Salah satu kelebihan dari Generative AI ini adalah dapat membuka peluang baru dalam segi kreativitas dan inovasi dengan lebih cepat dan efisien. Hal ini karena pembuatan konten akan lebih cepat dibandingkan tanpa menggunakan Generative AI.</p><p class="slate-paragraph">Selain itu, Generative AI juga dapat menghasilkan konten dalam skala besar yang bermanfaat dalam industri seperti media, hiburan, dan desain. Penerapan Generative AI dapat ditemui pada berbagai bidang industri dengan data yang sangat beragam mulai dari teks, citra, video, dan multi moda.</p><p class="slate-paragraph"></p><h4 class="slate-h4">Generative AI for Text</h4><p class="slate-paragraph">Generative teks adalah proses ketika AI membuat teks baru berdasarkan input atau prompt yang diberikan. Teknologi ini dapat digunakan dalam berbagai aplikasi, seperti penulisan otomatis, chatbot, penerjemahan bahasa, dan pembuatan konten kreatif.</p><p class="slate-paragraph">Generative teks ini seperti cerita salah satu penerapan chatbot kita sebelumnya. Chatbot yang menggunakan generative AI dapat menghasilkan respons otomatis yang kontekstual dalam percakapan dengan pengguna. Misalnya, asisten virtual seperti Siri, Alexa, atau Google Assistant menggunakan AI untuk memahami permintaan pengguna dan memberikan jawaban atau tindakan yang sesuai.</p><p class="slate-paragraph">Selain itu, Generative AI digunakan dalam sistem terjemahan bahasa seperti Google Translate yang dapat menerjemahkan teks dari satu bahasa ke bahasa lain. Model ini tidak hanya menerjemahkan kata demi kata, tetapi juga mempertimbangkan konteks untuk memberikan terjemahan yang lebih akurat.</p><p class="slate-paragraph">Generative teks menggunakan model bahasa besar (<em class="slate-italic">Large Language Models</em>, LLM) untuk menghasilkan teks yang koheren dan relevan dalam berbagai konteks. LLM adalah jenis model machine learning yang memiliki parameter sangat besar (miliaran hingga triliunan) dan dilatih pada dataset teks yang sangat besar. Contoh LLM yang populer termasuk GPT-3, GPT-4, Gemini, Gemma, BERT, dan lain sebagainya.</p><p class="slate-paragraph">Salah satu penerapan Generative teks paling populer adalah Gemini dan Chat GPT. keduanya merupakan tools yang sangat <em class="slate-italic">powerfull</em> karena memiliki data yang sangat banyak. Mari kita bahas salah satunya, yaitu Gemini.</p><p class="slate-paragraph"></p><h4 class="slate-h4">Generative AI for Images</h4><p class="slate-paragraph">Generative AI dalam konteks generasi citra adalah proses di mana model AI menciptakan gambar baru yang tidak ada sebelumnya berdasarkan pelatihan dari dataset gambar yang ada. Teknologi ini dapat menghasilkan gambar yang realistis atau artistik dengan berbagai aplikasi mulai dari desain grafis hingga peningkatan gambar medis.</p><p class="slate-paragraph"></p><p class="slate-paragraph">Salah satu contoh penerapan dari Generative Images ini adalah <a href="https://stablediffusionweb.com/app/image-generator" class="slate-a" target="\_blank"><u class="slate-underline">StableDiffusion</u></a>. StableDiffusion adalah model kecerdasan buatan (AI) canggih yang menggunakan teknik difusi untuk menghasilkan gambar realistis berdasarkan teks. Dirilis pada tahun 2022 oleh Stability AI, Stable Diffusion telah merevolusi dunia pembuatan gambar digital. </p><p class="slate-paragraph"></p><p class="slate-paragraph">Fitur utama Stable Diffusion adalah mengubah deskripsi tekstual menjadi gambar. Anda cukup memberikan instruksi tertulis, seperti "foto astronot mengendarai kuda di Mars" dan Stable Diffusion akan menghasilkan gambar yang sesuai.</p><p class="slate-paragraph"></p><p class="slate-paragraph"></p><h4 class="slate-h4">Generative AI for Video</h4><p class="slate-paragraph">Generative video adalah proses pembuatan atau modifikasi video menggunakan model AI dengan algoritma canggih untuk menghasilkan urutan gambar yang koheren dan realistis. Teknologi ini dapat digunakan untuk membuat film pendek, animasi, atau video musik, dengan AI menghasilkan adegan, karakter, dan efek visual yang sebelumnya sulit dibuat secara manual. </p><p class="slate-paragraph">Keuntungan generative video meliputi pengurangan waktu dan biaya produksi, serta kemampuan AI untuk menghasilkan elemen visual unik dan inovatif. AI juga memungkinkan penyesuaian dan umpan balik real-time untuk proses iteratif yang cepat. Tools seperti Veo Google DeepMind dan Sora OpenAI mampu menghasilkan video realistis dari teks deskriptif.</p><p class="slate-paragraph">Veo, diluncurkan oleh Google DeepMind pada Mei 2024, adalah model AI mutakhir yang mengubah deskripsi teks menjadi video dinamis. Dengan arsitektur jaringan saraf tiruan yang kompleks, Veo menganalisis teks untuk memahami makna dan menghasilkan gambar yang sesuai, menggunakan teknik AI canggih untuk menciptakan gambar realistis dan konsisten. Meskipun masih dalam pengembangan, Veo memiliki potensi besar untuk merevolusi pembuatan dan konsumsi video di berbagai industri.</p><p class="slate-paragraph"></p><h4 class="slate-h4">Generative Multimodal Model</h4><p class="slate-paragraph">Model multimodal adalah model yang dirancang untuk memproses dan mengintegrasikan informasi dari berbagai jenis data atau modalitas, seperti teks, gambar, audio, video, dan sensor lainnya. Model ini bertujuan untuk memahami dan menghasilkan output yang konsisten dan bermakna berdasarkan data input yang kompleks dan beragam.</p><p class="slate-paragraph">Jenis modalitas yang bisa diolah oleh multimodal model mencakup teks, gambar, audio, video, dan sensor. Dengan modalitas yang beragam biasanya multimodal menggunakan beberapa pendekatan arsitektur seperti <em class="slate-italic">Convolutional Neural Networks (CNNs), Recurrent Neural Networks (RNNs) </em>atau <em class="slate-italic">Transformers, Cross-Modal Attention Mechanisms, </em>dan lain sebagainya.</p><p class="slate-paragraph">Secara singkat multimodal akan menggabungkan fitur dari berbagai modalitas pada tahap awal sebelum pemrosesan lebih lanjut oleh model. Setelah itu, ia akan memproses setiap modalitas secara independen dan menggabungkan hasilnya di tahap akhir. </p><p class="slate-paragraph">Salah satu contoh penerapan dari multimodal ini adalah <a href="https://llava-vl.github.io/" class="slate-a" target="\_blank"><u class="slate-underline"><em class="slate-italic">Large Language and Vision Assistant</em></u><u class="slate-underline"> </u></a>(LLaVA). LLaVA adalah model kecerdasan buatan (AI) inovatif yang dikembangkan oleh Microsoft Research. Model ini menggabungkan kekuatan <em class="slate-italic">large language model </em>(LLM) dengan pemahaman visual sehingga memungkinkan model untuk mengolah data teks dan citra dalam waktu yang bersamaan.</p><p class="slate-paragraph"></p><h3 class="slate-h3">Image Generation</h3><p class="slate-paragraph">Secara umum ada tiga buah pendekatan yang sering digunakan untuk membangun Generative AI yang dapat menciptakan sebuah gambar yaitu <em class="slate-italic">Variational Autoencoders </em>(VAE), <em class="slate-italic">Generative Adversarial Network </em>(GAN), dan <em class="slate-italic">Dilllffusion Models</em>. </p><p class="slate-paragraph"></p><p class="slate-paragraph">GAN, VAE, dan <em class="slate-italic">Diffusion Models</em> adalah tiga model Generative AI yang ampuh dengan kelebihan dan kekurangan masing-masing. Pilihan model tergantung pada kebutuhan dan permasalahan yang ingin Anda selesaikan. GAN cocok untuk menghasilkan data yang sangat realistis, sementara VAE cocok untuk menghasilkan data yang konsisten dan koheren.  Di lain sisi, Diffusion Models menawarkan keseimbangan antara kualitas dan efisiensi pelatihan.</p><p class="slate-paragraph">Generative AI merupakan bidang yang berkembang pesat dan model-model baru terus bermunculan. Dengan kemajuan teknologi, kita dapat berharap untuk melihat model Generative AI yang semakin canggih dan mampu menghasilkan data yang lebih realistis dan bermanfaat di masa depan. Tentunya dengan perkembangan ini, Anda tidak ingin tertinggal jauh di belakang sebagai pengguna saja, ‘kan? </p><p class="slate-paragraph">Sebagai seorang machine learning engineer andal, alangkah baiknya Anda juga mempelajari dan membuat sendiri model Generative, baik itu melalui <em class="slate-italic">fine tuning,</em> <em class="slate-italic">quantization</em>, atau bahkan menggunakan open model yang tersebar di luar sana dibandingkan menggunakan API atau tools yang sudah <em class="slate-italic">plug and play</em>. Menggunakan API dan tools yang sudah ada bukanlah hal yang buruk, tetapi jika Anda bisa membuat dan menyesuaikan model Generative tentunya menjadi sebuah nilai lebih untuk mempertahankan posisi Anda di perusahaan. Berikut penjelasan dari ketiga pendekatan untuk image generation.</p><ul class="slate-ul"><li class="slate-li"><div style="position:relative"><em class="slate-italic">Variational Autoencoders </em>(VAE) adalah salah satu jenis model generatif yang menggabungkan konsep autoencoder dengan teknik probabilistik untuk menghasilkan data baru yang realistis. VAE dikembangkan oleh Kingma dan Welling pada tahun 2013. Konsep ini dirancang untuk mengatasi beberapa keterbatasan dari autoencoder tradisional, terutama dalam hal kemampuan generatif dan representasi laten.</div></li><li class="slate-li"><div style="position:relative"><em class="slate-italic">Generative Adversarial Networks</em> (GAN) adalah salah satu model paling inovatif dalam bidang machine learning, khususnya dalam generative AI. Diperkenalkan oleh <a href="https://www.linkedin.com/in/ian-goodfellow-b7187213/" class="slate-a" target="\_blank"><u class="slate-underline">Ian Goodfellow</u></a> <em class="slate-italic">et al.,</em> pada tahun 2014, GAN terdiri dari dua jaringan saraf yang berkompetisi satu sama lain, yaitu Generator dan Discriminator. Generator mencoba mengubah noise acak menjadi sebuah gambar baru, sedangkan diskriminator mencoba memprediksi apakah gambar tersebut asli atau bukan. </div></li><li class="slate-li"><div style="position:relative">Diffusion models adalah jenis model generatif yang digunakan untuk menghasilkan gambar menyerupai data asli. Secara singkat model ini memanfaatkan proses difusi dan denoising untuk belajar dan menghasilkan data. </div></li></ul><p class="slate-paragraph"></p><h3 class="slate-h3">Text Generation</h3><p class="slate-paragraph"><em class="slate-italic">Text generation</em> menggunakan <em class="slate-italic">Large Language Models </em>(LLMs) adalah bidang dalam pemrosesan bahasa alami (NLP) yang berfokus pada menghasilkan teks yang koheren dan bermakna berdasarkan input tertentu. LLMs adalah model pembelajaran mesin yang besar dan kompleks, dilatih pada dataset teks yang sangat besar untuk memahami dan menghasilkan bahasa manusia.</p><p class="slate-paragraph">Text generation yang menggunakan Large Language Models (LLMs) adalah bidang yang kompleks tetapi sangat kuat dalam pemrosesan bahasa alami. Dengan berbagai tipe LLM (public, private) dan pendekatan untuk membuat model dari scratch, pengguna memiliki fleksibilitas untuk memilih pendekatan yang paling sesuai dengan kebutuhan mereka, baik dalam hal kontrol, biaya, dan kompleksitas teknis. </p><p class="slate-paragraph">Model seperti GPT-3, BERT, dan lainnya telah digunakan dalam berbagai aplikasi baru pada kasus NLP. Perkembangan ini tentunya akan terus berlanjut untuk membuat model yang lebih cerdas, lengkap dan efisien. Lalu, bagaimana cara kita memiliki pendekatan yang cocok dari berbagai macam tipe LLM? Mari kita cari tahu perbedaannya terlebih dahulu.</p><ol class="slate-ol"><li class="slate-li"><div style="position:relative"><em class="slate-italic">Building from Scratch</em>Membuat LLM dari scratch berarti mengembangkan model bahasa besar dari awal, termasuk pengumpulan data, preprocessing, pelatihan model, dan deployment.Hal yang paling dipertimbangkan untuk membuat model dari nol adalah biaya, karena kita memerlukan <em class="slate-italic">resource</em> yang sangat banyak seperti waktu, sumber daya manusia, dan sumber daya komputasi. Namun, dengan membuat dari nol, kita memiliki kendali penuh terhadap model yang dibangun. Selain dapat menyesuaikan dengan kebutuhan. Anda juga dapat melakukan eksperimen dan inovasi baru dalam arsitektur model.</div></li><li class="slate-li"><div style="position:relative"><em class="slate-italic">Private Model/Commercial Model</em>Private LLMs adalah model bahasa besar yang dikembangkan dan digunakan secara eksklusif oleh organisasi atau individu tertentu. Model ini tidak tersedia untuk umum dan biasanya disesuaikan dengan kebutuhan spesifik organisasi atau proyek. Model bahasa yang digunakan oleh perusahaan besar seperti Google Search AI, Amazon Alexa, IBM Watson, Gemini, dan lain sebagainya.Untuk menggunakan model ini, biasanya kita perlu membayar lisensi untuk mendapatkan API sehingga bisa digunakan pada aplikasi yang sedang dibangun.</div></li><li class="slate-li"><div style="position:relative"><em class="slate-italic">Open Source Model</em>Public LLMs adalah model bahasa besar yang tersedia secara publik untuk digunakan oleh siapa saja. Model ini biasanya dikembangkan oleh organisasi riset, perusahaan teknologi besar, atau komunitas open-source dan dirilis untuk akses umum. Beberapa open source model seperti GEMMA, GPT-3, LLama, BERT, T5, Claude, Cohere, dan lain sebagainya.Untuk menggunakan model publik ini, kita tidak perlu biaya besar karena model sudah dilatih dan siap digunakan. Namun, sebagai pengguna, kita tidak memiliki kontrol penuh atas data pelatihan dan parameternya. Selain itu, dengan menggunakan layanan pihak ketiga, dapat menimbulkan resiko privasi untuk data sensitif karena kita perlu menyetujui syarat dan ketentuan dari masing-masing penerbit.</div></li></ol><p class="slate-paragraph"></p><h3 class="slate-h3">Multimodal Model</h3><p class="slate-paragraph">Multimodal model adalah jenis model pembelajaran mesin yang dapat memproses dan memahami berbagai jenis data atau modalitas, seperti teks, gambar, audio, dan video secara bersamaan. Tujuannya adalah untuk menggabungkan informasi dari berbagai sumber ini untuk mencapai pemahaman yang lebih komprehensif dan menghasilkan keluaran yang lebih kaya dan akurat.</p><p class="slate-paragraph"></p><p class="slate-paragraph">Setelah perkembangan yang sangat cepat dari Generative AI, lalu mengapa multimodal memiliki peran penting dan seringkali menjadi pilihan utama? Hal ini karena multimodal model memiliki kekayaan informasi, fleksibilitas aplikasi, hingga kemampuan pemahaman kontekstual yang lebih baik. </p><p class="slate-paragraph">Salah satu contoh multimodal model adalah LLaVa. LLaVa atau <em class="slate-italic">Large Language and Vision Assistant</em> adalah contoh model multimodal yang menggabungkan kemampuan pemrosesan NLP dan <em class="slate-italic">computer vision </em>(CV) sehingga memiliki kemampuan interaksi yang lebih kaya dan kontekstual. LLaVa bertujuan untuk memproses dan memahami informasi dari berbagai modalitas, seperti teks dan gambar, untuk menghasilkan output yang lebih informatif dan relevan.</p></x-turndown>