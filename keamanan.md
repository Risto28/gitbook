# 🛡 Keamanan

## Akun dappOS

Akun dappOS merupakan solusi desentralisasi non-kustodian. Keamanan tergantung dari pengguna pada **kunci private** dan **chain publik**. Jika anda menggunakan email sebagai metode pemulihan, maka itu akan bergantung pada **server email** tersebut.

**Satu-satunya cara untuk mengakses akun dappOS anda adalah dengan menyediakan tanda tangan yang cocok**. Tiap dompet virtual disandingkan dengan kontrak manajer dompet virtual yang merekam alamat pemilik ketika di deploy. Sebuah tanda tangan dibutuhkan untuk verifikasi semua transaksi dari dompet. Karena itu akan mustahil untuk membuat kontrak dompet berinteraksi dengan kontrak lain tanpa tanda tangan dari pengguna.

**Akun dappOS dapat digunakan tanpa jaringan dappOS**. Siapapun yang memilik tanda tangan yang cocok dapat berinteraksi dengan kontrak dompet virtual, jadi anda dapat mengunakannya secara manual tanpa layanan kami pada situasi krisis.

## Jaringan dappOS

### **Untuk Pengguna**

Satu-satunya kemungkinan pengguna kami kehilangan asetnya adalah saat mengirim aset ke node server yang gagal menyediakan layanan yang tepat. Bagaimanapun, skenario tersebut dapat dihindari dengan **over-kolateralisasi.**  Jaringan dappOS akan menjamin node yang mendapatkan input anda telah **mengunci lebih banyak aset dibanding jumlah aset yang anda inputkan**. SebagaI contoh, jika order anda 100 USDT pada BSC dan menerima 99.5 USDC pada OP, node yang mendapatkan USDT anda harus mengunci setidaknya 100 USD, bergantung pada fluktuasi dari nilai kolateral.

Dengan **over-kolateralisasi**, jaringan dappOS menjamin tiap order pengguna **dieksekusi dengan tepat**, atau node server akan memberikan k**ompensasi terhadap kerugian penggun**a.&#x20;

Disamping itu, kami juga memiliki pihak ketiga sebagai validator untuk melakukan pengecekan jaringan dappOS bekerja dengan semestinya, jadi pengguna dapat dengan cepat mengetahui ketika terjadi masalah. Tidak mungkin bagi peretas untuk menutup semua validator hanya berdasarkan data on-chain.

### Untuk Jaringan Node

Untuk jaringan dappOS, keamanan diproteksi oleh mekanisme **konsensus DPOS**. Node super **tidak memiliki akses pada aset node server**. Pada situasi terburuk, hanya setoran dari node server yang akan hilang.

Resiko yang ditimbulkan jauh lebih kecil dari bridge pada umumnya. Karena jaringan dappOS network hanya butuh untuk mengunci volume yang sama dari transaksi yang berlangsung, alih-alih dari pool dana yang umumnya jauh lebih besar dari volume harian. Mengunci aset sebanyak dua sampai lima juta USD cukup untuk mendukung volume transaksi harian sebanyak satu milyar USD pada banyak kasus.

### Laporan Audit

[Secure3 \[Nov, 2022\]](https://docsend.com/view/h4ru2w5kr6z7q9gh)
