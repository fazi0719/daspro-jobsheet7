PERCOBAAN 1
1. Sebutkan dan tunjukkan masing-masing komponen perulangan FOR pada kode program
Percobaan 1!
jawab: - for (int i = 1; i <= 10; i++) {
         int i = 1 inisialisasi untuk memulai awal perulangan/pengecekan
         i <= 10 kondisi untuk batasan pengecekan,jika SOP yang diminta 11 maka yang terjadi false
         i++ sebagai statement,setiap selesai 1 putaran, i bertambah 1
       - if (nilai > tertinggi) {
         untuk menyimpan nilai tertinggi sementara selama proses perulangan berlangsung
       - if (nilai > terendah) {
         untuk menyimpan nilai terendah sementara selama proses perulangan berlangsung

2. Mengapa variabel tertinggi diinisialisasi 0 dan terendah diinisialisasi 100? Apa yang
terjadi jika variabel tertinggi diinisialisasi 100 dan terendah diinisialisasi 0?
Jawab: Variabel tertinggi diberi nilai awal 0 supaya saat ada nilai yang lebih besar, nilainya bisa langsung diganti.
Sedangkan variabel terendah diberi nilai awal 100 supaya saat ada nilai yang lebih kecil, nilainya juga bisa diganti.
Kalau dibalik (tertinggi = 100 dan terendah = 0), maka perbandingan tidak akan pernah benar. Akibatnya, hasil akhirnya salah karena nilai tertinggi akan tetap 100 dan nilai terendah tetap 0.

3. Jelaskan fungsi dan alur kerja dari potongan kode berikut!
     if (nilai > tertinggi) {
               tertinggi = nilai;
           }
           berfungsi untuk menyimpan nilai tertinggi sementara selama proses perulangan berlangsung
           Alur Kerja: 
            1.Program mengecek apakah nilai lebih besar dari tertinggi.
            2.Jika kondisi ini Benar (true), artinya nilai yang baru adalah rekor tertinggi.
            3.Variabel tertinggi diperbarui (diisi ulang) dengan nilai yang baru (tertinggi = nilai;).
            4.Jika kondisi Salah (false), tertinggi tetap menggunakan nilai sebelumnya.

           if (nilai < terendah) {
               terendah = nilai;
           }
           berfungsi untuk menyimpan nilai terendah sementara selama proses perulangan berlangsung
           Alur Kerja :
            1.Program mengecek apakah nilai lebih kecil dari terendah.
            2.Jika kondisi ini Benar (true), artinya nilai yang baru adalah rekor terendah.
            3.⁠⁠Variabel terendah diperbarui (diisi ulang) dengan nilai yang baru (terendah = nilai;).
            4.Jika kondisi Salah (false), terendah tetap menggunakan nilai sebelumnya.
            
4. Modifikasi kode program sehingga terdapat perhitungan untuk menentukan berapa
mahasiswa yang lulus dan yang tidak lulus berdasarkan batas kelulusan (nilai minimal 60).
Tampilkan jumlah mahasiswa lulus dan tidak lulus setelah menampilkan nilai tertinggi
dan terendah!