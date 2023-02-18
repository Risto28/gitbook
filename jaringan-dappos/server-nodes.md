# ⚒ Server Nodes

Server node mengeksekusi permintaan dan menghasilkan dari setiap permintaan yang berhasil. Server node perlu memberi tahu layanan apa yang dapat mereka berikan dan besaran biaya untuk layanan mereka. Misalnya:

* Transaksi on-chain pada OP/BNB, biaya $1 untuk setiap satu kali layanan.
* Bridge aset USDT/USD/BNB/ETH dari OP ke BNB, biaya layanan 1 USD per transaksi.

Untuk menjamin keamanan jaringan dappOS, node server yang memenuhi syarat perlu menyetor beberapa aset ([aturan deposit](deposit.md)). Jumlahnya fleksibel, tetapi node server tidak akan dapat menerima pesanan yang tidak dapat ditanggung oleh deposit. Misalnya, jika node server hanya menyetor 10 USDT, ia tidak akan menerima pesanan yang menjembatani aset lebih dari 10 USDT.&#x20;

Node server dapat menolak pesanan yang dikirim.
