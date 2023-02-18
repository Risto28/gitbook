# 📡 Jaringan dappOS

Jaringan DappOS dirancang untuk memberikan pengalaman pengguna yang lancar dalam menggunakan akun dappOS di chain yang berbeda. Untuk memenuhi persyaratan menjalankan dApps saat ini dan memberikan pengalaman pengguna sebaik mungkin, jaringan harus menyediakan dua layanan dasar ini:

* _Bridge aset, Biaya seharusnya sedikit lebih tinggi dari gas fee dan waktunya hanya boleh sedikit lebih lama dari satu transaksi pada chain asal ditambah satu transaksi pada chain yang dituju dalam banyak kasus._
* _Eksekusi transaksi pada on-chain dari dompet virtual. Pengguna wajib diizinkan membayar biaya gas dengan token pada chain yang berbeda, aset di CEX, dan bahkan dengan fiat sekalipun._

Di jaringan dappOS, satu interaksi dApp diperlakukan sebagai permintaan yang mungkin berisi satu atau lebih layanan. Di bawah ini adalah dua contoh yang menunjukkan satu atau beberapa layanan dalam satu permintaan:

* _Eksekusi transaksi dari dompet virtual pada Optimism, dan pembayaran gas dapat dilakukan dengan USDT pada chain BNB._
* _Bridge 100 USDT dari chain BNB ke dompet virtual di Optimism, dan memicu transaksi pada saat yang sama, membayar biaya oleh BTC di chain BNB._

Jaringan akan mendelegasikan permintaan ke salah satu node [permissionless](https://mmsi.binus.ac.id/2021/10/14/blockchain-use-cases-di-bidang-ekonomi-dan-bisnis-blockchain-seri-3/) dan menjamin apakah permintaan tersebut dijalankan dengan baik atau node akan mengkompensasi kerugian pengguna.

Terdapat dua jenis node pada jaringan dappOS:[ Super Nodes ](super-nodes.md)dan [Server Nodes](server-nodes.md). Super node mendelegasikan permintaan dan memberi sanksi pada node yang keliru. Sedangkan server node mengambil permintaan dari super node dan menghasilkan keuntungan dari hasil mengeksekusi mereka.

<figure><img src="../.gitbook/assets/WhatsApp Image 2023-02-11 at 10.05.46.jpg" alt=""><figcaption></figcaption></figure>

**Alur kerja dari sebuah permintaan yang didemonstrasikan melalui flowchart**

<figure><img src="../.gitbook/assets/WhatsApp Image 2023-02-11 at 10.28.33.jpg" alt=""><figcaption></figcaption></figure>

Kami akan membangun jaringan ini langkah demi langkah (lihat [Roadmap](roadmap.md)). Baik super node maupun server node akan sepenuhnya terdesentralisasi.
