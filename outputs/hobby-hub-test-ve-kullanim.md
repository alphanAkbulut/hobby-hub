# Hobby Hub v2 — Kullanım ve doğrulama

**Teslimat:** `hobby-hub-demo-v2.html` · tek dosya, çevrimdışı temel akışlar  
**Son düzenleme:** 4 Ekim 2026  
**Önceki sürüm:** `hobby-hub-demo.html` korundu.

## v2'de değişen görünür öncelik

- Açılış seçkisinde rehber, uzman ve etkinlik birlikte bulunur.
- Topluluk hikâyeleri ilan bölümünden önce gelir.
- Sol tarafta önce keşif alanları, ardından ilan kategorileri vardır.
- Fiyat ve hobi özellik filtreleri İlanlar bölümünde görünür.
- Üstte Paylaş menüsü hem deneyim hem ilan eklemeyi sunar.
- Yapılandırma, bölüm görünürlüğü ve moderasyon akışları korundu.

## Nasıl açılır ve paylaşılır?

HTML dosyasını bilgisayarına indirip Chrome, Safari veya Edge gibi bir tarayıcıda aç. Başka dosya veya kurulum gerekmez. E-posta / mesaj önizlemeleri etkileşimleri çalıştırmayabilir; dosya indirildikten sonra açılmalıdır. Dış kaynak bağlantıları için internet gerekir.

Arkadaşlarına yalnız `hobby-hub-demo-v2.html` dosyasını gönderebilirsin. Yerel değişiklikleri de göndermek için Demo rehberi içindeki **Yapılandırılmış demoyu indir** düğmesini kullan. Bu dışa aktarma akışının gerçek tarayıcıda indirme doğrulaması henüz yapılmadı.

Veriler her tarayıcıda ayrıdır. v2, v1'in kayıt alanını değiştirmez. Tarayıcı depolamayı engellerse değişiklikler bellekte kalır ve bir uyarı gösterilir. Demoda gerçek hesap, mesaj iletimi, ödeme, rezervasyon veya güvenli yönetici yetkisi yoktur.

## Önerilen deneme turu

1. Bitkiler'de “Hobinde bugün” alanından rehberi aç.
2. “Uzmanı tanı” ile profili incele ve bir demo teklif talebi kaydet.
3. Etkinlik programını aç; ayrıca “Hafta sonu bitki takas buluşması”nda dolu kontenjan / bekleme listesi örneğine bak.
4. Topluluk hikâyesini aç ve deneyim paylaşımı oluştur. Kayıt önce incelemeye gider.
5. İlanlar → Tropikal bitkiler → Monstera. Bitki formunu veya fiyat aralığını değiştir.
6. Bir ilanı aç; satıcı vitrini, kullanım galerisi ve favoriye eklemeyi dene.
7. Üst aramaya “saat” yaz; tüm hobiler kapsamındaki farklı sonuç türlerini karşılaştır.
8. Backoffice → Hobiler → Yeni hobi. Örneğin “Parfüm” taslağı oluştur; kategori ve seçim özelliği ekle.
9. “Yayınla · Demo” ile yeni hobi ziyaretçi menüsüne gelsin. Bölüm kapatmanın seçkiyi de etkilediğini kontrol et.
10. Paylaş → İlan oluştur. Backoffice moderasyonundan gerekçeli onay ver; ziyaretçi görünümünde kaydı bul.

## Test sonucu ve kapsam

**37 / 37 kod düzeyi kontrol geçti.** JavaScript sözdizimi kontrolü de geçti.

Yöntem: Node VM içinde veri modeli, HTML üretim fonksiyonları ve olay işleyicileri çalıştırıldı. DOM, form ve depolama için kontrollü test nesneleri kullanıldı. Bu testler gerçek tarayıcıda tıklama, form doğrulaması, focus davranışı, viewport görüntüsü veya kullanıcı testi yerine geçmez.

Yerel `file://` adresi uygulama tarayıcısının URL politikası tarafından engellendi. Geçici yerel önizleme izni sonuçlanmadığı için tarayıcı testi yapılmadı. Bu engeli aşmak için başka tarayıcı yüzeyi veya düşük seviyeli yol kullanılmadı.

