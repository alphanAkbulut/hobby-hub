# Hobby Hub — Demo yetki modeli

5 Ekim 2026. Uygulanan dosya: hobby-hub-demo-v4.html.

| Rol | Yetki |
|---|---|
| Ziyaretçi | Açık içerik, vitrin ve uygunluk aracını kullanır. Backoffice görünmez. |
| Üye | Kendi vitrini ve paylaşımlarıyla çalışır; ilan ve deneyim gönderebilir. |
| Yönetici | Backoffice, moderasyon ve platform yapılandırması. Kullanıcı rollerini okuyabilir, değiştiremez. |
| Sistem sahibi | Yönetici yetkileri + rol atama/kaldırma ve demo sıfırlama. Son sistem sahibi korunur. |

Üretici, koleksiyoner ve uzman profil nitelikleridir; yönetim yetkisi değildir. İlk sürümde ayrı moderatör rolü yoktur.

## Deneme

Sağ üst Giriş yap → Demo hesabı seç. Kök Atölye başlangıçta sistem sahibi, Yaprak Kolektifi yönetici, diğer hesaplar üyedir. Hesap adı ve yetki sağ üstte görünür. Oturum sayfa yenilendiğinde kapanır; rol değişiklikleri tarayıcıda saklanır.

Sistem sahibiyle Backoffice → Kullanıcılar & yetkiler → rol seç → Uygula. Değişiklik işlem geçmişine yazılır. Son sistem sahibi kaldırılamaz; önce başka bir sahip atanmalıdır. Üye veya ziyaretçi doğrudan yönetim URL’si açarsa ziyaretçi görünümüne döner. Eski Vitrinim hesabı değiştirme yolu kaldırıldı; yalnız giriş yapılan kişinin vitrini açılır.

## Sınırlar ve production gereksinimleri

Bu tek HTML içindeki kontroller bir UX/iş kuralı simülasyonudur. Kullanıcı demo hesaplarını seçebilir ve yerel kod/veriyi değiştirebilir; gerçek erişim güvenliği sağlamaz. Gerçek uygulama sunucuda kimlik doğrulaması, her istekte rol ve kaynak sahipliği kontrolü, rol iptali sonrası oturum yetkilerinin yenilenmesi, sunucuda değiştirilemez denetim kaydı ve son sahip değişikliklerinde eşzamanlılık kontrolü gerektirir. Parola, token veya gerçek kullanıcı hesabı eklenmedi.

11 yetki senaryosu Node VM olay/model testleriyle geçti: ziyaretçi görünümü, URL erişimi, engellenen mutasyon, üye görünümü, eski hesap seçme yolunun kapatılması, yönetici sınırı, rol verme/geri alma, son sahip, geçersiz rol, işlem geçmişi ve çıkış. Gerçek tarayıcı doğrulaması yapılmadı.
