# Hobby Hub — Ürün keşfi, UX ve build planı

**Sürüm:** v2 · **Araştırma tarihi:** 3 Ekim 2026  
**Durum:** Ürün önerisi + yerel çalışan prototip. Üretim sistemi değildir.  
**İlgili demo:** `hobby-hub-demo-v2.html`  
**Temel karar:** Tek platform, hobiye özel keşif alanları; içerik, uzmanlık, öğrenme, topluluk ve ticaret aynı ürünün farklı giriş noktaları.

## 1. Önerilen ürün

Kullanıcı bir ürünü satın almaya karar vermeden de Hobby Hub'a gelmek için neden bulmalı: bir şey öğrenmek, güvenebileceği bir uzmanı bulmak, atölyeye katılmak veya kendi deneyimini göstermek. Alışveriş bu döngünün içinde anlamlı bir ihtiyaçtır.

Tek hesap, ortak arama, profil, medya, moderasyon ve yönetim altyapısı öneriyorum. Her hobi kendi kategori ağacına, özellik şemasına, içerik seçkisine ve operasyon kurallarına sahip olmalı. Ayrı domain ve bağımsız sitelerle başlamak içerik, kullanıcı kazanımı ve bakım işini çoğaltır; buna ihtiyaç duyulduğu henüz gösterilmiş değil.

Konfigürasyon kod tekrarını azaltır; her hobinin uzmanlığını ve operasyon yükünü ortadan kaldırmaz. Bitki çeliğinin sağlık durumu, bir saatin orijinalliği ve 3D tasarımın ticari kullanım hakkı ortak bir açılır listeyle çözülemez. Ortak çekirdek üzerine açıkça tanımlanmış domain kuralları gerekir.

**Konumlandırma önerisi:** “Hobinin insanlarını, bilgisini ve ihtiyaçlarını bir arada bul.” Hobby Hub şimdilik çalışma adıdır. Domain ve marka uygunluğu bu çalışma kapsamında yeniden doğrulanmadı; referans konuşmadaki eski domain iddiaları karar kanıtı olarak kullanılmadı.

### Kullanıcı ihtiyaçları ve doğrulanacak hipotezler

| Kullanıcı | Asıl iş | İhtiyaç kanıtı nasıl toplanır? | Öncelikli akış |
|---|---|---|---|
| Yeni başlayan | Yanlış ürün almadan öğrenmek | Son hobi başlangıcını anlatması; aradığı kaynakların incelenmesi | Rehber → uzman veya başlangıç etkinliği |
| Deneyimli hobici | Belirli bir parçayı bulmak; bilgisini paylaşmak | Son alışveriş ve paylaşım yolculuğu | Derin kategori / arama → ilan; koleksiyon → paylaşım |
| Hobi üreticisi | Doğru kişiye ulaşmak; üretimini göstermek | Mevcut satış kanalları ve tekrarlanan müşteri soruları | Vitrin → ilan → kullanım örnekleri |
| Uzman / eğitmen | Nitelikli talep almak | Son taleplerin kapsamı, yanıt süresi, fiyatlandırma şekli | Hizmet / etkinlik → kapsamlı talep |
| Editör / moderatör | Kaliteyi koruyarak alanı büyütmek | Gerçekçi kuyruk üzerinde görev testi | İnceleme → gerekçeli karar → itiraz |

**Hipotez:** İçerik ve topluluk geri dönüş sıklığını artırabilir. Bu araştırma kullanıcı retansiyonunu veya Türkiye'deki pazar büyüklüğünü kanıtlamaz. İlk pilotta davranışla ölçülmelidir.

## 2. Global benchmark

Araştırma doğrudan ürün sayfaları ve platformların resmî yardım / yayın içeriklerine dayanır. Pinkbike'ın desktop görüntüsü ve kategori yapısı, Houzz'ın profesyonel keşif ekranının erişilebilir arayüz yapısı ayrıca incelendi. Diğer örneklerde kaynak metni ve sayfa yapısı üzerinden değerlendirme yapıldı; hepsinde oturum açılarak uçtan uca işlem yapıldığı iddia edilmez. Özellikle eski tarihli rehberler güncel piksel yerleşiminin kanıtı olarak kullanılmadı.

