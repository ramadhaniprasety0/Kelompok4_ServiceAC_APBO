# MAJU JAYA SERVICE 
---

## Nama Anggota Kelompok 
- Ramadhani Prasetyo - 4522210009
- Daffa Abraar Sajuti - 4522210040
- Farah Tri Mahardini - 4522210042
- Salwa Khairu Mista - 4522210066
- Nadia Ayu Rahmawati - 4522210077
  
---
### Latar Belakang
Maju Jaya Service (MJS) adalah perusahaan layanan AC dan kulkas yang menyediakan berbagai layanan, termasuk perawatan rutin, penjualan, pemasangan, perbaikan, dan pemindahan. Mereka memiliki jadwal rutin untuk layanan harian dan melayani baik di Depok maupun di luar kota dalam skala kecil. Semua harga layanan dijelaskan secara rinci untuk transparansi konsumen, dan perusahaan memiliki logo yang dikenal oleh pelanggan. Meskipun mereka menyesuaikan pembayaran dengan keadaan, layanan kredit tidak tersedia saat ini. Tim yang terlatih siap untuk menangani pengerjaan, tetapi keberadaan tim kurang efektif jika pengerjaan dilakukan secara pribadi.Dengan masalah yang ada untuk memberikan kemudahan kepada konsumen dalam memperoleh informasi tentang layanan yang ditawarkan, termasuk jadwal rutin, harga-harga terkait, dan prosedur pemesanan. Upaya akan dilakukan untuk meningkatkan fitur dan keterjangkauan penggunaan bagi segmen tersebut. Melalui website, juga diharapkan dapat memfasilitasi pembayaran yang sesuai dengan kebutuhan pelanggan, termasuk kemungkinan pembayaran setelah pengerjaan untuk barang kecil dan penyesuaian pembayaran dari pihak ketiga. Dengan demikian, pembuatan website ini akan menjadi sarana penting dalam memperluas jangkauan dan meningkatkan efektivitas layanan MJS Maju Jaya Service.

---
### Kendala Maju Jaya Service 
1. Pemilik layanan sulit untuk memberikan informasi yang cukup kepada pelanggan secara efektif.
2. Skala layanan di luar kota yang sangat kecil, menjadi hambatan dalam pengembangan bisnis karena potensi pasar di luar kota kurang maksimal.
3. Kebanyakan pengguna pribadi pada website terdahulu
4. Jadwal layanan dan pemesanan yang bentrok membuat pemilik menjadi kurang efisien dalam manajemen jadwal.
5. Industri layanan sangat kompetitif, dengan banyak penyedia layanan yang bersaing untuk mendapatkan perhatian pelanggan.
6. Kurangnya perkembangan fitur website terdahulu

---
### Solusi  
**1. Fitur Customer**	
- login ke akun customer
- Reservasi Layanan
- Melihat Status Layanan
- Membuat Pesanan
- Melihat Laporan Perbaikan
  
**2. Fitur Admin**
- login ke akun Admin
- Menambah Layanan Jasa
- Menghapus Layanan Jasa
- Mengupdate Layanan Jasa
- Melihat Status Layanan
- Melihat Laporan perbaikan
  
**3.Fitur Teknisi**
- Login ke akun Teknisi
- Melihat Pesanan
- Menambah status Layanan
- Menghapus status Layanan
- Mengupdate status Layanan
- Melihat Status Layanan
- Membuat Laporan Perbaikan

---
### Actor
**Actor yang menggunakan**
1. Customer
2. Admin
3. Teknisi

---
### Use Case
![Use Case](./UseCaseServiceMJS.jpg)

---
### ERD (Entity Relationship Diagram)
![ERD](/ERD%20JASA%20SERVICE%20AC.png)
Terdapat 6 entutas pada ERD Jasa Service MJS seperti:
- Customer
- Admin
- Teknisi
- Order
- Service
- StatusService

Tiap entitas memiliki atribut
- Customer --> (IDcustomer, Nmcustomer, NoTelp, Alamat, Password)
- Admin --> (IDadmin, Nmadmin, NoTelp_admin, Password, IDcustomer)
- Teknisis --> (IDteknisi, Nmteknisi, NoTelpteknisi, Password, IDcustomer)
- Order --> (IDorder, Tglorder, IDcustomer, IDstatus, IDteknisi, IDservice)
- Service --> (IDservice, Nmservice, Harga)
- StatusService --> (IDstatus, keterangan)

