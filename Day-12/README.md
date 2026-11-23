# 📍 Gün 12 — Kompakt Şalt (RMU/SF6 Hücre) ve Kabinlerde Çalışma

## 🎯 Günün Hedefleri

-   [x] RMU (Ring Main Unit) mimarisini ve halka şebeke yapısını kavramak.
-   [x] SF6 gazlı kompakt hücrelerin güvenlik zincirini (kapak kilidi, topraklama) öğrenmek.
-   [x] Catu (kapasitif gerilim göstergesi) ile gerilimsizlik kontrolü yapmak.
-   [x] Kablolu hücrelerde test ve devreye alma adımlarını uygulamak.

---

## 📚 Özet Çalışma Notları

### 1. RMU (Ring Main Unit) Mimarisi

Halka şebekelerde (ring main) kullanılan kompakt, SF6 gazlı birimlerdir. Tipik bir RMU'da 3-4 odacık bulunur:

-   **2 adet Ring Switch (Giriş/Çıkış):** Halka bağlantısı, yük anahtarı olarak çalışır.
-   **1 adet Tee-off Fider:** Trafo veya çıkış beslemesi; **sigortalı yük anahtarı (LBS + fuse)** veya **kesicili** olabilir.
-   **Trafo bağlantısı:** Kompakt dağıtım TR'lerinde klasik yapı.

### 2. Güvenlik Zinciri (Interlock)

Kompakt hücrelerde kablolu tip interlock mekanizması:

1.  Hücre **toprak anahtarı KAPALI** değilse kablo bölmesinin kapağı açılmaz.
2.  Kablo bölmesi kapalı değilse kablolar test edilemez.
3.  SF6 gaz basıncı düşükse manevra engellenir (bazı modellerde).

> ⚠️ **Altın Kural:** Kapak kilidi **fiziksel** ve **bağımsızdır** — hiçbir bypass onaylanmaz.

### 3. Catu (Capacitive Voltage Indicator)

Kablolu hücrelerde gerilimsizlik kontrolü **dışarıdan** yapılır:

-   Kablo ekran katmanı ile iletken arasında kapasitif bölüşümle ölçüm alınır.
-   **LED'ler** her faz için yanar (canlı) veya sönük (gerilimsiz).
-   **Test düğmesi (Test / Simulate)** ile göstergenin çalıştığı kanıtlanır.

---

![Kompakt Hücre Emniyet](./assets/kompakt-hucre-emniyet.svg)

## 🔗 Detaylı Notlar

RMU test prosedürleri, SF6 basınç değerleri ve kablolu hücre devreye alma kontrol listesi için:
👉 **[12. Gün Detaylı Teknik Notları (detail.md)](./detail.md)**
