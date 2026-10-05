# Hobby Hub demo v4 — Bana uygun mu?

4 Ekim 2026. Güncel demo: hobby-hub-demo-v4.html. Kaynak temel: v3. v3 ve önceki dosyalar geçmiş sürümlerdir; yeni geliştirme v4 üzerinde sürdürülür. GitHub konsolidasyonu bu değişiklikte yapılmadı.

## Deneme

HTML dosyasını tarayıcıda aç. Bitkiler → Bana uygun mu? bölümüne gir. Baktığın bitkileri ve konumunu belirt; değerlendirmeyi çalıştır. Sonuçlar formun sağında, küçük ekranda altında görünür.

Örnek: aydınlık dolaylı ışık, orta nem, ılık/istikrarlı sıcaklık, düzenli bakım ve güvenlik kontrolünü değerlendirmeye dahil etmeme seçimiyle Monstera deliciosa için uygun sonucu çıkar. Işığı yok olarak değiştirip yeniden değerlendir; sonuç değişir. Nem yüksek değilse Anthurium için koşul değişikliği görünür. Eksik alanlarda kesin olumlu sonuç çıkmaz.

Monstera veya Anthurium clarinervium ilanını aç → Bana uygun mu? Hedef tür korunur. Türü kesin bilinmeyen ilanlarda bilgi eksik sonucu gösterilir. Saksılarda değerlendirme sunulmaz. Üretici vitrininin sonunda da bakım profiline giriş vardır.

Doğrudan örnek rota: #h=plants&t=fit&plant=deliciosa. URL oda adı veya kişisel cevap içermez. Genel alana dönmek hedef türü temizler. Mevcut breadcrumb ve üretici rota sistemi korunur.

## Veri ve sınırlar

Beş tür için açıklanabilir, basitleştirilmiş kurallar vardır. Temel bakım bilgileri arayüzde bağlantısı verilen RHS kaynaklarına dayanır. Bu bir uzman doğrulaması veya bitkinin sağlığına ilişkin garanti değildir. Çocuk/evcil hayvan güvenliği doğrulanmadığı için bu kontrol istendiğinde olumlu uygunluk verilmez.

Deneyim beyanı sonuç açıklamasına katılır; uygunsuz ortamı geçersiz kılmaz. Sayısal başarı puanı, sponsor etkisi veya satın alma zorunluluğu yoktur. Tek konum düzenlenebilir. Çoklu oda kaydı ve zaman içinde bakım günlüğü henüz yoktur.

Kişisel cevaplar varsayılan olarak yalnız oturum belleğindedir. Açık seçimle ayrı yerel anahtarda saklanır, silinebilir. HTML dışa aktarımı kişisel profili içermez; uygulama alanı ve modal içeriği ihracatta temizlenir. v4 genel demo kayıtları v3'ten ilk kullanımda okunabilir; v4 ayrı anahtara yazar, v3 kayıtlarını değiştirmez.

## Doğrulama

36/36 Node VM model, render, olay işleyici ve URL/geçmiş simülasyonu geçti. Bunların 23'ü önceki üretici vitrini regresyonları; 13'ü uygunluk özelliğine ait. Sonuç: work/fit-test-results.json. Gerçek tarayıcı tıklaması, ekran görüntüsü ve mobil görsel doğrulama yapılmadı. Yayın/production entegrasyonu yoktur.

## Başlangıç ve deneyim ayrımı

İlk bitkimle başlayacağım / Zaten bitki bakıyorum seçimleri eklendi. Yeni başlayana yalnız ortamına uygun türler listelenir. Deneyimli kullanıcı için ışık, nem ve bakım sıklığından en az ikisi benzer olan, ayrıca mevcut koşullara uygun türler gösterilir; en çok benzerliği olan önce gelir. Mevcut türler önerilerden çıkarılır. Bu eşik prototip ürün kuralıdır, bilimsel başarı puanı değildir. Tür detayında koşullu/eksik değerlendirme korunur. Genel öneride uyumsuz türler listelenmez. 41 otomatik kontrol geçti; gerçek tarayıcı kontrolü yapılmadı.

## Kaynaklı katalog genişletmesi

4 Ekim 2026: seçim kataloğuna 79 kayıt eklendi; toplam 97 kayıt (cins seçimleri dahil). PLNTS'in Philodendron, Anthurium, Alocasia, Begonia ve Monstera koleksiyon sayfaları ile Ecuagenera Monstera/Anthurium katalogları kullanıldı. Yeni kayıtların kaynak URL’si ve kontrol tarihi gömülü katalogda ve work/plant-catalog-additions.json içinde tutulur. Saksı boyu ve Baby ayrımı ayrı bitki olarak eklenmedi. Katalog adları taksonomik otorite veya popülerlik sıralaması değildir; tür/kültivar/ticari adlar içerir. Bakım öneri verisi bu işlemle genişletilmedi; eksik profillerden öneri üretilmez.