Adapun relationship antar entitas seperti:
1. dilayani --> pada entitas customer dan admin
2. ditangani --> pada entitas customer dan teknisi
3. Memesan --> pada entitas customer dan order
4. Mencakup --> pada entitas order dan Admin
5. Mencakup --> pada entitas order dan teknisi
6. Mencakup --> pada entitas order dan service
7. Berstatus --> pada entitas order dan StatusService

Terdapat kardinalitas juga seperti many to one

---
### Class Diagram
![Class Diagram](./DiagramClassServiceMJS.jpg)
Hampir sama seperti ERD, yang membedakan adalah adanya classpada class diagram serta tidak terdapat relationship, kardinalitas.

Contoh class dalam entitas Customer
-Login()
-VerifikasiLogin()
-BuatPesanan()
-RsrvsiSrvice()
-LihatStatusSrvice()
-LihatLprnPrbaikan()

Contoh class dalam entitas Admin
-Login()
-VerifikasiLogin()
-TmbhLynanSrvice()
-HpsLynanSrvice()
-UpdateLynanSrvice()
-LihatStatusSrvice()
-LihatLprnPrbaikan()

Contoh class dalam entitas Teknisi
-Login()
-VerifikasiLogin()
-LihatPesanan()
-TmbhStatusSrvice()
-UpdateStatusSrvice()
-HpsStatusSrvice()
-BuatLprnPrbaikan()

---
### Flowchart
![Flowchart](./Flowchart%20MJS.png)

---
### DataMentah
![Flowchart](./DataMentahServiceMJS.jpg)

---

### Wireframe Pelanggan Service
**Tampilan Login Pelanggan**
![Flowchart](./WireframePelanggan/WireframePelangganPage1.png)
**Tampilan Daftar Pelanggan**
![Flowchart](./WireframePelanggan/WireframePelangganPage2.png)
**Tampilan Home Page Pelanggan**
![Flowchart](./WireframePelanggan/WireframePelangganPage3.png)
**Tampilan Pemesanan Pelanggan**
![Flowchart](./WireframePelanggan/WireframePelangganPage4.png)
**Tampilan Riwayat Pemesanan Pelanggan**
![Flowchart](./WireframePelanggan/WireframePelangganPage5.png)

### Wireframe Admin
**Tampilan Dashboard Admin**
![Flowchart](./WireframeAdmin/WireframeAdminPage1.png)
**Tampilan Pesanan Admin**
![Flowchart](./WireframeAdmin/WireframeAdminPage2.png)
**Tampilan Pengaturan**
![Flowchart](./WireframeAdmin/WireframeAdminPage3.png)
**Tampilan Edit Layanan**
![Flowchart](./WireframeAdmin/WireframeAdminPage4.png)
**Tampilan Tambah Staff**
![Flowchart](./WireframeAdmin/WireframeAdminPage5.png)

### Wireframe Teknisi
**Tampilan Dashboard Teknisi**
![Flowchart](./WireframeTeknisi/WireframeTeknisiPage1.png)
**Tampilan Tugas Teknisi**
![Flowchart](./WireframeTeknisi/WireframeTeknisiPage2.png)
**Tampilan Pembayaran**
![Flowchart](./WireframeTeknisi/WireframeTeknisiPage3.png)

---
### Penjelasan UX
User Experience (UX) dari MJS App yang kami membuat agar pengguna dapat berinteraksi dengan mudah dan bisa digunakan di semua kalangan usia, agar pengguna merasakan pengalaman yang lebih saat menggunakan App kami.

Design kami intuitif, mudah dipahami, efisien, dan memuaskan pengguna, Kelebihan dari Design kami antara lain:
- Desain kami fokus pada kebutuhan pengguna.
- Pengguna tidak bingung atau frustrasi saat menggunakan layanan kami.
- Desain yang estetis dapat membuat layanan kami lebih menyenangkan untuk digunakan.

---
### Link Youtube
[Klik Untuk Melihat Vidio Presentasi Kelompok kami](https://youtu.be/2l02bllTSH0?si=e_DfEx330IrAECAd)
