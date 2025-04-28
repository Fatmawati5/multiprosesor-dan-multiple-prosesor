# multiprosesor-dan-multiple-prosesor

**1.Arsitektur Multiple Prosesor**

Pada bagian kiri gambar, kita melihat Arsitektur Multiple Prosesor. Dalam arsitektur ini, terdapat beberapa CPU, tepatnya empat CPU yang dinamakan CPU 1, CPU 2, CPU 3, dan CPU 4. Keempat CPU ini saling terhubung melalui sebuah jalur komunikasi bersama, yang disebut bus. Bus ini berfungsi sebagai jalur utama untuk pertukaran data, instruksi, dan sinyal kontrol antar CPU dan komponen lainnya. Karena semua CPU menggunakan bus yang sama, jika banyak CPU aktif bersamaan, akan terjadi kemacetan data atau yang disebut bottleneck.

Semua CPU mengakses memory controller yang sama. Memory controller ini bertugas mengelola semua permintaan dari CPU untuk membaca ataupun menulis ke main memory atau memori utama. Memori utama berfungsi untuk menyimpan data dan program yang sedang berjalan. Setelah itu, dari main memory, jalur komunikasi dilanjutkan ke I/O controller. I/O controller ini berperan sebagai penghubung antara sistem dengan berbagai perangkat eksternal, seperti komputer, printer, atau perangkat input dan output lainnya.

**2.Arsitektur Multiprosesor Symmetric (SMP)**

Kemudian, pada bagian kanan gambar, diperlihatkan Arsitektur Multiprosesor Simetris atau biasa disebut SMP. Dalam arsitektur ini, terdapat lima CPU, yaitu CPU 1 hingga CPU 5. Semua CPU dihubungkan secara simetris atau sejajar, bukan melalui satu jalur bus seperti pada multiple prosesor, tetapi melalui koneksi langsung yang saling terintegrasi. Artinya, setiap CPU memiliki akses yang setara ke semua sumber daya, termasuk memori utama.

Semua CPU dalam SMP terhubung langsung ke memory controller. Tidak ada prioritas atau urutan khusus, sehingga semua CPU bisa mengakses memori secara bebas dan adil. Memory controller ini berfungsi sama, yaitu mengelola hubungan antara CPU dan main memory. Karena semua CPU memiliki hak akses yang sama terhadap memori, sistem ini mampu mengurangi bottleneck dan meningkatkan efisiensi kerja antar prosesor. Arsitektur ini sangat cocok digunakan dalam server besar, pusat data, dan superkomputer modern karena skalabilitasnya yang tinggi.

Secara keseluruhan, perbedaan utama antara kedua arsitektur ini terletak pada bagaimana CPU berkomunikasi dan mengakses memori. Pada multiple prosesor, semua CPU berbagi satu jalur sehingga rawan kemacetan, sedangkan pada multiprosesor simetris, CPU bisa mengakses memori secara langsung dan merata, sehingga performa keseluruhan sistem menjadi lebih baik.

**Kesimpulannya**, kedua arsitektur ini sama-sama bertujuan untuk meningkatkan kinerja sistem dengan menggunakan banyak prosesor. Namun, arsitektur multiple prosesor cenderung sederhana namun berisiko bottleneck karena menggunakan jalur bus yang sama, sedangkan arsitektur multiprosesor simetris lebih kompleks namun memberikan akses memori yang seimbang, meningkatkan efisiensi dan kinerja sistem secara keseluruhan. Pemilihan arsitektur ini sangat bergantung pada kebutuhan performa dan skalabilitas dari sistem yang dibangun.
