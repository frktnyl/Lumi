# Technical Outline

## Teknik Hedef

Lumi, masaustunde seffaf bir pencere uzerinde calisan, kullanici etkilesimlerine tepki veren hafif bir desktop companion uygulamasi olmalidir. Teknik kararlar performans, stabilite ve kullanicinin kontrol hissi etrafinda alinmalidir.

## Ilk Platform

- Windows
- Java mevcut proje baslangici
- Desktop UI icin JavaFX veya alternatif desktop framework degerlendirilecek

## Temel Teknik Bilesenler

### Desktop Overlay

- Seffaf pencere
- Always-on-top mod
- Kenarliksiz pencere
- Tiklanabilir veya tiklamayi alttaki pencereye gecirebilir modlar
- Coklu monitor destegi icin hazir tasarim

### Character Runtime

- Animasyon state machine
- Hareket sistemi
- Idle davranis secici
- Mouse yakinlik algisi
- Ekran/pencere kenari algisi
- Davranis yogunlugu ayari

### State System

- Mutluluk
- Enerji
- Aclik
- Temizlik
- Arkadaslik seviyesi
- Gunluk aktivite kaydi

### UI Control Center

- Ana durum paneli
- Ayarlar
- Pet odasi
- Ozellestirme
- Aktiviteler
- Magaza/kozmetik listeleme

### Persistence

- Kullanici ayarlari
- Karakter durumu
- Acilan animasyonlar
- Kozmetik secimleri
- Gunluk ozet verileri

## Teknik Riskler

- Transparent always-on-top pencerenin farkli Windows surumlerinde tutarli calismasi
- Mouse ve pencere etkilesimlerinin kullaniciyi rahatsiz etmemesi
- Dusuk performans hedefinin korunmasi
- Antivirus veya Windows izinleriyle uyumluluk
- Steam paketleme sureci

## Erken Teknik Karar Noktalari

- JavaFX mi, baska framework mu?
- Karakter 2D sprite animasyonu mu, iskelet animasyon mu?
- Pencere algisi native API ile mi, sinirli MVP kurallariyla mi?
- Ilk surumde browser sekmesi algisi gercekten gerekli mi, yoksa pencere ustu illuzyonu yeterli mi?

## Performans Hedefleri

- Idle durumda dusuk CPU kullanimi
- Hafif bellek kullanimi
- Uzun sure acik kaldiginda bellek sizintisi olmamasi
- Animasyonlarin takilmadan calismasi

