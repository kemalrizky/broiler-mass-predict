// Broiler Mass Prediction
Dibuat untuk memenuhi tugas besar mata kuliah sains data rekayasa. Program ini menggunakan detectron untuk mengklasifikasi broiler dari suatu gambar dan memprediksi rata-rata berat broiler per hari.

1. Sebelum menjalankan program, Anda dapat melakukan 'make a copy' untuk file Google Colab dengan nama 
'broilerWeightPrediction.ipynb'
2. Program utama untuk image segementation dan prediksi rata-rata berat ayam yang digunakan adalah file google colab
dengan nama file 'broilerWeightPrediction.ipynb' dengan tautan berikut:
https://colab.research.google.com/drive/1Evm-hbYMgUZj90z5xlXbPyqxcrG6IvM7?usp=share_link
3. Pastikan Anda telah mengunduh folder COCO ke dan mengunggah folder tersebut ke directory
drive/My Drive/Colab Notebooks/Tubes_SDR/
4. Buka program utama 'broilerWeightPrediction.ipynb, kemudian jangan lupa untuk mengubah tipe runtime
ke GPU Hardware Accelerator. Kemudian lakukan instalasi library pada cell pertama dan cell kedua.
5. Setelah menginstall library pada cell kedua yakni library detectron, restart runtime, kemudian run cell berikutnya.
6. Google Colab program utama terbagi menjadi beberapa segmen yakni:
  a. Bagian Config merupakan bagian yang akan menjalankan semua hal yang diperlukan untuk menjalankan 
  kode-kode selanjutnya. Kode ini terdiri dari, instalasi dependency yang digunakan, set up drive, 
  dan init dari berbagai hal yang digunakan pada program. 
  b. Bagian Train merupakan bagian utama dari seluruh program yang ada ini, 
  bagian train ini bertugas dalam melatih dan membuat model yang dapat menerima 
  suatu gambar dan menyeleksi dimanakah yang merupakan ayam ataupun bukan.
  c. Bagian Image Segmentation Prediction merupakan bagian yang akan menguji model 
  yang dihasilkan oleh bagian train sebelumnya dalam mendeteksi ayam pada data val yang ada. 
  d. Bagian Weight Prediction merupakan abgian yang akan memodelkan hubungan antara rata-rata berat ayam 
  dengan rata-rata luas yang dibentuk ayam atau average total pixel value.
7. Pastikan Anda menjalankan (run) semua cell secara berurut.



