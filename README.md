<img width="734" height="759" alt="image" src="https://github.com/user-attachments/assets/5323abff-108f-448c-b2e1-64b3e4465992" />

Penjelasan:
1. Membangun Kerangka (Bagian HTML)
Di tahap awal, kode ini berfungsi untuk menyiapkan benda-benda nyata yang akan dilihat oleh pengguna di layar:

Pemasangan Objek Lampu: Setiap lampu dipasang menggunakan elemen <img>. Setiap lampu diberi identitas unik yang disebut id (seperti lA, lB, lC, lD). Tanpa id ini, instruksi selanjutnya tidak akan tahu lampu mana yang harus dinyalakan.

Penyediaan Saklar (Tombol): Elemen <button> berfungsi sebagai pemicu. Di dalam setiap tombol, terdapat perintah onclick, yang artinya "ketika diklik, jalankan instruksi ini". Ini adalah jembatan yang menghubungkan tombol di layar dengan logika di dalam sistem.

2. Tata Letak (Bagian CSS)
Pengelompokan (Container): Lampu-lampu dibungkus dalam sebuah kelas bernama .rangkaian. Ini bertujuan agar Rangkaian 1 dan Rangkaian 2 memiliki jarak yang jelas dan tidak menyatu.

Garis Pembatas: Penggunaan border-bottom memberikan tanda visual kepada pengguna bahwa kedua rangkaian tersebut adalah dua sistem listrik yang berbeda dan memiliki kontrol masing-masing.

3. Logika Instruksi (Bagian JavaScript)
Pengecekan Status (Logika If-Else): Setiap kali sebuah lampu akan diubah, sistem melakukan pengecekan melalui perintah includes('off.gif'). Caranya adalah dengan melihat nama file gambar yang sedang terpasang. Jika sistem melihat gambar "mati", maka ia akan menggantinya ke "nyala". Begitu pula sebaliknya. Ini adalah dasar dari cara kerja saklar digital.

Sistem Antrean (Variable Counter): Untuk fungsi "Satu per Satu", sistem menggunakan angka urutan (0, 1, 2...). Setiap kali tombol diklik, sistem hanya mengubah lampu yang sesuai dengan angka tersebut, lalu secara otomatis menambah angkanya untuk klik berikutnya. Teknik ini memastikan lampu menyala bergantian, bukan semuanya sekaligus.

4. Simulasi Rangkaian Listrik
Kontrol Individu (Satu per Satu): Mensimulasikan saklar tunggal yang hanya terhubung ke satu lampu dalam satu waktu.

Kontrol Serentak (Semua Lampu): Mensimulasikan saklar utama (Master Switch) yang terhubung ke jalur utama listrik. Begitu saklar ditekan, aliran listrik dikirimkan ke semua lampu dalam daftar secara bersamaan melalui perintah "perulangan" (looping).

Kontrol Kelompok (Grup AB & CD): Mensimulasikan pembagian jalur atau sub-panel. Sistem mengelompokkan id lampu ke dalam daftar tertentu, sehingga satu perintah klik bisa menyasar lampu A dan B secara spesifik tanpa harus menulis perintahnya berkali-kali.
