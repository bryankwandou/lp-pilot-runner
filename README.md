# lp-pilot-runner

Runner untuk LP Pilot (Meteora DLMM). Hanya berisi workflow; kode bot ada di repo privat.

- `paper-loop.yml` — paper trading 24/7, tick tiap 1 menit. Tidak ada wallet atau kunci trading: hanya membaca
  harga & fee pool Meteora, state disimpan di database.
- `devnet-mass.yml` — uji buka/tutup posisi nyata di **devnet** dari banyak server paralel. Memakai satu wallet
  khusus devnet (Beow32F7XvqgF5xs7R68bhsRwQMMdX6t9LSARuMePDjx, secret terenkripsi `DEVNET_MASS_KEYPAIR`), tidak ada
  kunci mainnet. Hasil tiap run ada di folder `devnet/`.