| Kontrol | Sonuç |
|---|---|
| Başlangıç verisi: dört hobi ve 24 görünür ilan | Geçti |
| Ana sayfa seçkisi ilanlardan önce gelir | Geçti |
| Keşfet sayfasında ilan filtresi yok | Geçti |
| İlan sekmesi fiyat ve hobi filtrelerini açar | Geçti |
| Kategori ağacında ebeveyn tüm alt ilanları içerir | Geçti |
| Monstera kategorisi üç ilan getirir | Geçti |
| Facet filtreleri birlikte uygulanır | Geçti |
| Filtre temizleme kategori bağlamını korur | Geçti |
| Artan fiyat sıralaması | Geçti |
| Sıfır sonuç durumu görünür | Geçti |
| Global arama uzman ve ilanları bulur | Geçti |
| Türkçe arama normalizasyonu | Geçti |
| İlan detayında vitrin ve kullanım galerisi | Geçti |
| Favori ekleme ve kaldırma | Geçti |
| Satıcı vitrini açılır | Geçti |
| Uzman detayı portfolyo ve teklif içerir | Geçti |
| Dolu etkinlik bekleme listesi gösterir | Geçti |
| Talep yalnızca yerel kayda eklenir | Geçti |
| Paylaş menüsü ilan ve deneyim seçenekleri içerir | Geçti |
| Yeni ilan moderasyona düşer | Geçti |
| Moderasyon onayı ilanı görünür yapar | Geçti |
| Kullanım paylaşımı önce incelemede | Geçti |
| İçerik bildirimi ve gizleme | Geçti |
| Yeni hobi taslakta kalır | Geçti |
| Yeni kategori ve filtre kod yazmadan eklenir | Geçti |
| Yayınla yeni hobiyi ziyaretçiye taşır | Geçti |
| Yeni özelliğe göre dinamik ilan formu | Geçti |
| Bölüm kapatmak seçkiyi de kaldırır | Geçti |
| İlan bölümü kapatılınca kayıtlar global yüzeyden çıkar | Geçti |
| Geri dönüş önceki yapılandırmayı yükler | Geçti |
| Kendi altına kategori taşıma reddedilir | Geçti |
| İçerik formunda tehlikeli URL reddedilir | Geçti |
| Kullanıcı metni HTML olarak işlenmez | Geçti |
| Yapılandırma ve talepler yerel kayda yazılır | Geçti |
| Kaynakta harici script ve CSS bağımlılığı yok | Geçti |
| Küçük ekran stilleri ve reduced motion mevcut | Geçti |
| Tüm referans kategoriler ve öznitelikler mevcut | Geçti |

## Henüz doğrulanmayanlar

- Gerçek tıklama akışları ve modalın klavye / odak davranışı.
- 390 / 768 / 1280 / 1440 px görsel yerleşim ve %200 yazı büyütme.
- Safari, Chrome ve Edge'de yerel dosya / depolama farklılıkları.
- HTML indirme ve indirilen kopyanın yeniden açılmasının tarayıcıda kontrolü.
- WebMCP gezinme aracının destekli tarayıcıda kaydı ve çağrısı.
- Ekran okuyucu ve renk kontrastı uygunluğu.
- Saha performansı / yük testi ve production güvenlik testi.

## Dosya bütünlüğü

- `hobby-hub-demo.html`: 504,668 bayt; SHA-256 `bede4eafa9b6fd603681f921fd1e81d6f1328a177725ba427bcb224850c0d315`.
- `hobby-hub-demo-v2.html`: 703,992 bayt; SHA-256 `257bb103c52422efd8d3dc249b4680dee79db30fe479cf55a8b8f21be4d8a9e8`.

## Navigasyon düzeltmesi

Sol menüye Genel bakış eklendi; sağ sekme aynı adla güncellendi. Dört hobide 16 bölüm geçişinde iki navigasyonun seçili durumlarının eşleştiği kod düzeyinde doğrulandı. Mevcut 37 kontrol tekrar geçti. Tarayıcı tıklama doğrulaması yapılmadı.

## Breadcrumb ve URL tutarlılığı

Aktif bölüm breadcrumb’a eklendi; Bitkiler gibi hobi bağlantısı genel bakışı, ilan üst kategorileri kendi sonuçlarını açar. Bölüm değişiminde kategori, ilan filtreleri ve sıralama temizlenir. Sekme/kategori geçişleri geçmişe eklenir; Geri/İleri ve doğrudan URL okuması durumu yeniden kurar. Aynı ekranın yeniden çizimi yinelenen geçmiş üretmez.

Mevcut 37 kontrol geçti. Ek Node VM geçmiş simülasyonunda dört hobide 20 bölüm breadcrumb’ı, kategori ataları, filtre izolasyonu, geri/ileri, doğrudan adres ve bozuk/eski URL normalizasyonu doğrulandı. Gerçek tarayıcı doğrulaması yapılmadı.
