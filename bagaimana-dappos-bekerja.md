# 💡 Bagaimana dappOS bekerja

**DappOS V1 terbagi menjadi 2 bagian utama:**

* [Akun dappOS](akun-dappos/)     : Penerapan abstraksi akun (dompet virtual) yang memungkinkan eksekusi alur kerja dengan otomatis, dan metode pemulihan yang fleksibel.
* [Jaringan dappOS](jaringan-dappos/): Suatu jaringan yang terdesentralisasi untuk membantu pengguna menggunakan akun dappOS miliknya.

<figure><img src=".gitbook/assets/WhatsApp Image 2023-02-10 at 21.24.52.jpg" alt=""><figcaption></figcaption></figure>

**Berikut langkah-langkah dari alur bagan diatas:**

1. Pengguna memberikan perintah dengan membuat tanda tangan untuk mengonfirmasi seluruh alur kerja termasuk interaksi pada satu chain atau lebih, menjembatani aset, dan biaya untuk menggunakan jaringan dappOS.
2. DApps mengirimkan permintaan tadi pada jaringan dappOS melalui JSON-RPC.
3. Jaringan dappOS akan mendelegasikan permintaan tadi ke salah satu node permissionless\* (siapapun bisa menjadi bagian dari jaringan\*) dan menjamin apakah transaksi dieksekusi dengan baik atau node akan memberikan kompensasi setiap kerugian pengguna.
4. Karena diiming-imingi dengan hadiah, node yang dipilih akan menjalankan seluruh alur kerja termasuk menjembatani aset dan transaksi on-chain (dari dompet virtual pengguna hingga kontrak dApp).