| Platform ve kaynak | Kaynakta görülen desen | Hobby Hub için karar | Taşımayacağımız yük |
|---|---|---|---|
| [Etsy: arama görünürlüğü](https://www.etsy.com/seller-handbook/article/1289139008351), [müşteri görselleri](https://help.etsy.com/hc/en-us/articles/360000572708-How-the-Review-System-Works-for-Sellers) | Mağaza kimliği ve ilan kalitesi; yorumlarda fotoğraf / video | Satıcı adı, görsel kimlik, üretim hikâyesi ve kullanım galerisi. İşlem doğrulaması ayrı etiket | Gerçek doğrulama olmadan güven rozeti ve yıldız üretmek |
| [eBay: arama kullanımı](https://www.ebay.com/help/buying/bidding/bidding?id=4006) | Üst arama ve solda ürün özellikleri, durum, alış biçimi, teslimat filtreleri | Desktop'ta kalıcı kategori; ilan sayfasında facet, seçili filtre ve sıralama | Hobi keşif sayfasını satın alma filtreleriyle doldurmak |
| [Reverb: arama rehberi](https://reverb.com/news/tips-for-making-great-searches-on-reverb), [fırsat keşfi](https://reverb.com/uk/news/how-to-find-the-best-deals-on-reverb) | Alan diline uygun marka / durum filtreleri; rehber ve fırsat içerikleri | Hobiye özel özellikler, ayrı editoryal keşif, kaydedilen arama | İlk günden fiyat endeksi, teklif pazarlığı ve bildirim motoru |
| [Chrono24](https://www.chrono24.com/) | Saat kategorileri; Magazine, Watch Collection ve işlem güveni aynı ürün ailesinde | İçerik ile koleksiyon alışverişini ilişkilendir; servis geçmişi ve referans gibi alanları açık tut | Gerçek süreç kurulmadan escrow / orijinallik garantisi vermek |
| [Houzz: profesyoneller](https://www.houzz.com/professionals), [Ideabooks](https://www.houzz.com/magazine/how-to-create-and-use-ideabooks-stsetivw-vs~19764256) | Hizmet türü ve konumla uzman bulma; görselleri, hikâyeleri ve profilleri kaydetme | Uzman vitrini, yapılan işler, çalışma biçimi, teklif talebi; kullanım görselinden uzmana geçiş | Başlangıçta proje yönetimi, CRM ve kapsamlı randevu takvimi |
| [Discogs: koleksiyon / istek listesi notları](https://support.discogs.com/hc/en-us/articles/360007425393-How-Can-I-Add-Collection-Wantlist-Notes) | Koleksiyon ve istek listesi; marketplace ile uyumlu kondisyon alanları | Koleksiyon nesnesi ile satış ilanını ayrı düşün. MVP'de kaydetme; sonraki fazda koleksiyon | Tüm hobilere aynı “katalog ürünü” varsayımını zorlamak |
| [Pinkbike BuySell](https://www.pinkbike.com/buysell/) | Çok derin spor ekipmanı kategorileri, konum, ilan sayıları; haber ve topluluk navigasyonu | Domain derinliği korunmalı; kategoriler uzmanların kullandığı dille adlandırılmalı | Desktop görüntüsündeki yoğun listeyi ve reklam ağırlığını kopyalamak |
| [AquaBid kategorileri](https://www.aquabid.com/categories/?lang=en_US) | Tatlı su, cichlid, omurgasız ve bitki kırılımları | Akvaryumu tek “balık” kategorisine indirgememek | Açık artırma ve canlı sevkiyatı operasyonunu MVP'ye almak |
| [Ravelry hakkında](https://www.ravelry.com/about), [tasarımcıların projelerle ilişkisi](https://blog.ravelry.com/designers-welcome/) | Belirli bir hobi etrafında proje, desen ve insanların ilişkisi; kullanıcı uygulamaları | “Kullananlardan” galerisini ürün / üretici / proje arasında ilişkilendirmek | Genel amaçlı sosyal ağ veya sınırsız forum yapısı |
| [Instructables](https://www.instructables.com/), [topluluk projeleri](https://www.instructables.com/Teacher-Approved-DIY-Projects/) | Proje yaparak öğrenme ve topluluk örnekleri | Maker'da rehber → atölye → üretim paylaşımı döngüsü | Kapsamlı video kurs platformu ve sertifikasyon |

**Çıkarım:** Tek bir referansı kopyalamak yeterli değil. Arama ve taxonomy için eBay/Reverb/Pinkbike; görsel kimlik ve uygulama kanıtı için Etsy/Houzz/Ravelry; alışveriş dışı geri dönüş için Chrono24/Instructables birlikte daha uygun bir model oluşturuyor. Bu bir tasarım sentezidir, kanıtlanmış dönüşüm artışı iddiası değildir.

## 3. Desktop web UI/UX kararı

### v1 → v2 değişikliği

İlk demo ilanları en üstte bir ürün grid'iyle sunuyordu. Kullanıcı geri bildirimi üzerine v2'de bilgi hiyerarşisi değiştirildi:

1. Kısa hobi kimliği ve üstte global arama.
2. **Hobinde bugün:** görünür bir rehber, uzman ve etkinlik aynı seçkide.
3. Yeni editoryal içerikler ve topluluk hikâyeleri.
4. Hobiden hobiye ürünler / ilanlar.
5. Açık koşulları olan fırsatlar.

Üstteki birincil eylem **Paylaş**: kullanıcı deneyimini veya ilanını paylaşabilir. Sol sütunda önce içerik, uzman, etkinlik ve topluluk girişleri; ardından ilan kategori ağacı vardır. Fiyat ve ürün filtreleri yalnızca ilan bağlamında açılır. Bu düzen alışveriş akışını saklamadan platformun diğer değerlerini görünür kılar.

### Ekran ve etkileşim sözleşmeleri

| Alan | Önerilen davranış | Önemli edge case |
|---|---|---|
| Global search | Üstte kalır. Kapsam: tüm hobiler veya seçilen hobi. Sonuçlar türlerine göre gruplanır | Uzman sonucu fiyat filtresiyle yanlışlıkla elenmez; boş arama keşfe döner |
| Hub landing | Bir içerik, uzman ve etkinlik seçkisi; ardından konfigüre bölümler | Bir bölüm kapalıysa seçkide veya global aramada da görünmez |
| Kategori ağacı | Ebeveyn / çocuk ilişkisi, ilan sayısı, seçili kategori ve breadcrumb | Sıfır ilanlı kategori gösterilebilir; “0” gizlenmez. Ebeveyn tüm alt dalları kapsar |
| Faceted filters | Fiyat, konum, tür, teslimat ve bağlama uygun özellikler | Filtreler birlikte uygulanır; boş sonuçtan çıkış ve tek tek kaldırma vardır |
| Listing detail | Görsel, fiyat, nitelikler, durum, teslimat, satıcı ve bildirim | Eksik servis geçmişi “bilinmiyor” olur; “yok” kabul edilmez |
| Seller showcase | Kimlik, hikâye, vitrin, ürünler, kullanım örnekleri | Aynı kişi satıcı ve uzman olabilir; rozetler gerçek kontrol türünü açıklamalı |
| Customer media | Ürüne / sağlayıcıya bağlı uygulama örnekleri | Onaylı paylaşım, satın alması doğrulanmış yorum demek değildir |
| Services | Uzmanlık, portfolyo, konum, çalışma şekli, başlangıç bedeli / teklif | Başlangıç bedeli kesin fiyat değildir; tek tuşla kesin rezervasyon yapılmaz |
| Courses/events | Tarih, süre, seviye, format, organizatör, ücret, kontenjan | Başvuru, bekleme listesi ve kesin katılım ayrı durumlar |
| Offers | Sağlayıcı, indirim, alt limit, üst sınır, bitiş tarihi, kapsam | Süresi dolan / doğrulanamayan fırsat ayrılır; sponsorlu içerik etiketlenir |
| Aggregated content | Kaynak adı, format, kısa özgün özet, yayın tarihi, kaynak linki | Tam makale kopyalanmaz; kaynak kaldırıldıysa kart gözden geçirilir |
| Backoffice | Taslak → yayınla → geri dön; moderasyonda gerekçeli karar | Şema değişikliği mevcut ilanları sessizce geçersizleştirmez |

### İçerik toplama yaklaşımı

MVP'de editör kontrollü kaynak seçkisi: başlık, izinli görsel, özgün kısa özet ve dış bağlantı. Resmî RSS / API desteği olan kaynaklar ikinci adımda bağlanabilir. Kaynak bilgisi, özgün yayın tarihi ve son kontrol tarihi ayrı tutulmalı. Aynı içeriğin birden fazla feed'den gelmesi canonical URL veya sağlayıcı kimliğiyle tekilleştirilmeli.

Video kartı otomatik oynatılmaz. Kullanıcı açmak istediğinde izinli embed yüklenir; bozuk / bölgesel olarak erişilemeyen video için kaynağa git seçeneği bulunur. Gömme davranışı sağlayıcının resmî parametreleriyle uygulanmalıdır. [YouTube embed dokümantasyonu](https://developers.google.com/youtube/player_parameters).

**Demoda:** Editoryal örnek metinler ve iki açık kaynak bağlantısı var. Canlı RSS, otomatik scraping, video oynatma veya dış API çağrısı yok.

### Erişilebilirlik ve farklı ekranlar

Desktop ana hedef: 1280–1440 px genişlikte sol navigasyon ve içerik alanı. Dar ekranda sol panel bir düğmeyle açılır, sekmeler yatay kayar, grid iki sütuna iner. Modal için doğal HTML dialog, klavye odağı, Escape ile kapanma; alanlarda açık etiketler ve görünür focus stilleri kullanıldı.

Üretim kabulü için 390 / 768 / 1280 / 1440 px, %200 metin büyütme, yalnız klavye ve ekran okuyucu ile ayrıca kontrol gerekir. Demo için bu viewport'ların gerçek tarayıcıda görsel kontrolü tamamlanmadı. Stil dosyasının responsive kurallar içermesi, erişilebilirlik uygunluğu kanıtı değildir.

## 4. İlk dört hub ve pilot stratejisi

Dört hub ürün modelini görünür kılmak için iyi bir örneklem. Ancak dördünde aynı anda derin arz yaratmak operasyonu gereksiz büyütebilir. **Önerim: dört hub konfigüre edilsin; Bitkiler ve 3D/Maker ilk kontrollü pilot, Akvaryum ve Saatler koşullu genişleme olsun.** Kullanıcının dört alanı birlikte görme ihtiyacı demoda karşılandı.

| Hub | Öğrettiği davranış | İlk kapsam | Açılış koşulu / risk |
|---|---|---|---|
| Bitkiler | Çoğaltma, yerel üretim, bakım içeriği, görsel paylaşım | Tropikal koleksiyon bitkileri, saksı / ekipman, bakım danışması | Tür, sağlık ve paketleme açıklıkları; hassas türler için uzman değerlendirmesi |
| 3D / Maker | Üretici vitrini, ekipman ve özel hizmet | Yazıcı, fiziksel baskı, atölye ve baskı hizmeti | Tasarım hakkı, tehlikeli / yasak kullanım politikaları; dijital dosya lisansı sonraki faz |
| Akvaryum | Derin taxonomy, kurulum hizmeti ve canlı bakımı | Önce ekipman, bitki ve eğitim; canlılar ayrı açılış kontrolü | Tür / sağlık / sevkiyat politikası ve deneyimli moderatör gerekir. Demoda elden teslim örneği |
| Saatler | Koleksiyon, ikinci el, tamir ve güven | Rehberler, uzman portfolyosu, sınırlı ilan pilotu | Sahte ürün, servis geçmişi, yüksek değerli uyuşmazlık ve sigortalı taşıma |

Bu önceliklendirme doğrulanmış pazar hacmi sıralaması değildir; kapsam ve operasyon riskine dayalı ürün yargısıdır. Pilot katılımcılarına erişim veya güvenilir bir vertical lideri varsa sıra değişebilir.

### Örnek kategori paketleri

- **Bitkiler:** Tropikal → Monstera / Anthurium / Alocasia / Philodendron; Sukulent & kaktüs; Bonsai; Saksı & ekipman → Saksılar / Yetiştirme ışıkları.
- **Akvaryum:** Tatlı su → Cichlid → Malawi / Tanganyika; Karides & omurgasız; Akvaryum bitkileri; Deniz akvaryumu; Tank & ekipman → Tank / Filtre & aydınlatma.
- **Saatler:** Kol saatleri → Mekanik → Otomatik / Elle kurmalı; Quartz; Vintage koleksiyon; Kordon & aksesuar → Kordon / Bakım araçları.
- **3D/Maker:** 3D yazıcılar → FDM / Reçine; Sarf → PLA / PETG; Üretilen ürünler → Saksı & dekorasyon; Yedek parça & aksesuar.

Ağaç bir alışveriş navigasyonudur, biyolojik veya teknik sınıflandırmanın eksiksiz modeli değildir. Vintage gibi kesişen özellikler üretimde facet veya editoryal koleksiyon da olabilir. Mükerrer kategori dalları yaratmadan bu karar domain temsilcileriyle verilmelidir.

## 5. MVP ve faz planı

Süreler bir deneyimli geliştirici, düzenli ürün / tasarım desteği ve yarı zamanlı içerik-operasyon sorumlusu varsayımıyla **planlama aralığıdır**; teklif veya taahhüt değildir. En büyük belirsizlik teknoloji değil ilk kaliteli arzın ve editoryal ritmin kurulmasıdır.

| Faz | Kapsam / somut çıktı | Tahmini efor aralığı | Çıkış kapısı |
|---|---|---|---|
| 0 — Problem ve kullanılabilirlik doğrulaması | Bu demo; 12–16 kullanıcı / üretici / uzman görüşmesi; 8 görev testi; pilot arz listesi | 1–2 hafta | Ana ihtiyaç ve hangi vertical'da arz sağlanabildiği belirlenir |
| 1 — Davetli MVP | Hesap, iki pilot hub, şemalı ilan, editoryal içerik, uzman profili, etkinlik rehberi, kaydetme, talep, raporlama, backoffice | 6–10 hafta | Gerçek kullanıcıyla baştan sona görevler; yetki ve yedek geri dönüş testleri geçer |
| 2 — Operasyon ve dört hub | Akvaryum / Saat koşullarının tamamlanması; koleksiyon, kaynak bağlantıları, moderasyon itirazı, sınırlı bildirim | 4–6 hafta | Moderasyon yükü sürdürülebilir; yeterli arz ve yanıt kalitesi |
| 3 — İşlem katmanı | Ödeme, satıcı onboarding, sipariş, iade / uyuşmazlık, kargo durumu; önce düşük riskli ürün grubu | Keşif sonrası yeniden tahmin | Sağlayıcı sözleşmesi, sandbox ve finansal mutabakat senaryoları doğrulanır |

### MVP kapsamı

**Dahil:** Web-first hub, kaynaklı içerik, kategori / özellik / filtre konfigürasyonu, ilan ve satıcı vitrini, kullanım galerisi, uzman ve etkinlik rehberi, nitelikli talep, favori, içerik bildirimi, editör ve moderatör iş akışları. İçerik, hizmet ve etkinlik ürünün açılış değerinin parçasıdır.

**Kapsam dışı:** Mobil uygulama, gerçek zamanlı forum / chat, açık artırma, otomatik orijinallik garantisi, ödeme ve cüzdan, kurs video barındırma, canlı kargo orkestrasyonu, tam otomatik öneri sistemi, AI destekli otomatik moderasyon kararı, mikroservislere bölünme.

**Gelir hipotezi:** Ücretsiz temel hobici kullanımı; uzman vitrini ve açıkça etiketlenen ilgili sponsorlu konumlar. Ücretli uzman talebi veya aboneliği ancak sağlayıcı değeri ölçüldükten sonra. İlan komisyonu işlem ve uyuşmazlık altyapısı kurulmadan ana model olmamalı.

### Başarı ölçümü

İlk ürün metriği yalnız ilan görüntüleme olmamalı. **Haftalık anlamlı hobi etkileşimi yaşayan aktif kişi:** rehberden ilişkili bir adım atma, uzman profili sonrası talep, etkinlik başvurusu, onaylı paylaşım veya satıcıya nitelikli soru. Aynı kişinin tekrarlı tıklamaları tekil sayılmalı; türler ayrıca raporlanmalı.

Pilot için önerilen, henüz doğrulanmamış eşikler:

- 8 görev testinde en az 6 kişi yardım almadan içerik / uzman / etkinlik bulabilsin.
- En az 6 kişi kategori ve filtreyle hedef ilanı iki dakika içinde bulabilsin.
- Her pilot hub'da açılıştan önce en az 5 etkin sağlayıcı / üretici, 20 nitelikli ilan, 8 içerik ve 2 etkinlik kaydı hazırlansın. Bunlar arz planı hedefidir, mevcut kayıt sayısı değildir.
- Talep yanıt süreleri, 7/28 günlük geri dönüş ve sıfır sonuç oranı baseline olarak ölçülsün; keyfî “sektör ortalaması” kullanılmasın.
- İçerik, uzman, etkinlik ve ilan tıklama payları ayrı izlensin. İlan dışı akışların görünür olması, tek başına değer ürettikleri anlamına gelmez.

Üretimde olaylar: `hub_view`, `section_open`, `search_submitted`, `search_empty`, `filter_applied`, `content_open`, `source_click`, `provider_view`, `lead_submitted`, `event_interest`, `listing_view`, `favorite_added`, `media_submitted`, `moderation_decision`. Demo üçüncü taraf analitik çağrısı yapmaz.

## 6. Konfigüre edilebilir mimari

### Çekirdek ilişkiler

```text
Hobby
 ├─ CategoryTree (versioned) → Category (parent_id)
 ├─ ListingTypePolicy → allowed category + AttributeSchemaVersion
 ├─ AttributeSchema → fields, types, units, validation, applicability
 ├─ FilterSchema → attribute reference, UI control, ordering
 ├─ HubSection → enabled, order, layout, selected/promoted references
 └─ DomainPolicy → review rules, delivery eligibility, publication gates

Listing → Hobby + Category + ListingType + AttributeSchemaVersion
ContentItem → Hobby + topics + publisher/source/canonical URL
Service → ProviderProfile + expertise + service area + price mode
Course/Event → Organizer + session/format/time/capacity
Offer → provider + validity + terms + eligibility
CommunityPost/CustomerMedia → author + optional listing/provider + consent
Profile → one or more roles: hobbyist / seller / provider
Report → target + reason → ModerationCase → Decision → Appeal
ConfigRevision → draft / published / superseded + audit + rollback
```

Hizmet, kurs ve içerik, bütün alanları nullable bir “ilan” tablosuna sıkıştırılmamalı. Ortak kimlik, medya, etiket ve yayın durumu altyapısını kullanabilirler; fiyat, kapasite, takvim veya kaynak alanları kendi sözleşmelerinde kalmalı.

### Veri ve uygulama yaklaşımı

İlk gerçek ürün için modüler monolit, ilişkisel veritabanı ve nesne depolama yeterli bir başlangıçtır. Katalog/taxonomy, içerik, profil, talep ve moderasyon ayrı modüller olabilir; ayrı servisler şart değildir. Web sayfaları arama motorlarının ve paylaşım bağlantılarının okuyabileceği biçimde sunulmalı. Kesin framework ve sağlayıcı seçimi mevcut ekip yetkinliği / barındırma koşullarıyla yapılmalı; bu demoda yeni çalışma zamanı bağımlılığı yok.

Çekirdek alanlar tipli kolonlarda; hobiye özel değerler şema sürümüne bağlı kontrollü JSON veya tipli attribute-value kayıtlarında tutulabilir. Başlangıçta ilişkisel sorgu ve full-text arama; katalog büyüyüp facet sorgu süresi hedefi aşıldığında bağımsız indeks değerlendirilmeli. Arama indeksi ana veri kaynağı değildir; yayın durumu ve erişim kuralları her okuma yolunda uygulanır.

### Şema sözleşmesi örneği

```json
{
  "hobbyId": "watches",
  "categoryId": "automatic",
  "listingType": "used",
  "schemaVersion": 3,
  "attributes": {
    "movement": "automatic",
    "caseDiameterMm": 40,
    "boxIncluded": true,
    "serviceHistory": "unknown"
  }
}
```

`AttributeSchema` alanı örneğin `caseDiameterMm`: sayı, birim mm, min/max, kategori kapsamı, required. `FilterSchema`: aynı özelliğe referans, aralık kontrolü, gösterim sırası, facet hesaplama biçimi. Üretimde sayısal aralık filtresi gerekir; demoda hobiye özgü sayısal filtre mevcut değerleri listeleyerek basitleştirildi.

Kategori ve ilan türü uygunluğu sunucuda doğrulanır. Miras alınan şemalarda aynı alanın tipini çelişkili biçimde override etmek yayın anında engellenir. Boş değer, bilinmiyor, yok ve false farklı kalır. Temel ölçüler tek birimde saklanır; gösterim birimi ayrı olabilir.

### Backoffice yayın kuralları

1. Yapılandırmayı taslakta düzenle; kimlikler isimden bağımsız kalır.
2. Ağacın döngüsüz olduğunu, tüm parent ve alan referanslarını, tip / seçenek tutarlılığını kontrol et.
3. Mevcut ilanların kaçının değişiklikten etkilendiğini göster. Yeni zorunlu alanı geçmiş ilanlara sessizce dayatma.
4. Yeni şema sürümünü yayımla; yeni ilanlar bunu kullanır. Eskiler sürümünü korur veya kontrollü göç kuyruğuna girer.
5. İndeks / cache güncellemesini revision ile bağla; kısmi yayın sorununda önceki tutarlı revizyona dön.
6. Eşzamanlı yönetici düzenlemesinde optimistic locking ile çakışmayı göster. Kim, neyi, neden değiştirdi kaydı tutulur.

**Demoda uygulanan:** Hobi ekle / adlandır / aktiflik, kategori ekle / adlandır / taşı ve döngü engeli; alan tipi ve kapsamı; filtre görünürlüğü; bölümleri aç/kapat/sırala; içerik ekle/düzenle/sponsorlu işaretle; moderasyon; taslak yayınlama ve önceki yapılandırmaya dönüş. Kalıcı sunucu, eşzamanlı editör, veri göçü ve yetki sistemi yok.

## 7. Demo kapsamı ve paylaşım

v2 tek HTML dosyasıdır. Görseller, stil, uygulama kodu ve başlangıç verisi içindedir. Harici font veya script bağımlılığı yoktur. Açılışta ağ isteği yapmaz; dış kaynak bağlantısına tıklamak internet gerektirir.

Başlangıç içeriği: 4 hobi, 24 yayındaki + 1 incelemedeki ilan, 25 içerik/hizmet/etkinlik/fırsat/topluluk kaydı ve 1 örnek bildirim. İsim, bedel, organizasyon, etkinlik, medya ve uzmanlık bilgileri kurgusaldır. Saat görselleri markasız temsilidir; başlıktaki modelin ürün fotoğrafı oldukları iddia edilmez.

**Paylaş:** HTML dosyasını gönder; alıcı bilgisayarına indirip tarayıcıda açsın. E-posta / mesajlaşma önizlemesi JavaScript çalıştırmayabilir. “Demo rehberi → Yapılandırılmış demoyu indir” mevcut yerel veriyle yeni dosya üretir. Tarayıcı kaydı cihazlar arasında senkronize olmaz. Yeni indirilen kopya ayrı kayıt anahtarı kullanır; eski tarayıcı verisinin yeni başlangıç paketini gölgelemesi önlenir.

**Gerçek olmayan işlemler:** Kullanıcı hesabı, admin güvenliği, ödeme, kargo, e-posta / mesaj gönderimi, kesin rezervasyon, doğrulanmış satın alma, otomatik içerik toplama. Başvuru formu sadece yerel kayıt üretir ve bunu açıkça söyler. Müşteri medya akışında hazır görsel seçilir; gerçek dosya yükleme yoktur.

v1 dosyası korundu. v2 kendi yerel kayıt alanını kullanır; v1 değişikliklerini sessizce üzerine yazmaz.

## 8. Güvenlik, gizlilik ve moderasyon planı

Bu bölüm üretime geçiş tasarımıdır; tamamlanmış bir penetrasyon testi veya güvenlik sertifikası değildir.

| Risk / sınır | Üretim kontrolü | Doğrulama |
|---|---|---|
| Açık backoffice | Sunucu tarafında oturum, MFA ve rol/nesne bazlı yetki; least privilege | Editörün moderasyon, kullanıcının başka satıcının kaydı üzerinde işlem yapamaması |
| İlan / profil erişimi | Her endpoint'te ownership ve yayın durumu kontrolü | ID değiştirerek okuma/güncelleme; gizli kayıtların aramada görünmemesi |
| Kullanıcı metni / XSS | Girdi doğrulama, çıktı kodlama, rich text allowlist; CSP | Başlık, açıklama, URL ve medya metaverisinde saldırı girdileri |
| Upload | İzinli uzantı/MIME + dosya imzası, boyut/piksel sınırı, yeniden kodlama, karantina, tarama | Yanlış uzantı, çok büyük görsel, SVG/HTML, içerik tipi uyuşmazlığı |
| Kaynak içeriği alma / SSRF | Yalnız izinli kaynaklar, özel ağlara çıkışı engelleme, redirect kontrolü, zaman/boyut sınırı | Dahili IP, DNS ve redirect senaryoları |
| Hesap ve talep suistimali | Rate limit, e-posta doğrulama, risk bazlı challenge, spam kuyruğu | Bot ilanı, seri mesaj ve brute-force denemeleri |
| Gizlilik | Asgari veri, açık görünürlük seçimi, silme/saklama planı, EXIF temizleme | Dışa aktarılan medya/loglarda adres, konum ve token olmaması |
| Sırlar ve loglar | Sunucu secret store; log maskeleme; ayrı ortam anahtarları | Build çıktısında credential taraması ve log örnek incelemesi |
| Yapılandırma | Sürüm, çakışma kontrolü, etki önizlemesi, denetim izi | Yanlış şema yayını ve geri dönüş tatbikatı |

Yetki ve upload yaklaşımı için birincil teknik referanslar: [OWASP Authorization](https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Cheat_Sheet.html), [OWASP File Upload](https://cheatsheetseries.owasp.org/cheatsheets/File_Upload_Cheat_Sheet.html).

**Demo sınırı:** Metinler HTML escape ile yazılır, içerik kaynak adresi HTTPS ile sınırlandırılır; CSP bağlantı isteklerini engeller. Ancak sayfa içinde kod ve admin işlemleri kullanıcıya açıktır. `localStorage`, güvenilir veri deposu veya yetkilendirme değildir. Bu dosyaya gerçek müşteri / ödeme / kimlik bilgisi konulmamalıdır.

### Moderasyon işletimi

- Yeni ilan ve kullanıcı medya: `pending → published / rejected`. Bildirim içerikten ayrı kayıttır; tek bildirim otomatik suçluluk anlamına gelmez.
- Yayındaki içerik: bildirim → inceleme → içeriği koru / düzeltme iste / gizle. Karar, gerekçe, aktör ve zaman tutulur. İtiraz ikinci incelemeye gider.
- Yeni satıcılar ve riskli kategoriler için yayın öncesi kontrol; güvenilir geçmişte örneklem kontrolü. Önceliklendirme tehdidin ağırlığına göre yapılır.
- Saat: gerçek görsel, referans, kondisyon ve servis geçmişi; iddia edilen uzman doğrulamasının kapsamı açık olmalı.
- Bitki/akvaryum: tür ve sağlık bilgisi, yasaklı / kontrollü türler, canlı sevkiyatı ve bakım politikaları için ilgili uzman ve güncel hukuk incelemesi açılış kapısıdır.
- Maker: tasarım / marka / karakter hakları ve tehlikeli kullanım politikası. Dijital dosya ile fiziksel ürünü ayır.
- Kullanım galerisi: görsel kullanım izni ve ilişkilendirilen ürün; “satın alma doğrulandı” işareti yalnız gerçek işlem kaydı varsa.

Önerilen operasyon hedefi: ağır güvenlik/kişisel veri bildirimlerinde hızlandırılmış kuyruk; diğerlerinde bir iş günü içinde ilk inceleme. Bu hedef için görevli ve kapasite ayrılmadan kullanıcıya SLA taahhüdü verilmemeli.

## 9. Medya ve performans

Demodaki atlas yaklaşımı tek dosyada paylaşımı kolaylaştırır; üretimde tüm görselleri HTML'ye gömmek doğru ölçekleme değildir. Üretimde görseller nesne depolama + CDN üzerinden responsive türevlerle sunulmalı; sabit en/boy, uygun format ve görünüm altı lazy loading kullanılmalı. İlk görünümün baskın görseli öncelikli yüklenir; bütün kartlara preload yapılmaz.

Önerilen başlangıç bütçesi: kart türevleri çoğunlukla 40–100 KB; ilk ekran toplam medya yaklaşık 500 KB altında; video yüklemesi kullanıcı eylemine kadar ertelenir. Bunlar tasarım bütçesi hedefleridir, her fotoğraf için garanti değildir. Upload'da EXIF temizleme, boyut sınırlama, kalite ve renk kontrolü yapılmalı. Poster olmadan autoplay kullanılmamalı.

Gerçek kullanıcı verisinde p75 için hedefler: **LCP ≤2,5 sn, INP ≤200 ms, CLS ≤0,1**. Ölçüm cihaz ve sayfa tipine göre ayrılmalı. Yerel hızlı açılma, saha performansı kanıtı değildir. [Web Vitals](https://web.dev/articles/vitals?hl=en).

Arama ve facet için ölçülecek teknik hedef: ilk pilot veri setinde p95 API yanıtı 500 ms altında; ağır sorgular izlenir. Sınırsız offset yerine kontrollü sayfalama, metaveri indeksi ve sorgu bütçesi gerekir. Demo küçük diziler üzerinde bellek içi arama yapar.

## 10. Ödeme ve kargo için gelecek entegrasyonu

MVP'de talep / iletişim doğrulansın. Ödeme geldiğinde tek “başarılı” alanı yeterli olmaz:

```text
Order: draft → awaiting_payment → paid → fulfilling → delivered → completed
Payment: created / pending / authorized / captured / failed / refunded
Shipment: not_created / label_created / picked_up / in_transit / delivered / exception
Dispute: opened / evidence_requested / under_review / resolved
```

Sağlayıcı timeout'u `unknown` veya `pending` olabilir; doğrudan `failed` kabul edilmez. Webhook imzası ve tekrar önleme, idempotency key, sıra dışı olay geliş sırası, periyodik mutabakat ve yalnız doğrulanmış sonuca göre sipariş ilerletme tasarlanmalı. Para birimi, tutar ve satıcı hesap eşleşmesi doğrulanır. Kart verisi tutulmadan sağlayıcı arayüzüyle işlem yapılması tercih edilir.

Pazaryeri satıcı onboarding, tahsilat / komisyon / payout, kısmi iade, iptal, uyuşmazlık ve vergi/fatura sorumlulukları sağlayıcı ve hukuk incelemesinde netleşmeli. Bu çalışma belirli bir ödeme sağlayıcısının kullanılabilirliğini, ücretini veya mevzuata uygunluğunu doğrulamaz.

Kargoda kategori bazlı uygunluk matrisi: normal fiziksel ürün, kırılabilir tank, yüksek değerli saat ve canlı gönderimi aynı taşıma sözleşmesine zorlanmaz. Taşıyıcı event mapping, duplicate webhook, yanlış teslim, hasar, iade ve kayıp senaryoları sandbox / test ortamında doğrulanır. Demo elden teslim / kargo tercihlerini yalnızca gösterir.

## 11. Test, deployment ve bakım

### Tamamlanan doğrulama

- JavaScript sözdizimi kontrolü geçti.
- 37 model / HTML üretimi / olay işleyici kontrolü geçti. Filtre kombinasyonları, kategori soy ağacı, global arama, moderasyon, yeni hobi, şema, yayın / geri dönüş, bölüm görünürlüğü ve yerel kayıt kapsandı.
- Görseller dosyaya gömülü; harici script / CSS bağımlılığı ve başlangıç network çağrısı yok.
- **Gerçek browser tıklaması, görsel viewport kontrolü, ekran okuyucu, indirme akışının tarayıcıda readback'i ve çok tarayıcı uyumluluğu tamamlanmadı.** Yerel dosya adresi uygulama tarayıcısı tarafından engellendi; geçici yerel önizleme izni sonuçlanmadı. Bu kısıt aşılmaya çalışılmadı.

Ayrıntılı sonuçlar: `hobby-hub-test-ve-kullanim.md`.

### Üretime geçiş test kapıları

1. Model: kategori döngüsü, yetim kayıt, alan türü, zorunluluk, geçersiz enum, para ve tarih.
2. Arama: çapraz hobi, Türkçe karakterler, facet birleşimi, sıfır sonuç, gizlenen içerik, indeks gecikmesi.
3. Akış: hesap → ilan → moderasyon → görünürlük; rehber → uzman → talep; etkinlik → başvuru; rapor → karar → itiraz.
4. Yetki: rol matrisi, başka kullanıcının kaydı, admin MFA, CSRF, XSS, SSRF, medya işleme.
5. Görsel: desktop / tablet / mobil, uzun Türkçe başlıklar, çok kategori, %200 yazı, klavye, odak sırası.
6. Sağlayıcı: timeout, tekrar, eksik webhook, partial refund ve mutabakat.
7. Operasyon: yedekten geri yükleme, hatalı konfigürasyonu geri alma, üçüncü taraf kesintisi, medya kotası.

### Yayınlama

**Mevcut teslimat:** Yerel HTML, internete deploy edilmedi. Arkadaşlarla dosya olarak paylaşılabilir. Bu prototipin planlanan sonraki kontrolü tarayıcıdaki görünüm ve temel tıklamalardır.

**Demo linki istenirse:** Yalnız bu anonim demo dosyası ayrı statik alanda yayınlanır. HTTPS, noindex ve uygun güvenlik başlıkları; gerçek veri veya sunucu sırları yok. Backoffice'in demo olduğu görünür kalır. Dağıtım sonrası ana sayfa, dört hub, arama, admin ve dosya indirme linki hedef adreste yeniden kontrol edilir.

**Gerçek ürün:** Development → staging → production; ayrı hesap/anahtar/veri. Preview deployment'da smoke test, schema migration için geriye uyum, release etiketi ve rollback. Yönetim alanına server-side auth, sentetik veriyle staging. Domain, erişim politikası ve altyapı bütçesi netleştikten sonra yayınlanır. Mevcut dosyayı olduğu gibi “gerçek pazaryeri” diye yayınlamak yeterli değildir.

### Bakım sorumlulukları

| Ritim | Sorumlu rol | Kontrol |
|---|---|---|
| Günlük | Topluluk / moderasyon | Riskli bildirimler, bekleyen yayınlar, yanıtsız talepler |
| Haftalık | Editör / vertical sorumlusu | İçerik seçkisi, bozuk kaynaklar, tarihi geçen etkinlik / fırsat, taxonomy soruları |
| Haftalık | Geliştirici | Hata, arama yavaşlığı, medya işleme başarısızlığı, kota ve maliyet eğilimi |
| Aylık | Teknik sorumlu | Bağımlılık yamaları, izin incelemesi, geri yükleme örnek testi, alarm kalitesi |
| Her release | Ürün + teknik | Kabul kriterleri, regresyon yüzeyi, veri göçü ve geri dönüş |
| Üç aylık | Ürün + operasyon | Hub başına değer / arz / yük, kapatılacak veya açılacak kapsam |

Başlangıç planı için önerilen RPO 24 saat, RTO 4 saat; ödeme açıldığında işlem verisi için hedefler ayrıca sıkılaştırılır. Bu hedefler mevcut sistemde sağlanmış değildir. Hosting, veri, CDN, arama, e-posta, moderasyon ve destek maliyetleri ayrı izlenmeli; trafik yokken kesin maliyet tahmini üretilmemeli.

## 12. Öncelikli sonraki adım

v2'yi küçük bir kullanıcı grubuyla şu dört görevde test et: bir konu öğren, uygun uzman bul, etkinliğe başvur, belirli ilan bul. Kullanıcının ilk tıklamasını ve alışveriş dışı alanları fark edip etmediğini gözlemle. Ardından ilk pilot hub'ların gerçek sağlayıcılarını ve editoryal sorumlularını belirle. Backend yatırımına geçiş için en değerli belirsizlik bu iki alandadır.

**Açık kalan kararlar:** Gerçek pilot arzı, domain/marka, üretim bütçesi, erişim/üyelik modeli, yüksek riskli kategorilerin açılış koşulları ve ödeme sağlayıcısı. Bu kararlar demoyu incelemeyi engellemez; bu çalışma kapsamında dış sisteme bağlantı, ödeme veya deploy yapılmadı.
