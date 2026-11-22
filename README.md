# Sensör Verileriyle Turbofan Motor Bozulma Analizi ve Kestirimci Bakım Modellerinin Karşılaştırılması

Bu depo, Makine Öğrenmesi dersi proje ödevi kapsamında **NASA C-MAPSS (Turbofan Engine Degradation Simulation)** veri seti (`FD001` alt kümesi) kullanılarak geliştirilen kestirimci bakım (predictive maintenance) ve arıza sınıflandırma çalışmasını içermektedir.

## 🎯 Projenin Amacı
Turbofan uçak motorlarına ait zaman serisi sensör ve operasyonel ayar verilerini analiz ederek motorların **Kalan Faydalı Ömür (RUL - Remaining Useful Life)** değerine dayalı arıza riskini erken aşamada sınıflandırmak, farklı klasik makine öğrenmesi algoritmalarının performanslarını karşılaştırmak ve model kararlarını Açıklanabilir Yapay Zeka (XAI) yöntemleriyle yorumlamaktır.

## 📊 Veri Seti Bilgisi
Ödev yönergesi gereği ham veri seti dosyaları bu depoya yüklenmemiştir. Çalışmada kullanılan **C-MAPSS (`FD001`)** veri setine aşağıdaki kaynaklardan erişilebilir:
* **NASA Resmi Veri Deposu:** [NASA PCoE Data Set Repository (6. Turbofan Engine Degradation Simulation)](https://www.nasa.gov/intelligent-systems-division/discovery-and-systems-health/pcoe/pcoe-data-set-repository/)

> **Not:** Çalışmayı yerel ortamda çalıştırmak için NASA bağlantısından indirilen `train_FD001.txt` (ve gerekirse `test_FD001.txt`, `RUL_FD001.txt`) dosyalarını yerel çalışma dizininizdeki `data/` klasörüne yerleştiriniz.

## 📁 Proje Klasör Yapısı
```text
├── notebooks/          # Açıklamalı Jupyter Notebook analiz ve modelleme dosyaları
├── reports/            # Proje raporu taslağı ve grafik çıktıları
├── src/                # İsteğe bağlı yardımcı Python modülleri
├── requirements.txt    # Gerekli Python kütüphaneleri
├── .gitignore          # Veri dosyaları ve geçici dosyaları hariç tutma kuralları
└── README.md           # Proje dokümantasyonu
```

## 👥 Proje Ekibi
* Nigar Abdullayeva — B231210561
* Rafig Abdullayev — B231210566
* Gulnur Naghiyeva — B231210584

## ⚙️ Kurulum ve Çalıştırma
Notebook çıktıları kayıtlı olsa da kodu kendi ortamınızda sıfırdan çalıştırmak için önce gerekli paketleri kurunuz:

```bash
pip install -r requirements.txt
