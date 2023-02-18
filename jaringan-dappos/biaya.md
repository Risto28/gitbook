# 💰 Biaya



Jaringan dappOS akan membebankan sejumlah biaya untuk setiap permintaan. Biaya merupakan pendapatan utama dari jaringan dappOS yang nantinya akan dibagi antara super node dan server node.

## Kalkulasi biaya

1. **Permintaan yang diinputkan oleh pengguna harus menyertakan berberapa keterangan**

| Item          | Penjelasan                                              | Contoh           |
| ------------- | ------------------------------------------------------- | ---------------- |
| Method        | Pilihan pembayaran (VW, EOA, ACH)                       | VW               |
| GasPriceLimit | Jumlah besaran biaya gas                                | 5 USDT di BSC    |
| PriorityFee   | Biaya yang dibayarkan untuk node                        | 1 USDT di BSC    |
| BridgeFee     | Biaya untuk bridge                                      |  1 USDT di BSC   |
| Token         | Alat tukar dan chain dari biaya gas dan biaya prioritas | USDT di BSC      |
| Input         | Jumlah dan alat tukar yang dibutuhkan untuk bridge      | 1000 USDT di BSC |
| Output        | Jumlah yang seharusnya diterima                         | 1000 USDT di BSC |

Pengguna akan membayar:

&#x20;       _PriorityFee + BridgeFee + GasUsage \* GasPrice + Input_

Biaya gas akan dihitung sesuai dengan harga oracle dalam transaksi pembayaran, dan maksimum tidak akan melebihi GasPriceLimit yang ditentukan pengguna. Jumlah Gas termasuk biaya transaksi abstraksi akun dan biaya transfer yang dihasilkan dalam bridging.

Pengguna akan menerima:

&#x20;     _Output + GasRefundFee_

GasRefundFee adalah pengembalian kelebihan pembayaran saat membayar melalui EOA atau ACH.



2. **Server node akan memberikan kuotasi atau penawarannya sendiri ke super node, yang berisi informasi berikut**

| Item            | Penjelasan                                                      | Contoh                          |
| --------------- | --------------------------------------------------------------- | ------------------------------- |
| SupportedToken  | Token yang didukung saat bridge                                 | USDT on BSC                     |
| Method          | Metode pembayaran (VW, EOA, ACH)                                | VW                              |
| Chains          | Chain publik yang didukung                                      | BSC / OP                        |
| FeeToken        | Alat tukar yang didukung sebagai biaya                          | BSC:ETH/USDT         OP  : USDC |
| BridgeFee       | Biaya minimal yang dikenakan dalam USD                          | 2 USD                           |
| FeeForSuperNode | Biaya yang dibayarkan pada Super node                           |                                 |
| PriorityFee     | Biaya minimal yang dikenakan (USD) dan alat tukar yang didukung | 5 USD                           |

Biaya final yang diterima oleh server node:

&#x20;     _PriorityFee + BridgeFee + GasUsage \* GasPrice + Input_

Pengguna bebas memilih semua tipe pembayaran ketika server node menentukan apa saja yang dapat mereka terima.

3. **Super node akan secara holistik mengurutkan semua node server berdasarkan biaya, kecepatan, dan staking untuk memilih mana yang sesuai.**
