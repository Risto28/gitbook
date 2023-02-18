# 🔔 FAQ

## Bagaimana cara menggunakan dappOS?

Untuk klien pengguna, silahkan cek [dApps](produk-dappos/sdk-dapp/kegunaan.md) yang terintegrasi dengan [dApp SDK](produk-dappos/sdk-dapp/) kami. Nantinya kami akan menghadirkan suatu aplikasi mobile ([mini-program platform](mini-program-platform.md)).

Untuk developer, anda dapat menggunakan [dApp SDK](produk-dappos/sdk-dapp/) untuk membuat dApp chain-agonistic anda sendiri. Anda juga dapat mengembangkan versi mini program pada [mini-program platform](mini-program-platform.md) kami untuk mewujudkan pengalaman pengguna yang serupa dengan web2.

## Apa perbedaan kami dengan bridge antar chain?

Pada dasarnya, alih-alih sebuah bridge jaringan dappOS merupakan suatu sistem order yang kompleks. Jika dirujuk pada kegunaan, layanan bridge umumnya adalah bagian dari perintah eksekusi dan disediakan oleh node server, dimana node super tidak terlibat dengan peran node server dalam menyelesaikan pekerjaannya (berdasarkan CEX, bridges, dan solusi lainnya).

Kami hanya mendelegasikan order dan mengecek apakah order dieksekusi dengan tepat. Prinsip ini memberikan kami beberapa [keuntungan](jaringan-dappos/keuntungan.md).

## Apakah dappOS terlibat dalam penyimpanan aset pengguna?

Kami tidak memiliki akses terhadap aset pengguna dan juga pada node server. Jaringan hanya berperan dalam mengatur penyetoran dari node server.

## Apakah dappOS terdesentralisasi

Node super mengadopsi konsensus dari DPOS, dimana memiliki tingkatan yang sama dengan desentralisasi sebagai DPOS chain atau jaringan layer2 (seperti EOS, dan Optimism).

Node server akan disediakan oleh para institusi profesional (seperti CEX / perusahaan pembayaran), tim proyek, dan klien pengguna. Kami secara langsung akan menghadirkan implementasi siap pakai dari node server untuk memfasilitasi provider yang berminat untuk berpartisipasi pada jaringan. Ketika skala transaksi memadai pada jaringan, kelayakan dan APR yang tinggi akan menarik banyak node desentralisasi untuk berpartisipasi.

## Apakah dappOS aman saat proses dev?

Implementasi yang terkait dengan akun pengguna telah melewati audit keamanan ([Secure3](https://docsend.com/view/h4ru2w5kr6z7q9gh)), dan keamanannya sendiri telah sesuai dengan EOA.

Node super dioperasikan oleh tim pada tahap [1](jaringan-dappos/roadmap.md#tahap1-sentralisasi-node-super-dan-node-server-22-q3) and[ 2](jaringan-dappos/roadmap.md#tahap2-sentralisasi-node-super-dan-desentralisasi-node-server-22-q4-23-q1), dijamin oleh pool pendanaan yang besarannya sama dengan jumlah setoran, dan tim dapat mengambil langkah darurat untuk menjaga keamanan. Tahap[ 3 ](jaringan-dappos/roadmap.md#tahap3-desentralisasi-node-super-dan-node-server-23-q2-23-q3)akan mengadopsi keamanan dengan mekanisme standar industri (MPC signatures atau relayer chains). Jika setoran jauh lebih kecil dari daripada pool pendanaan reguler, kapabilitas anti serangan akan jauh lebih tinggi dari standar industri.

Pool pendanaan dari node server dikelola oleh pihak ketiga, dan dappOS tidak memiliki akses terhadap dana tersebut.
