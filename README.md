# CitraDigital
Ini adalah repositori untuk pembelajaran OPERASI Dasar MORFOLOGI PADA CITRA BINER

Deskripsi
Operasi morfologi adalah teknik pemrosesan citra yang menganalisis dan memodifikasi struktur bentuk objek dalam citra. Operasi ini sangat berguna untuk tugas-tugas seperti penghilangan noise, segmentasi objek, ekstraksi fitur, deteksi tepi, terutama pada citra biner.

Notebook `UTS-citraDigital.ipynb` melakukan langkah-langkah berikut:
1. Memuat beberapa gambar contoh.
2. Mengonversinya ke skala abu-abu (grayscale).
3. Mengonversinya ke citra biner menggunakan thresholding.
4. Menampilkan citra biner asli.
5. Membuat Structuring Element (Kernel) dasar (`np.ones`) dan berbagai bentuk (`MORPH_RECT`, `MORPH_ELLIPSE`, `MORPH_CROSS`) menggunakan `cv2.getStructuringElement`.
6. Menerapkan operasi morfologi dasar:
    * Erosi (`cv2.erode`)
    * Dilasi (`cv2.dilate`)
    * Opening (`cv2.morphologyEx` dengan `cv2.MORPH_OPEN`)
    * Closing (`cv2.morphologyEx` dengan `cv2.MORPH_CLOSE`)
7. Menerapkan operasi morfologi turunan:
    * Morphological Gradient (`cv2.morphologyEx` dengan `cv2.MORPH_GRADIENT`)
    * Top Hat (`cv2.morphologyEx` dengan `cv2.MORPH_TOPHAT`)
    * Black Hat (`cv2.morphologyEx` dengan `cv2.MORPH_BLACKHAT`)
8. Menampilkan hasil dari setiap operasi menggunakan Matplotlib untuk perbandingan visual.

Persyaratan

* Python 3.x
* OpenCV (`opencv-python`)
* NumPy (`numpy`)
* Matplotlib (`matplotlib`)
* Jupyter Notebook / Jupyter Lab (untuk menjalankan file `.ipynb`)

Instal dependensi menggunakan pip:
``bash
pip install opencv-python numpy matplotlib jupyterlab
