Pengenalan Natural Language Processing
--------------------------------------

Natural language processing (NLP) adalah salah satu cabang ilmu komputer yang mempelajari cara komputer berinteraksi dengan penggunaan bahasa dalam kehidupan sehari-hari. NLP bertujuan mengembangkan teknik-teknik agar komputer dapat memahami **bahasa alami manusia.**

### Peran NLP dalam Kehidupan Sehari-hari

1.  Search Engine (Mesin Pencari)
    
2.  Asisten Virtual
    
3.  Penerjemahan Otomatis
    
4.  Analisis Sentimen Media Sosial
    
5.  Deteksi Spam
    
6.  Pemeriksaan Tanda Baca, Tata Bahasa, dan Parafrase
    
7.  Chatbot dalam Layanan Pelanggan
    

### TensorFlow + NLP, Mengapa?

TensorFlow dan NLP adalah pasangan yang kuat dalam dunia teknologi karena kombinasi kemampuan komputasi numerik TensorFlow dan fokus NLP untuk memahami bahasa manusia. TensorFlow, sebagai framework machine learning dan deep learning yang populer, menawarkan efisiensi dalam komputasi numerik yang sangat dibutuhkan dalam operasi matriks kompleks, seperti yang digunakan dalam model NLP, yaitu neural networks. 

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

Word embedding adalah teknik dalam NLP untuk **merepresentasikan distribusi kata-kata di ruang vektor**. Tujuan utama dari word embedding adalah menangkap hubungan semantik dan sintaktis antarkata dalam teks. 

Ada beberapa teknik word embedding yang populer digunakan dalam NLP.

1.  **Word2Vec**: Word2Vec memodelkan kata-kata sebagai vektor numerik berdasarkan hubungan kata-kata yang muncul bersama dalam teks. Ada dua pendekatan utama dalam Word2Vec.
    
    *   **Skip-gram**: Model Word2Vec skip-gram melatih neural network untuk memprediksi kata target berdasarkan kata-kata sekitarnya (konteks) dalam suatu kalimat.
        
    *   **Continuous Bag of Words (CBOW)**: Pendekatan CBOW adalah kebalikan dari skip-gram. Alih-alih memprediksi kata target berdasarkan context, skip-gram justru berupaya memprediksi kata-kata di sekitar (context) berdasarkan kata tertentu (kata target). 
        
2.  **GloVe (Global Vectors for Word Representation)**: GloVe adalah metode word embedding untuk menghasilkan vektor representasi kata-kata berdasarkan statistik dari matriks frekuensi kemunculan kata dalam teks (_co-occurrence matrix_). 
    
3.  **FastText**: FastText adalah ekstensi dari Word2Vec yang dikembangkan oleh Facebook AI Research (FAIR).
    

#### Term Frequency-Inverse Document Frequency (TF-IDF)

TF-IDF (_term frequency-inverse document frequency_) adalah sebuah metode  pengolahan teks untuk mengevaluasi seberapa penting sebuah kata pada suatu dokumen dalam konteks korpus atau kumpulan dokumen yang lebih besar. 

#### Bag of Words (BoW)

Bag of Words (BoW) adalah sebuah pendekatan sederhana dalam pemrosesan teks yang digunakan untuk mewakili teks sebagai kumpulan kata-kata terurut tanpa memperhatikan tata urutan atau struktur kalimat.

#### N-gram

N-gram adalah sekumpulan n kata berurutan yang diambil dari sebuah teks atau urutan data. N-gram digunakan pada pemrosesan teks dan pengenalan pola untuk memahami hubungan antar kata dalam teks. Nilai n dalam "n-gram" menunjukkan jumlah kata yang diambil pada satu kali pengambilan. Contoh umum n-gram yaitu unigram (1-gram), bigram (2-gram), trigram (3-gram), dan seterusnya.

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