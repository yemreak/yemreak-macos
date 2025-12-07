# Değişiklik Günlüğü

> [English](CHANGELOG-en.md)

## [0.4.3] - 2025-12-07

### Değişiklikler
- **Kısayol değişimi**: `⌥A` = Sadece ses (insan), `⌥⇧A` = Clipboard destekli (AI)
- **Okunabilir çıktı**: Clipboard referansları `[1:App]` formatında footer ile gösteriliyor
- **Tam Türkçe arayüz**: Menu bar, paneller, alertler ve tüm UI Türkçe

### İyileştirmeler
- `dictation.getEntries` yanıtında meta bilgisi (count, limit) eklendi
- Whisper halüsinasyon filtresi geliştirildi ("Altyazı M.K.", "Subscribe" vb.)
- Clipboard göstergesi her iki modda da görünüyor
- Uzun clipboard önizlemeleri için scroll desteği (VS Code tarzı)
- Whisper kelimeler arası çift boşluk düzeltildi
- Snippet'lar artık markdown formatında
- About paneli: "Sesli Clipboard Yöneticisi" alt başlığı
- About paneli: Tarih bilgisi artık doğru gösteriliyor

### Geliştirici (Beta)
- **Sesli Snippet Önerileri**: Kayıt sırasında anahtar kelime söyle, snippet önerileri al

---

## [0.4.2] - 2025-12-07

### İyileştirmeler
- Event-driven chunk tamamlama (polling yerine daha hızlı yanıt)
- Thread-safe context key okuma (AtomicContextKeys)
- Lisans paneli input alanı genişletildi (340px)
- Sparkle versiyon formatı semantic olarak değişti (402, 403...)

### Düzeltmeler
- "Güncellemeleri Kontrol Et" artık yeni versiyonları doğru algılıyor
- ESC tuşu kayıt sırasında düzgün tüketiliyor
- Kayıt durumu tek kaynaktan senkronize ediliyor

---

## [0.4.1] - 2025-12-06

### Yeni Özellikler
- **Caps Lock Hyper Tuşu**: Caps Lock'u modifier olarak kullan (Caps+A, Caps+B, vb.)
- **HTTP Toplu İstekler**: Agent dostu API, sadece array formatı
- **Dikte Kısayolları**: Dil (Otomatik/İngilizce/Türkçe) ve model (Hızlı/Doğru) değiştirmek için kısayol ata

### İyileştirmeler
- Kısayol paneli varsayılan olarak "Tümü" filtresiyle açılıyor
- Özel karakterler için genişletilmiş klavye eşlemeleri
- ESC kayıt yapmıyorken kısayol panelini kapatıyor
- Adaptif clipboard yoklama (kayıtta 100ms, beklemede 500ms)
- "Sorun Bildir..." menü öğesi eklendi
- "Logları Aç" Araçlar menüsüne taşındı

### Düzeltmeler
- Kısayol kaydı ve çakışma tespiti düzeltildi
- Kendi yapıştırman artık clipboard geçmişine kaydedilmiyor
- ESC transkripsiyonu iptal ediyor ve clipboard toast'larını temizliyor
- Model değişimi kayıt/transkripsiyon sırasında engelleniyor
- Takılma ipucu pipeline üzerinde örtüşmeden gösteriliyor
- ESC kısayol kaydı sırasında tüketiliyor

---

## [0.4.0] - 2025-12-05

### Transkripsiyon Artık Işık Hızında
- İstediğin kadar kayıt yap - transkripsiyon arka planda oluyor
- Kaydı durdurduktan sonra bekleme yok
- Eskisinden %70 daha hızlı
- Otomatik sessizlik kaldırma ile temiz sonuçlar

### Yeni Özellikler
- **Dikte** `Option+Shift+A`: Sesten metne, doğrudan yapıştır
- **Clipboard Modu** `Option+A`: Kopyaladıklarını AI sohbetleri için transkripsiyona dahil et
- **Clipboard Yığını**: Kayıt sırasında kopyaladıklarını gör, önizlemek için üzerine gel
- **Dil Seçimi**: Transkripsiyon dilini menüden seç
- **Model Seçimi**: Doğru veya Hızlı transkripsiyon arasında seç
- **Sessizlik Hassasiyeti**: Kaydın duraklamalara ne kadar duyarlı olduğunu ayarla
- **Oturum Takibi**: Bilgisayar başında ne kadar süredir olduğunu gör
- **Hareketsizlik Uyarıları**: Çok uzun süre hareketsiz kaldığında hatırlat (15dk-2sa)
- **Uyku Algılama**: Gece molalarından sonra otomatik sıfırlanır
- **Oturum Bildirimleri**: Zaman kilometre taşlarına ulaştığında bil
- **XDR Parlaklık**: Ekranı normal limitin ötesine it
- **Klavye Temizleyici**: Silmek için klavyeni kilitle
- **Kısayol Paneli**: Tüm kısayolları tek yerden gör ve özelleştir
- **Güvenli API Anahtarları**: Anahtarların macOS Keychain'de güvenle saklanıyor
- **Çökme Raporlama**: Bir şey bozulduğunda düzeltebilmemiz için biliyoruz

### Daha İyi Deneyim
- Transkripsiyon sırasında uygulama donmuyor
- Kısayollar anında yanıt veriyor
- İzinler sadece gerektiğinde soruluyor
- Transkripsiyon ilerlemesini gör: REC -> Kaydedildi -> % -> Yapıştırıldı
- Takıldın mı? 3 saniye sonra ipucu görünüyor
- Clipboard öğelerini geçmişte satır içi gör
- Yepyeni ikon

### Menü ve Ayarlar
- "Güncellemeleri Kontrol Et..." artık üst seviyede
- Hakkında panelinde otomatik güncelleme düğmesi
- Geliştirici seçenekleri olmadan temiz menü
- Hakkında panelinde GitHub bağlantıları

### Düzeltmeler
- ESC tuşu artık her yerde çalışıyor
- Ok tuşları aramada çalışıyor
- Durdurduğunda ses temiz şekilde duruyor
- Oturum süresi yeniden başlatmalar arasında kaydediliyor

### Ekran Görüntüleri

![Kayıt](images/v0.4.0/recording.png)
![Dikte Geçmişi](images/v0.4.0/dictation-history.png)
![Oturum](images/v0.4.0/session.png)
![Ekran Menüsü](images/v0.4.0/display-menu.png)
![Araçlar](images/v0.4.0/tools.png)
![Klavye Temizleyici](images/v0.4.0/keyboard-cleaner-panel.png)
![Hakkında](images/v0.4.0/about.png)

---

## [0.3.0] - 2025-11-28

### Yeni Özellikler
- F1/F2 ile ekran parlaklığını kontrol et
- Dahili ekranı kapat
- Transkripsiyon geçmişinde ara

---

## [0.2.0] - 2025-11-26

### İlk Sürüm
- Sesten metne
- Global kısayollar
- Menü çubuğu arayüzü
- Otomatik güncellemeler
