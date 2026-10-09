# 📍 Gün 02 — Primer Ekipmanlar: Güç Trafoları ve Testleri

## 🎯 Günün Hedefleri

-   [x] Trafo vektör gruplarını (Dyn11, YNd11 vb.) ve saat açısı mantığını kavramak.
-   [x] Saha kabul ve periyodik trafo test yöntemlerini (TTR, İzolasyon, Sargı Direnci) öğrenmek.
-   [x] Trafo mekanik ve elektriksel koruma ekipmanlarını (Buchholz, Hermetik, Termometreler) incelemek.

---

## 📚 Özet Çalışma Notları

### 1. Trafo Bağlantı & Vektör Grupları (Vektör Açısı Mantığı)

Vektör grubu, yüksek gerilim (primer) ve alçak gerilim (sekonder) sargıları arasındaki bağlantı şeklini ve gerilimler arasındaki **faz açısı farkını** ifade eder.

-   **Harf Anlamları:**
    -   **Büyük Harfler (Primer / YG):** `D` = Üçgen (Delta), `Y` = Yıldız (Star), `N` = Nötr Çıkışlı.
    -   **Küçük Harfler (Sekonder / AG veya OG):** `d` = Üçgen, `y` = Yıldız, `z` = Zigzag, `n` = Nötr Çıkışlı.
-   **Saat Sayısı (Faz Açısı):** Her 1 saatlik dilim **30°** faz farkını temsil eder.
    -   **Dyn11:** Primer Üçgen, Sekonder Nötr Çıkarılmış Yıldız. Sekonder gerilimi, Primer geriliminden $11 \times 30^\circ = 330^\circ$ ileridedir (veya $30^\circ$ geridedir). _Dağıtım trafolarında en yaygın yapı._
    -   **YNd11:** Primer Nötr Çıkarılmış Yıldız, Sekonder Üçgen. _Güç iletim trafolarında ve santral çıkış trafolarında yaygındır._

---

### 2. Temel Trafo Testleri & Saha Amacı

| Test Adı                               | Ölçüm Aleti / Cihaz                                              | Saha Amacı & Kabul Kriteri                                                                                                                                       |
| :------------------------------------- | :--------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **TTR (Turn Ratio Test)**              | TTR Test Cihazı                                                  | Primer/Sekonder sarım oranını ve vektör grubunu doğrular. Tolerans genelde $<\%0.5$'dir.                                                                         |
| **İzolasyon Direnci (Megger)**         | Yüksek Gerilim İzolasyon Test Cihazı ($1\text{kV} - 5\text{kV}$) | Sargılar arası ve sargı-gövde yalıtımını ölçer. $R_{10min}/R_{1min}$ oranıyla **PI (Polarizasyon İndeksi)** hesabı yapılır ($PI > 2$ olmalıdır).                 |
| **Sargı Direnci (Winding Resistance)** | Mikroohmmetre / Sargı Direnç Cihazı                              | Sargılardaki iletken kopukluklarını, gevşek bağlantıları ve Kademe Değiştirici (Tap Changer) kontak kalitesini kontrol eder. Fazlar arası fark $<\%2$ olmalıdır. |

---

### 3. Mekanik Korumalar (Gövde Emniyet Zinciri)

-   **Buchholz Rölesi:** Yağlı trafolarda kazan ile genleşme deposu arasına konulur. Yavaş gaz birikmesinde **İhbar (Alarm)**, ani yağ akışında ve büyük arklarda **Açma (Trip)** verir.
-   **Sıcaklık Röleleri / Termometreler:** Yağ sıcaklığı ($Oil\ Temp$) ve Sargı sıcaklığı ($Winding\ Temp$) ölçer. Çift kademelidir (Alarm & Trip).
-   **Basınç Boşaltma Valfi (PRD):** Kazan içi aşırı basınçta yağın dışarı fışkırmasını sağlayarak patlamayı önler.

---

## 🔗 Detaylı Notlar

Tüm teorik detaylar, hesaplamalar ve saha test adımları için:
👉 **[2. Gün Detaylı Teknik Notları (detail.md)](./detail.md)**
