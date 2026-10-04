# Hobby Hub

Türkçe, web-first hobi platformu için ürün keşfi ve etkileşimli prototip. Private geliştirme deposu; canlı ürün değildir.

## Ana sürüm

`outputs/hobby-hub-demo-v4.html` dosyasını tarayıcıda açın. Mevcut geliştirme bu dosyada sürer. v1–v3 HTML dosyaları tarihsel referanstır; paralel ürün değildir.

- `outputs/*.md`: ürün planı, gereksinimler, yetki modeli ve değişiklik kayıtları.
- `work/test-qa.cjs`, `work/test-learning.cjs`: mevcut ana sürüm için otomatik akış kontrolleri.
- `work/*.js`: geçmiş geliştirmede kullanılan yardımcı parçalar; HTML ile otomatik senkronize edilmez. Yeniden build kaynağı olarak kullanmayın.

## Kontrol

Node.js ile proje kökünde:

```sh
node work/test-qa.cjs
node work/test-learning.cjs
```

Bunlar VM/DOM stub testleridir; gerçek tarayıcı, ödeme veya güvenli giriş testleri değildir. Hesaplar, Premium ve bildirimler demodur. Kişisel demo verileri tarayıcıda tutulur. Kaynak depoya tarayıcı verileri aktarılmaz.

## Sürümleme

İlk aktarım mevcut çalışmaların başlangıç kaydıdır; geçmişte yapılmamış commitler geriye dönük uydurulmaz. Bundan sonraki değişiklikler odaklı feature/fix commitleriyle izlenir. İlk GitHub aktarımı v0.1.0 başlangıç kapsamıdır; release etiketi ayrıca doğrulanmalıdır.

Bu depo bu çalışma hattının tek uzak deposudur. Diğer sohbet/klasörlerdeki çalışmaların tam envanteri ve konsolidasyon kontrolü henüz tamamlanmadı. Canlı deployment yoktur.
