# RNN (Recurrent Neural Network)

Adalah jenis arsitektur jaringan saraf yang di rancang untuk memproses data berurutan, yakni ketika hubungan antar elemen dalam urutan memiliki arti atau konteks temporeral.
RNN biasanya di gunakan pada teks,(Sekuens data), audio (gelombang suara), deret waktu(data urutan terkait waktu).keunggulan utama RNN adalah kemampuannya untuk "mengingat" atau mempertahankan informasi tentang sejarah (konteks) dari urutan data yang di proses.

### Tipe-Tipe RNN
- One-to-one: jaringan neural sederhana yang umum digunakan untuk masalah pembelajaran mesin dengan satu input dan satu output.
- One-to-many: memiliki satu input dan banyak output. ini biasanya digunakan untuk menghasilkan deskripsi gambar.
- many-to-one: mengambil urutan multiple inputs dan memprediksi satu output. populer dalam klasifikasi sentimen, yaitu ketika input nya teks dan output nya kategory.
- many-to-many: mengambil urutan multiple inputs dan outputs.pada umum nya adalah terjemahan mesin.


### Jenis-Jenis RNN

1. RNN sederhana (Vanila RNN)
   adalah bentuk dasar dari arsitektu RNN.pada RRN ini, setiap nuoron memiliki sambungan kembali ke dirinya sendiri.
2. Long Short-Term Memory (LSTM)
   adalah varian RNN yang di kembangkan untuk mengatasi massalah vanishing gradient.
3. Gated Recurrent unit
   adalah vers dari LTSM kaena keduanya memiliki kemiripan dalam desain, GRU menggunakan gerbang pembaruan(update get) dan gerbang reset (reset gate) untuk mengatasi masalah **vanishing gardient**.gerbang gerbang ini dapat dilatih untuk menyimpan informasi dari waktu yang lama tanpa menghilang seiring berjalannya waktu atau mengahpus informasi tidak relevan.


### cara kerja RNN
  1. langkah 1: pengolahan input 
      RNN menerima input berurutan, seperti kata-kata dalam sebuah kalimat atau drame pada sebuah video.setiap  elemen iniput di representasikan dengan vector fitur nemerik. misalnya dalam pemprosesan teks,setiap kata dapat di ubah menjadi vector
      berdasarkan representasi tertentu, seperti word embedding.
  2. langkah 2: perhitungan aktivasi
      setiap unit (neuron) dalam RNN menghitung aktivasi berdasarkan input saat ini dan status internal(state) dari unit pada waktu sebelumnya.aktivasi ini mencermikan informasi yang telah dipelajari dari konteks sebelumnya dalam urutan data. perhitungan aktivasi di lakukan menggunakan fungsi aktivasi,seperti tangen hiperbolik (tanh) atau fungsi sigmoid.
  3. langkah 3: Pembaruan satatus internal
      setiap unit RNN memiliki status internal yang menyimpan informasi dari elemen elemen sebelumnya dalam urutan data. status internal tersebut diperbaharui pada setiap langkah waktu dengan mempertimbangkan aktivasi saat ini dan status internal sebelumnya. pembaruan status internal dapat di jelaskan deb=ngan rumus matematis yang melibatkan operasi matematika, seperti penilain matriks antara vektor input dan bobot serta penambahan biasa.
  4. Langkah 4: Output
      RNN menghasilkan output berdsarkan aktivasi saat ini atau status internal terakhir.output ini sapat digunakan sebagai prediksi berikutnya dalam urutan(mmisalnya, kata berikutnya pada kalimat) atau sebagai hasil akhir dari proses pemprosesan data. output RNN dapat digunakn dalam berbagai tugas,seperti klasifikasi,regresi,atau generasi urutan.
      
