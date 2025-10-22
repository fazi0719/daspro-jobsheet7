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
Jawab: 
import java.util.Scanner;
public class SiakadFor06 {
    public static void main(String[] args) {
        Scanner sc = new Scanner (System.in);

       double nilai, tertinggi = 0, terendah = 100;
       int jumlahMahasiswaLulus = 0,jumlahMahasiswaTidakLulus=0;

       for (int i = 1; i <= 10; i++) {
           System.out.print("Masukkan nilai mahasiswa ke-" + i + ": ");
           nilai = sc. nextDouble();

           if (nilai > tertinggi) {
               tertinggi = nilai;
           }
           if (nilai < terendah) {
               terendah = nilai;
           }
           if (nilai >= 60) {
              jumlahMahasiswaLulus++;
           }
           else  {
               jumlahMahasiswaTidakLulus++;
       }
       
     } 
       System.out.println("Nilai tertinggi: " + tertinggi);
       System.out.println("Nilai terendah: " + terendah);
       System.out.println("Jumlah mahasiswa yang lulus: " + jumlahMahasiswaLulus);
       System.out.println("Jumlah mahasiswa yang tidak lulus: " + jumlahMahasiswaTidakLulus);        
    }

}


PERCOBAAN 2
1. Pada potongan kode berikut, tentukan maksud dan kegunaan dari sintaks berikut:
a. nilai < 0 || nilai > 100 
jawab: nilai < 0 Kondisi pertama: Memeriksa apakah variabel nilai memiliki nilai yang kurang dari nol (negatif).
nilai > 100	Kondisi kedua: Memeriksa apakah variabel nilai memiliki nilai yang lebih dari seratus.
||: digunakan untuk melihat kondisi ini akan benar (true) kalau salah satu dari dua syarat terpenuhi.
Kesimpulannya, nilai < 0 || nilai > 100 digunakan untuk memeriksa apakah nilai berada di luar batas yang diperbolehkan, yaitu antara 0 sampai 100.
b. continue
jawab: perintah untuk melewati atau skip eksekusi iterasi perulangan yang sedang berjalan saat ini dan langsung melompat ke iterasi perulangan berikutnya
2. Mengapa sintaks i++ dituliskan di akhir perulangan WHILE? Apa yang terjadi jika posisinya dituliskan di awal perulangan WHILE?
Jawab: i++ digunakan untuk menambahkan nilai  agar perulangan bisa berjalan ke mahasiswa berikutnya. Jika ditulis di awal maka perhitungannya naik terlebih dahulu sebelum peng-input dilakukan.
3. Apabila jumlah mahasiswa yang dimasukkan adalah 19, berapa kali perulangan WHILE akan berjalan?
Jawab: 18 kali karena diawali dari 0
Modifikasi kode program sehingga apabila terdapat mahasiswa yang mendapat nilai A, program menampilkan pesan tambahan "Bagus, pertahankan nilainya"!