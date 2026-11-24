# 📍 Gün 15 — Fider Devreye Alma: Komisyonlama Akışı ve Dokümantasyon

## 🎯 Günün Hedefleri

-   [x] Fider komisyonlama sürecinin adım adım akışını kavramak.
-   [x] Ayar dosyası yükleme ve doğrulama prosedürünü uygulamak.
-   [x] Devreye alma kontrol listesi (checklist) hazırlamak.
-   [x] Test dossier yapısını ve imza akışını öğrenmek.
-   [x] Devreye alma öncesi ölçülebilir kabul kriterleri ve müşteri ön koşullarını netleştirmek.

---

## 📚 Özet Çalışma Notları

### 1. Komisyonlama Adımları (Sıra Kritik!)

1.  **Kurulum ve görsel kontrol** — mekanik montaj, etiketler, kapaklar.
2.  **Sekonder kablo testleri** — süreklilik, izolasyon, bağlantı doğruluğu.
3.  **CT/VT testleri** — oran, polarite, burden.
4.  **IED ayar yükleme** — setting file + doğrulama (readback).
5.  **Sekonder enjeksiyon** — koruma fonksiyonlarının testi.
6.  **Interlock ve kumanda testleri** — tüm manevra senaryoları.
7.  **SCADA point testleri** — her sinyal tek tek.
8.  **Enerjileme ve faz kontrolü** — faz sırası, faz-faz gerilim.
9.  **Yük altında ölçüm doğrulama** — CT/VT yönleri, faz açıları.

### 2. Ayar Yönetimi

-   **Ayar dosyası hash'i** hesaplanır ve saklanır (yüklenen dosyanın birebir doğrulanması).
-   **4-göz prensibi:** Hesaplayan ve kontrol eden farklı kişiler.
-   **Versiyon kontrol:** Her değişiklik revizyon numarası ile kaydedilir.

### 3. Test Dossier Yapısı

```
📁 Test Dossier — Fider F1
 ├── 01_Proje Dokümanları (schematic, ayar listesi)
 ├── 02_Ekipman Sertifikaları (FAT raporları)
 ├── 03_Cihaz Kalibrasyon Sertifikaları
 ├── 04_Test Prosedürleri ve Kabul Kriterleri
 ├── 05_Ölçüm Sonuçları (ham veri)
 ├── 06_Interlock ve Kumanda Test Raporu
 ├── 07_SCADA Point Test Raporu
 ├── 08_Enerjileme Kayıtları (manevra fişi)
 └── 09_İmza ve Onay Sayfası
```

---

![Fider Koruma Ayarları](./assets/fider-koruma-ayarlari.svg)

## 🔗 Detaylı Notlar

Her adımın detaylı kontrol listesi ve tipik hata senaryoları için:
👉 **[15. Gün Detaylı Teknik Notları (detail.md)](./detail.md)**


---

### 📋 Devreye Alma Öncesi Kabul ve Hazırlık Mutabakatı
Test başlamadan önce müşteri, TDA/yüklenici ekibi ve işletme temsilcisi; kriterleri, ön koşulları, kanıtları ve kabulü imzalayacak yetkiliyi yazılı olarak netleştirmelidir. Limitler evrensel kabul edilmemeli; sözleşme, onaylı proje dokümanı, üretici talimatı ve uygulanabilir standarttan alınmalıdır.

| Mutabakat başlığı | Önceden belirlenmesi gerekenler |
| :--- | :--- |
| Teknik kabul kriteri | Ekipman/işlev, test yöntemi, beklenen değer ve tolerans; referans dokümanın adı/revizyonu |
| Süre ve takvim | Test penceresi, tahmini test süresi, tekrar test için plan ve gecikme varsayımları |
| Müşteri hazırlıkları | Enerji ve yardımcı beslemeler, saha erişimi, çalışma izinleri, operatör; gerekiyorsa yük/proses koşulları |
| Kaynaklar | Kalibrasyonu geçerli test cihazı, gerekli personel, yardımcı malzeme ve iletişim düzeni |
| Kanıtlar | Ham ölçüm, imzalı test raporu, olay kayıtları, eğitim ve teslim kayıtları, revizyon bilgisi |
| Yetki ve imza | Testi yapan, tanık olan, teknik değerlendiren ve kabulü imzalayacak isim/rol |
| Sapma yönetimi | PASS/FAIL/şartlı kabul tanımı, açık uygunsuzluk sahibi, düzeltme ve tekrar test onayı |

> **KPI notu:** Çevrim süresi ve ilk geçiş oranı gibi ölçütler yalnızca proje kapsamına uyuyorsa sözleşmede tanımlanmalıdır. Bunlar ekipman kabul testlerinin yerine geçmez. Ölçüm yöntemi, başlangıç/bitiş noktası, örneklem ve istisnalar da tanımlanmalıdır.

Örnek kabul satırı ve doldurulabilir proje matrisi için [detaylı teknik notlara](./detail.md#11-devreye-alma-oncesi-kabul-ve-hazirlik-matrisi) bakın.

### 4. Detaylı Notlar
Her adımın kontrol listesi, kabul matrisi ve tipik hata senaryoları için:
👉 **[15. Gün Detaylı Teknik Notları (detail.md)](./detail.md)**