Aramadaki sekiz sonuç sınırı kaldırıldı. Sonuç sayısı, 300px (mobilde 240px) kaydırılabilir liste ve görünür scrollbar stili eklendi. İşletim sisteminin scrollbar gizleme tercihi görünürlüğü etkileyebilir. Philedendron/filodendron, alokasya, antoryum, begonya aramaları desteklenir.

Sürdürülebilir güncelleme: kaynaklı yeni kayıtları mevcut kimliklere eşleştir, eş anlamlı ve kültivar ayrımlarını incele, editör kontrolü sonrası kataloğa al. Canlı arama üçüncü taraf sitesine bağlı değildir; demo çevrimdışı çalışır. Otomatik periyodik çekme veya sağlayıcı entegrasyonu kurulmadı.

## Açık soru, özel mesaj ve faydalı oyu — 5 Ekim 2026

İlan/içerik detayları ve üretici profillerine Sorular ve yanıtlar eklendi. Soru sor formunda açık veya özel seçilir; alıcı tercihlerine uyulur. Hesabım → Mesajlarım & gelen sorular üzerinden taraflar demo hesaplarıyla yanıt verebilir. Bir soru ve bir düzenlenebilir yanıt desteklenir; çok mesajlı sohbet/takip yanıtı, kullanıcı engelleme ve bildirim teslimi henüz yoktur. Açık soruların ilk üçü sayfada, tümü ayrı görünümde açılır. Yönetici açık soruyu gizleyebilir. Günlük 10 soru demo sınırı vardır.

Profil sahibiyle eşleştirilebilen yayındaki makale/deneyimler ve açık yanıtlar için Faydalı buldum oyu eklendi. Her farklı hesaptan tekil oy +2 itibar; kaldırılan oy puanı geri alır. Kendi kendine oy ve özel yanıt oyu yoktur. Profilde ve Hesabım'da itibar görünür. İçerik listeleri faydalı oyuna göre önceliklenir; sıfır oyda önceki sıra korunur. Bu, bot/sahte hesap tespiti içermeyen basit demo kuralıdır.

Özel mesajlar genel sayfalarda ve ilgisiz hesapların mesaj kutusunda gösterilmez; HTML dışa aktarımından çıkarılır. Ancak tüm demo verisi yerel tarayıcıdadır ve hesap seçimi serbesttir: gerçek gizlilik/kimlik güvenliği sağlamaz. Gerçek kişisel bilgi girilmemelidir.

21 rol/avatar/soru-cevap kontrolü Node VM simülasyonunda geçti. Gerçek tarayıcı görsel ve tıklama kontrolü yapılmadı.

## 5 Ekim 2026 — Öğrenme rotaları ve kişisel kanal takibi pilotu
- 3D/Maker > İçerikler: herkese açık iki üç-adımlı rota, kaynak seçimi, isteğe bağlı YouTube embed, manuel ilerleme ve kişisel notlar.
- Prusa'nın 2016 arşivinden iki video: model/tarih uyarısıyla, evrensel cihaz talimatı olarak sunulmadan. Kaynak: https://blog.prusa3d.com/youtube-quick-tips_4116/
- Hesaba bağlı Premium simülasyonu; kişisel YouTube kanal URL ekleme, tekrar/URL kontrolü, takipten çıkma, bildirim açma/kapama, okunma durumu ve tekil örnek bildirim.
- Ücretsiz rota erişimi devam eder; Premium kapatıldığında bildirim üretimi durur. Kişisel öğrenme verileri HTML dışa aktarımından çıkarılır.
- Test: work/test-learning.cjs 10/10; mevcut work/test-qa.cjs 21/21. Bunlar VM/DOM stub akış testleridir; gerçek tarayıcı görünümü ve video oynatma doğrulanmadı.
- Sınırlar: Canlı kanal çözümleme, hobi uygunluğu doğrulaması, yeni video senkronizasyonu, gerçek abonelik ve bildirim teslimi yok. Notlar/kanallar aynı cihazdaki demo verisidir; gerçek hesap güvenliği sunmaz.
- Sonraki canlı kapsam: kanal kimliğini sunucuda çözümleme, video bazında hobi uygunluğu, tekil video ID ile bildirim deduplikasyonu, erişime kapalı/silinmiş videoları ele alma, editör kanal yönetimi. Platformdan çıkışı engelleme; öğrenme notu, ilerleme ve topluluk katkısıyla geri dönüş nedeni oluşturma.
