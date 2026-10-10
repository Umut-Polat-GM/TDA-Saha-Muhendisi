# 📖 Gün 03 — Kesiciler, Ark Söndürme ve Ölçü Trafoları (Teknik Detaylar)

Bu dökümanda OG/YG kesicilerinin ark söndürme mekanizmaları, CRM ve zamanlama testlerinin kabul kriterleri ile Akım Trafolarında doyum ve polarite kavramları detaylandırılmıştır.

---

## 1. Kesici Teknolojileri ve Ark Söndürme Prensipleri

Kesicilerin temel görevi, nominal yük akımlarını ve sistemdeki kısa devre akımlarını güvenle kesmektir. Kontak ayrılması anında kaçınılmaz olarak bir elektrik arkı oluşur. Bu arkın söndürülme yöntemi kesici tipini belirler.

### 1.1. Vakum Kesiciler (Vacuum Circuit Breakers - VCB)

-   **Kullanım Alanı:** Genellikle Orta Gerilim ($1\text{ kV} - 36\text{ kV}$) şebekelerinde ve panolarda tercih edilir.
-   **Çalışma Prensibi:** Kontak kapalıyken akım vakum tüpü içinden akar. Kontak açıldığında aradaki metal buharı arkı besler, ancak yüksek vakum ortamı ($10^{-6}\text{ torr}$) sayesinde metal buharı hızla çevre duvarlara yoğuşur ve ilk akım sıfır ($0$) noktasında ark kalıcı olarak söner.

### 1.2. $\text{SF}_6$ Gazlı Kesiciler

-   **Kullanım Alanı:** Yüksek Gerilim ($36\text{ kV}$ üstü) açık şalt sahalarında ve GIS sistemlerinde kullanılır.
-   **Çalışma Prensibi:** $\text{SF}_6$ gazı yüksek elektronegatifliğe sahiptir; serbest elektronları yakalayarak negatif iyonlara dönüşür ve arkın iletkenliğini hızla düşürerek arkı söndürür.

![Image](./assets/Circuit%20Breaker.webp)

---

## 2. Kesici Saha Testleri

### 2.1. Kontakt Direnci Testi (CRM - Contact Resistance Measurement)

-   **Amaç:** Kesici kapalı pozisyondayken ana kontakların temas direncini ölçmek. Yüksek geçiş direnci $I^2R$ kayıplarından ötürü kontaklarda aşırı ısınmaya ve erimeye yol açar.
-   **Uygulama:** Genellikle $100\text{A}$ veya $200\text{A}$ DC akım enjekte edilerek milivolt düşümü ölçülür.
-   **Kabul Kriteri:** Üretici katalog değerlerine uygun olarak genelde **mikro-ohm ($\mu\Omega$)** seviyelerinde olmalıdır.

### 2.2. Zamanlama (Timing) Testi

-   **Amaç:** Kesicinin açma ve kapama komutunu almasından kontakların fiziksel olarak ayrılmasına/birleşmesine kadar geçen sürenin milisaniye ($ms$) cinsinden ölçülmesidir. Ayrıca 3 fazın aynı anda (eşzamanlı) çalışıp çalışmadığını kontrol eder.
-   **Kabul Kriteri:** Fazlar arası zaman senkronizasyon kayması üretici sınırları dahilinde (genellikle $< 2-3\text{ ms}$) olmalıdır.

---

## 3. Akım Trafoları (CT) ve Kritik Parametreler

### 3.1. Akım Trafosu Doyumu (Saturation)

Kısa devre anında arıza akımı çok yüksek seviyelere ulaştığında, CT'nin demir çekirdeği manyetik olarak doyuma (saturation) ulaşır. Doyuma ulaşan bir CT, primerden ne kadar yüksek akım geçerse geçsin sekondere doğru orantılı akım aktaramaz (akım kırpılır). Bu durum, koruma rölelerinin arızayı algılayamamasına ve gecikmesine neden olabilir.

### 3.2. Knee-Point (Diz Noktası) Gerilimi

CT'nin lineer (doğrusal) çalışma bölgesinden doyum bölgesine geçtiği kritik eşiktir.

-   **Tanım:** Gerilimde **%10'luk bir artış**, magnetizasyon akımında **%50'lik bir artışa** neden oluyorsa o nokta diz noktasıdır. Koruma sınıfı CT'lerde (örneğin 5P20) diz noktası geriliminin yüksek olması istenir.

### 3.3. Polarite Testi ve Önemi

-   **Neden Önemlidir?** CT'lerin primer giriş ($P1$) ve sekonder çıkış ($S1$) uçlarının yönü vardır. Özellikle **Diferansiel Koruma** ve yönlü koruma rölelerinde faz açısı hayati önem taşır. Yanlış polarite bağlantısı, normal işletme şartlarında bile koruma rölesinin sistemi hatalı bir şekilde açmasına (False Trip) yol açar.
