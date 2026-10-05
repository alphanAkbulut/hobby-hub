# Hobby Hub v3 — Üretici vitrinleri

## Yeni yapı

v2 korunarak `hobby-hub-demo-v3.html` oluşturuldu. Bitkiler için 10, tüm hobilerde toplam 18 kurgusal üretici/koleksiyoner profili bulunur. Bu kişiler gerçek Shopier satıcıları değildir.

- Genel bakışta üretici vitrinleri üst seçkide görünür.
- Sol menü ve sekmelerde Üreticiler & Koleksiyonerler bölümü vardır.
- Üretici kartından Vitrini keşfet veya İlanları gör ile tek adımda ilgili ekrana gidilir.
- Kişisel sayfada Vitrin, İlanlar, Koleksiyon & üretim, Notlar ve Hakkında bulunur. Hizmet ve etkinlik sekmeleri yalnızca ilgili kayıt varsa açılır.
- Kişisel sayfada başka satıcıların ilanları gösterilmez.
- Vitrin başlığı, kapak, renk, hikâye, uzmanlık alanları, öne çıkan ilanlar, albüm ve notlar düzenlenebilir.
- Düzenleme önce önizlenir. Kaydetmeden mevcut ziyaretçi görünümü değişmez.
- Yeni ilan, seçili demo üreticisine bağlanır; moderasyon onayından sonra o kişinin İlanlar sekmesinde görünür.
- Takip seçimi bu cihazda saklanır; bildirim gönderilmez.
- HTTPS Shopier adresi eklenebilir. Entegrasyon veya stok eşitlemesi yoktur.
- Vitrinler ve alt sekmeleri dosya içindeki doğrudan adreslerle açılır; Geri/İleri ve breadcrumb bağlamı korunur.

## Hızlı deneme

1. v3 HTML dosyasını bilgisayarında tarayıcıyla aç.
2. Bitkiler → Üreticiler & Koleksiyonerler bölümüne gir.
3. Kök Atölye kartında İlanları gör seç: yalnız o kişinin ilanları açılır.
4. Vitrin sekmesine geç, albümü ve notları incele.
5. Vitrinimi düzenle ile başlığı, renk temasını veya bakım notunu değiştir.
6. Değişiklikleri önizle; ardından Vitrini kaydet · Demo seç.
7. Vitrinim / Vitrinimi yönet alanından başka bir demo kişisi seçerek akışı tekrar dene.

## Paylaşım ve sınırlar

Dosya tek başına çalışır; görseller gömülüdür. Vitrini paylaş penceresi aynı dosyadaki doğrudan adresi gösterir. Yerel dosya adresi başka bilgisayarda açılmaz: arkadaşlarına HTML dosyasını gönder. Mevcut düzenlemelerle paylaşmak için Mevcut demoyu indir kullanılabilir. Canlı web adresi oluşturulmadı.

Demo kişilerinin değiştirilmesi gerçek hesap oturumu veya güvenlik sınırı değildir. Kimlik doğrulama, sunucu veritabanı, gerçek upload, bildirim, ödeme ve dış platform senkronizasyonu bulunmaz. Galeri/kapak düzenlemede hazır temsili görseller seçilir. Notlar demo kaydı olarak hemen yayınlanır; üretim sürümü için içerik moderasyonu gerekir.

v3 ayrı yerel kayıt anahtarı kullanır. v2 tarayıcı değişiklikleri otomatik aktarılmaz; v2 dosyası ve kayıtları korunur. Üretim veri modelinde profil ile ilan/içerik bağları kalıcı profil kimliğiyle tutulmalıdır; demo isim değişiminde ilişkili kayıtları birlikte günceller.

## Doğrulama

JavaScript sözdizimi kontrolü ve **23/23** kod düzeyi kontrol geçti. Node VM ortamında render, olay işleyici, veri ve tarayıcı geçmişi simülasyonu kullanıldı. Gerçek tarayıcı görsel/tıklama doğrulaması veya cihazlar arası test yapılmadı. İndirme ve yeniden açma akışının tarayıcı testi de açıktır.

- 10 plant profiles / 18 total: PASS
- Creator spotlight before editorial and marketplace: PASS
- Directory accessible in sidebar and tabs: PASS
- Directory filters name + city: PASS
- Creator links go to own listings in one navigation: PASS
- Back restores directory: PASS
- Seller entry opens full routed profile: PASS
- Profile breadcrumb includes person and subpage: PASS
- Services only when profile has services: PASS
- Follow persists and preserves page: PASS
- Owner editor opens: PASS
- Preview does not mutate live data: PASS
- Publish updates profile, notes and storage: PASS
- Profile rename retains own listings and content: PASS
- Reject non-Shopier URL and crafted hostname: PASS
- Other creator cannot be edited without demo account selection: PASS
- Demo account switch routes to selected creator: PASS
- Share explains file-only limitation: PASS
- Section navigation clears personal route: PASS
- New listing category navigation remains intact: PASS
- Unknown profile safely falls back: PASS
- Profile theme and user text are bounded/escaped: PASS
- New listing belongs to selected creator after moderation: PASS

Dosya boyutu: 760,537 bayt. SHA-256: `02e7b9f3f31d745c855c63a26e97fa37ab2806111fc579d2eb3462257b85f02b`.
