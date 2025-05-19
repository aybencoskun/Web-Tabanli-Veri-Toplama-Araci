# Web Tabanlı Veri Toplama ve Fiyat Karşılaştırma Aracı

Bu proje, Python kullanılarak üç farklı e-ticaret sitesinden (Trendyol, Hepsiburada, N11) ürün verilerini toplayan, analiz eden ve karşılaştıran bir araç geliştirmeyi amaçlar. Proje, web kazıma (web scraping), veri temizleme, analiz ve görselleştirme gibi temel veri bilimi becerilerini kapsar.

##  Proje Özeti
- **Veri Toplama:** Trendyol, Hepsiburada ve N11 sitelerinden ürün verileri toplandı.
- **Veri Birleştirme:** Farklı sitelerden toplanan veriler tek bir veri kümesinde birleştirildi.
- **Veri Analizi:** En ucuz ve en pahalı 5 ürün belirlendi.
- **Veri Görselleştirme:** En ucuz ve en pahalı ürünler için grafikler oluşturuldu.
- **Sonuçlar:** Elde edilen veriler CSV dosyalarına kaydedildi.

##  Proje Klasör Yapısı
```
Web-Tabanli-Veri-Toplama-Araci
├── veriler
│   ├── trendyol.csv
│   ├── hepsiburada.csv
│   ├── n11.csv
│   ├── en_ucuz_5.csv
│   └── en_pahali_5.csv
├── Web_Tabanli_Veri_Toplama_Raporu.pdf
├── iPhone_Karsilastirma_Raporu.pdf
└── README.md
```

##  Nasıl Çalıştırılır?
1. Bu depoyu bilgisayarınıza klonlayın veya ZIP olarak indirin.
2. Gerekli kütüphaneleri yükleyin:
```bash
pip install pandas matplotlib
```
3. Python dosyasını çalıştırın:
```bash
python veri_toplama.py
```

##  Örnek Çıktılar
En ucuz ve en pahalı 5 ürünün grafik çıktıları aşağıda gösterilmiştir:

###  En Ucuz 5 Ürün
![En Ucuz 5 Ürün](veriler/en_ucuz_5.png)

###  En Pahalı 5 Ürün
![En Pahalı 5 Ürün](veriler/en_pahali_5.png)

##  Teknik Raporlar
- **Web Tabanlı Veri Toplama Raporu**: Web_Tabanli_Veri_Toplama_Raporu.pdf
- **iPhone Karşılaştırma Raporu**: iPhone_Karsilastirma_Raporu.pdf
