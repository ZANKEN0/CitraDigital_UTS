Implementasi Operasi Morfologi Citra Menggunakan OpenCV
Repositori ini berisi kode sumber Python untuk mendemonstrasikan dasar-dasar pengolahan citra digital menggunakan teknik morfologi. Program ini mengubah citra input menjadi format grayscale dan biner, kemudian menerapkan operasi Erosi, Dilasi, Opening, dan Closing.
Deskripsi Program
Program ini melakukan langkah-langkah pemrosesan citra sebagai berikut:
Preprocessing: Membaca file gambar (img/pokemon1.jpg), mengubahnya menjadi skala abu-abu (grayscale), dan melakukan ambang batas (thresholding) untuk menghasilkan citra biner hitam-putih.
Erosi (Erosion): Mengikis elemen citra. Digunakan untuk memperkecil objek dan menghilangkan noise kecil.
Dilasi (Dilation): Memperbesar elemen citra. Digunakan untuk mempertebal objek dan mengisi celah kecil.
Opening: Kombinasi operasi Erosi diikuti Dilasi. Efektif untuk menghilangkan noise di latar belakang.
Closing: Kombinasi operasi Dilasi diikuti Erosi. Efektif untuk menutup lubang kecil di dalam objek.
Setiap hasil operasi akan ditampilkan dalam jendela GUI secara berurutan.
Prasyarat
Pastikan lingkungan pengembangan Anda memiliki instalasi berikut:
Python 3.x
Library OpenCV (cv2)
Library NumPy
Instalasi
Anda dapat menginstal dependensi yang diperlukan menggunakan pip melalui terminal atau command prompt:
pip install opencv-python numpy

Struktur Direktori
Agar program berjalan dengan benar, pastikan struktur folder Anda disusun seperti berikut:
/direktori-proyek
|-- main.py (File kode python utama)
|-- README.md (Dokumentasi ini)
|-- img/ (Folder untuk menyimpan gambar input)
|-- pokemon1.jpg

Catatan: Jika nama file gambar Anda berbeda, sesuaikan variabel path_file di dalam kode main.py.
Cara Penggunaan
Simpan gambar yang akan diproses di dalam folder img dengan nama pokemon1.jpg.
Jalankan script Python:
python main.py

Program akan menampilkan jendela gambar asli dan biner.
Tekan tombol apa saja pada keyboard (misalnya SPASI atau ENTER) untuk menutup jendela saat ini dan melanjutkan ke proses morfologi berikutnya (Erosi, lalu Dilasi, dst).
Ulangi langkah menekan tombol hingga seluruh proses selesai dan program berhenti.
Catatan Tambahan
Kode ini menggunakan kernel default (None) dari OpenCV yang setara dengan matriks persegi ukuran 3x3.
Terdapat bagian kode yang dinonaktifkan (komentar) di bagian bawah file. Bagian tersebut berisi logika untuk melakukan iterasi eksperimental dengan berbagai ukuran kernel dan jumlah iterasi dilasi. Anda dapat mengaktifkannya jika ingin melihat perbandingan hasil yang lebih kompleks.
