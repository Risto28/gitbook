# Setel via e-mail (DKIM-based)

## Rangkuman

DappOS mendukung pengguna untuk mengatur email guardian (penjaga) untuk memverifikasi permintaan reset melalui Domain Keys Identified Mail (DKIM). Pengguna cukup mengirim email dari akun email guardian yang telah ditentukan sebelumnya untuk mengatur ulang kunci utama.

## Menautkan e-mail dengan akun

DappOS akan melakukan hash informasi email guardian pengguna dan kata sandi yang ditetapkan oleh pengguna. Hash itu nantinya akan disimpan pada chain publik.

## Mengirim e-mail reset

Setelah pengguna mengajukan permohonan reset email pada laman muka DappOS, laman muka DappOS akan membuat template email pemulihan untuk pengguna, yang dapat dikirim cukup dengan satu klik saja. Isi email mencakup maksud dan informasi terkait akun terenkripsi

## Reset akun

Setelah super node atau pengguna menerima email reset ulang, mereka akan membuat ZK-proof merujuk pada DKIM, dan menyetel ulang izin akun setelah verifikasi pada on-chain berhasil.\


## Flowchart

<figure><img src="../../.gitbook/assets/WhatsApp Image 2023-02-11 at 06.46.56.jpg" alt=""><figcaption></figcaption></figure>

