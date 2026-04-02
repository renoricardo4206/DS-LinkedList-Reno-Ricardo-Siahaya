Part A
1. Mengapa linked list membutuhkan variabel head?
Karena head adalah satu-satunya pintu masuk ke seluruh linked list. Linked list tidak memiliki indeks seperti array, sehingga tanpa head, kita tidak tahu di mana list dimulai dan tidak bisa mengakses node manapun. Semua traversal selalu dimulai dari head.
2. Mengapa setiap node menyimpan referensi next?
Karena node-node dalam linked list tidak disimpan secara berurutan di memori (tidak seperti array). Referensi next berfungsi sebagai "penunjuk" ke node berikutnya, sehingga kita bisa berpindah dari satu node ke node lain secara berantai.
3. Mengapa penyisipan di awal lebih mudah di linked list daripada array?
Di linked list, kita hanya perlu membuat node baru dan mengarahkan next-nya ke head lama, lalu update head. Tidak ada pergeseran elemen sama sekali. Sedangkan Array bergantung pada jumlah data didalamnya. Misalnya kita ingin menambahkan data ditengah-tengah puluhan data maka akan banyak langkah-langkah yang digunakan dalam menggeser posisi index datanya.

Part B
4. Jika dibalik (head = newNode dulu), maka referensi ke list lama hilang selamanya karena tidak ada yang menyimpannya. Karena harus simpan dulu alamat head lama ke newNode.next agar rantai list tidak putus.
5.  Dengan kondisi yang salah, loop akan berhenti satu node lebih awal — yaitu berhenti saat current adalah node terakhir karena current.next == null. Akibatnya, node terakhir tidak pernah ditampilkan/diproses.

Part C
6. Struktur mana yang lebih baik untuk akses acak (random access)?
    Kalau secara acak maka array yang lebih baik secara time complexity Array O(1) dibandingkan LinkedList O(n)
7. Struktur mana yang lebih baik untuk penyisipan di awal yang sering?
    LinkedList, karena penyisipan awal O(1) sedangkan array O(n) karena semua elemen harus digeser ke kanan.
8.  Mengapa linked list menggunakan lebih banyak memori daripada array?
    Karena linked list menyimpan 2 yaitu data dan pointer node sedangkan array hanya data saja.