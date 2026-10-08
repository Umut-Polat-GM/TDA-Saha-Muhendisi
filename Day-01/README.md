# 📍 Gün 01 — Şalt Mimarisi, Tek Hat Şemaları (SLD) ve Manevra Sıralaması

## 🎯 Günün Hedefleri

-   [x] OG ve YG Şalt sahası tiplerini (AIS / GIS) kavramak.
-   [x] Bir fideri oluşturan temel bileşenleri ve yerleşim sırasını öğrenmek.
-   [x] Elektriksel ve mekanik kilitleme (Interlock) mantığını analiz etmek.
-   [x] Fider devreye alma ve devreden çıkarma manevra adımlarını simüle etmek.

---

## 📚 Araştırma & Çalışma Notları

### 1. AIS ve GIS Şalt Sahaları

-   **AIS (Air Insulated Switchgear):** Yalıtım ortamı havadır. Geniş alan gerektirir, bakımı ve görsel kontrolü kolaydır.
-   **GIS (Gas Insulated Switchgear):** Yalıtım ortama SF6 gazıdır. Çok daha kompakt alan kaplar, çevresel faktörlerden etkilenmez.

### 2. Bir Fiderin Yapısal Dizilimi

Bara'dan hatta doğru ekipman sıralaması:
`Bara ➔ Bara Ayırıcısı ➔ Kesici ➔ Akım Trafosu ➔ Gerilim Trafosu ➔ Hat Ayırıcısı ➔ Toprak Bıçağı`

---

## 🛠️ Günün Görevi & Çıktısı: Manevra Sıralaması

> ⚠️ **Altın Kural:** Yük altında (akım geçerken) ayırıcı açılıp kapatılmaz! Bütün açma/kapama operasyonlarında yükü kesecek eleman **Kesici**'dir.

### 🟢 Fider Devreye Alma Adımları (Enerjilendirme)

1. Toprak Bıçağı **Açılır**.
2. Hat Ayırıcısı **Kapatılır**.
3. Bara Ayırıcısı **Kapatılır**.
4. Kesici **Kapatılır** (Fidere enerji verilir).

### 🔴 Fider Devreden Çıkarma Adımları (İzolasyon)

1. Kesici **Açılır** (Akım kesilir).
2. Bara Ayırıcısı **Açılır**.
3. Hat Ayırıcısı **Açılır**.
4. Toprak Bıçağı **Kapatılır** (Hattın kalıntı yükü topraklanır).

---

![Tek Hat Şeması](./assets/Tek_Hat_Seması01.jfif)

## 🔗 İlgili Kaynaklar & Dokümanlar

-   _IEC 62271 Standardı — Yüksek Gerilim Şalt Tesisleri_
-   [LinkedIn Post Linki](https://linkedin.com/...)
