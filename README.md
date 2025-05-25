#  Web Tabanlı Veri Toplama ve Fiyat Karşılaştırma Aracı

##  Proje Amacı

Bu projenin amacı, çevrimiçi alışveriş platformlarında aynı ürünün birden fazla satıcı tarafından sunulduğu durumları analiz ederek fiyat, satıcı bilgisi, kargo gibi kriterlere göre karşılaştırma yapabilen bir Python tabanlı araç geliştirmektir.

Proje kapsamında web kazıma, veri temizleme, CSV ile veri kaydetme ve temel analiz işlemleri gerçekleştirilmiştir.

---

## Kullanılan Platformlar

- [Trendyol](https://www.trendyol.com)
- [Hepsiburada](https://www.hepsiburada.com)
- [N11](https://www.n11.com)

---

##  Kullanılan Teknolojiler ve Kütüphaneler

- Python 3.10
- `requests` – HTTP istekleri gönderme
- `BeautifulSoup` – HTML parse etme
- `pandas` – Veri analizi ve CSV işlemleri
- `re` – Regex ile metin işleme
- `time` – Sayfa istekleri arası bekleme süresi

>  **Neden BeautifulSoup?**  
> Sayfa yapısını hızlı ve pratik bir şekilde ayrıştırması, selenium gibi ağır çözümlere ihtiyaç bırakmaması nedeniyle tercih edilmiştir.

---

##  Proje Dosya Yapısı
Web-Tabanli-Veri-Toplama-Araci/
│
├── trendyol_scraper.py # Trendyol ürün verilerini çeker
├── hepsiburada_scraper.py # Hepsiburada ürün verilerini çeker
├── n11_scraper.py # N11 ürün verilerini çeker
├── analyze_data.py # CSV verisini analiz eder
├── output.csv # Tüm platformlardan toplanan ürün verileri
└── README.md # Teknik rapor ve proje açıklaması

---

##  Proje Özeti

- Kullanıcıdan ürün linki alınır veya ürün adı girilir.
- Seçilen web sitesi için scraper çalıştırılır.
- Satıcılar listelenir, fiyat, puan, kargo bilgileri toplanır.
- Veriler `output.csv` dosyasına kaydedilir.
- `analyze_data.py` dosyası ile en ucuz ve en pahalı ürünler belirlenir.

---

##  Veri Analizi Örneği (`analyze_data.py`)

`output.csv` dosyasındaki ürün verileri işlenir. Ardından:

- En **ucuz 5 ürün**
- En **pahalı 5 ürün**

fiyat sıralamasına göre yazdırılır.

### Örnek Çıktı:

En Ucuz 5 Ürün:

Ürün A - 189.99 TL

Ürün B - 210.00 TL

Ürün C - 239.00 TL
...

En Pahalı 5 Ürün:

Ürün X - 9999.00 TL

Ürün Y - 8599.00 TL

Ürün Z - 7200.00 TL
...
---

##  Teslim Kriterlerine Uyum

| Teslim Maddesi                                                    | Durum |
|-------------------------------------------------------------------|-------|
| Belirlenen sitelerden veri kazıma                                 | ✅     |
| Ürün adı, fiyat, satıcı gibi temel bilgilerin çıkarılması         | ✅     |
| Verilerin CSV formatında kaydedilmesi                             | ✅     |
| En ucuz/en pahalı ürünleri gösteren analiz                        | ✅     |
| Teknik açıklama ve proje dökümantasyonu                           | ✅     |

---

##  Zorluklar ve Çözüm Önerileri

- **JavaScript ile yüklenen içerikler:** Sayfalar dinamik olduğundan, doğrudan HTML yerine bazı durumlarda API uç noktaları veya JSON yanıtları analiz edilmiştir.
- **Eksik veri sorunları:** Hataları önlemek için `try-except` blokları kullanılmıştır.
- **Farklı sayfa yapıları:** Her site için özel scraper yazılmıştır.

---

##  Gelecek Geliştirme Önerileri

- Selenium veya Playwright gibi araçlarla JavaScript destekli sayfalara daha etkin erişim
- Basit bir arayüz (GUI) ile kullanıcıdan ürün linki alma sürecini kolaylaştırma
- Kargo süresi, yorum sayısı, ürün açıklamaları gibi ek alanların kazınması
- Satıcı puanı ve yorum sayısına göre sıralama yapma

---

##  Geliştirici

**Fatma Ayben Coşkun**  
Çankırı Karatekin Üniversitesi – İstatistik (1. Sınıf)  
linkedIn: www.linkedin.com/in/ayben-coskun-95337b33b


