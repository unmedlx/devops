# Parameter Acuan

Direktorat Teknologi Informasi ULBI, dalam pengembangannya berpedoman pada Green Coding

![image](https://github.com/ditif/devops/assets/11188109/83a9cb3a-a932-4244-9de2-feb13a76fcad)

Green Coding : Low Level Carbon Footprint Code

Dimana setiap program yang dihasilkan mengurangi dampak emisi karbon pada lingkungan. Sehingga sasaran parameter pendukungnya antara lain :

## GTMetrix

Website selalu di evaluasi dan memiliki nilai GTMetrix : A

![image](https://user-images.githubusercontent.com/11188109/222995180-6544137c-0068-4861-a1c4-0704b2ea11e4.png)

## Green Coding Bahasa Pemrograman

Sebagai perbandingan konsumsi komputasi CPU dan Memori dari beberapa bahasa pemrograman yang berjalan di server on premise kami :

![image](https://github.com/ditif/devops/assets/11188109/25a0cbc9-8d0b-46b4-88c1-b46b9d486602)

![image](https://github.com/ditif/devops/assets/11188109/7ad9d39b-6c1f-4bc5-8c9f-a21066e79659)

![image](https://github.com/ditif/devops/assets/11188109/58582ef3-8eba-4849-be21-fd7b5d702eb0)

Rata-rata penggunaan Memori :
1. PHP : 238 MiB
2. Python : 62 MiB
3. Golang : 28,6 MiB

## Green Coding Pengembangan Aplikasi

Untuk mendukung low level carbong coding, pengembangan yang dilakukan pada DTI antara lain pengembangan Frontend, Backend dan Profile Web. Dengan kriteria sebagai berikut :

### Frontend

Pengembangan sisi tampilan tampak depan (Frontend) dengan kriteria :
* Dibangun menggunakan builder CSS (Contoh : shuffle.dev untuk Tailwind Builder)
* Interaksi dengan backend menggunakan Pure VanillaJS dengan fungsi-fungsi yang dipakai ulang dipanggil menggunakan Javascript import dari CDN. Kumpulan fungsi JS Kami ada di [JSCroot](https://jscroot.github.io/).
* Login Otorisasi dan Authentikasi Pengguna menggunakan [WhatsAuth](https://github.com/whatsauth/) yang sudah menggunakan Paseto untuk Security Token ke Backend.
* Dibangun diatas platform GitHub Pages.

### Backend

Pengambangan sisi Backend dengan kriteria :
* Dibangun dengan menggunakan bahasa pemrograman Go dengan framework Golang Fiber. Boiler Plate Kami ada di [GoCroot](https://github.com/gocroot/gocroot).
* Fungsi-fungsi yang dipakai berulang kali maka wajib dibuatkan package (Reuse Code). Package kami ada di [aiteung](https://github.com/aiteung).
* Token Barier akses API yang digunakan adalah Paseto, tidak lagi menggunakan JWT karena lebih aman.
* Backend berada di Docker On-premises atau layanan Cloud yang memiliki nilai latensi paling kecil yang diakses dari Indonesia.
* Unit Testing menggunakan go test.

### Landing page dan Web Profil

Web berita, profile, landing page dipilih provider [Google](https://cloud.google.com/architecture/reduce-carbon-footprint). Blogger.com dengan custom css, js dan konten gambar didistribusikan dalam CDN Blogger.com dengan tetap menjaga nilai GTMetrix A.
