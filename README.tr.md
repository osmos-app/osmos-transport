# osmos-transport

[English](./README.md) · Türkçe

Kendi cihazların arasında, araya hiçbir sunucu girmeden eşler arası senkronizasyon.

> **Henüz başlanmadı.** Bu repo şimdilik planı tutuyor; önce protokol yazılacak, sonra kod.

## Fikir

Aynı kişiye ait iki cihaz birbirini bulur, kim olduklarını kanıtlar ve yalnızca karşı tarafta eksik olanı gönderir. İlk kullanıcı [Mythos](https://github.com/mythoside) olacak: bir romanı masaüstü ile telefon arasında eşit tutmak.

- **Taşıma:** QUIC (TLS 1.3), [`quinn`](https://github.com/quinn-rs/quinn) ile
- **Keşif:** önce yerel ağda mDNS
- **Kimlik:** her cihaz için bir anahtar çifti
- **Veri:** BLAKE3 ile içerik adresli; böylece bir cihaz tam olarak eksik olanı isteyebilir ve gelen veriyi doğrulayabilir

## Lisans

MIT, bkz. [LICENSE](./LICENSE).
