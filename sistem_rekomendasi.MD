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