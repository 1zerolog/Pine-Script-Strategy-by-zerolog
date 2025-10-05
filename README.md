# 📈 RSI Long/Short Break-Even Point Optimizer Strategy

[![Pine Script](https://img.shields.io/badge/Pine%20Script-v5-blue.svg)](https://www.tradingview.com/pine-script-docs/)
[![Strategy](https://img.shields.io/badge/Type-Trading%20Strategy-green.svg)](https://www.tradingview.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## 🎯 Proje Özeti

Bu proje, RSI (Relative Strength Index) göstergesini kullanarak otomatik long/short pozisyon açan ve break-even point optimizasyonu yapan gelişmiş bir Pine Script stratejisidir. Strateji, trail stop parametrelerini otomatik olarak optimize ederek maksimum kar elde etmeyi hedefler.

## ✨ Özellikler

- 🔄 **RSI Tabanlı Sinyaller**: Overbought/oversold seviyelerinde otomatik giriş
- 📊 **Leverage Desteği**: Özelleştirilebilir kaldıraç oranları
- 🎯 **Trail Stop Optimizasyonu**: Otomatik parametre optimizasyonu
- 📈 **Long/Short Pozisyonlar**: İki yönlü işlem desteği
- 📋 **Gerçek Zamanlı Raporlama**: En iyi parametreleri görsel olarak gösterim
- ⚙️ **Esnek Parametreler**: Tüm ayarlar kullanıcı tarafından özelleştirilebilir

## 🛠️ Teknik Detaylar

### RSI Parametreleri
- **RSI Length**: 9 (varsayılan)
- **Overbought Level**: 68
- **Oversold Level**: 31
- **Source**: Close price

### Optimizasyon Parametreleri
- **Trail Start**: 0.5% - 2.0%
- **Trail End**: 2.0%
- **Trail Step**: 0.1%
- **Offset Start**: 0.02% - 0.1%
- **Offset End**: 0.1%
- **Offset Step**: 0.01%

### Risk Yönetimi
- **Leverage**: 1x (varsayılan, özelleştirilebilir)
- **Position Size**: Equity'nin %100'ü
- **Initial Capital**: $100

## 📁 Dosya Yapısı

```
Pine-Script-Strategy-by-zerolog/
├── README.md                              # Bu dosya
├── RSI_L_S_BEP_Optimizer_Report.pine      # Ana strateji dosyası
└── LICENSE                                # Lisans dosyası (opsiyonel)
```

## 🚀 Kurulum ve Kullanım

### 1. TradingView'da Kullanım
1. TradingView platformuna giriş yapın
2. Pine Editor'ı açın
3. `RSI_L_S_BEP_Optimizer_Report.pine` dosyasının içeriğini kopyalayın
4. Pine Editor'a yapıştırın
5. "Add to Chart" butonuna tıklayın

### 2. Parametre Ayarları
Stratejiyi chart'a ekledikten sonra ayarlar panelinden şu parametreleri özelleştirebilirsiniz:

- **RSI Ayarları**: Length, overbought/oversold seviyeleri
- **Leverage**: Risk seviyenize göre kaldıraç oranı
- **Trail Stop**: Optimizasyon aralıkları
- **Offset**: Stop loss offset değerleri

## 📊 Strateji Mantığı

### Giriş Koşulları
- **Long Pozisyon**: RSI değeri 68'in üzerine çıktığında
- **Short Pozisyon**: RSI değeri 31'in altına düştüğünde

### Çıkış Koşulları
- **Trail Stop**: Dinamik stop loss ile kar koruması
- **Optimizasyon**: En iyi trail stop parametrelerini otomatik bulma

### Performans Takibi
- Gerçek zamanlı kar/zarar hesaplama
- En iyi parametreleri chart üzerinde gösterme
- Break-even point optimizasyonu

## ⚠️ Risk Uyarıları

- Bu strateji eğitim amaçlıdır
- Gerçek para ile işlem yapmadan önce paper trading ile test edin
- Geçmiş performans gelecekteki sonuçları garanti etmez
- Risk yönetimi kurallarına uyun
- Sadece kaybetmeyi göze alabileceğiniz para ile işlem yapın

## 🔧 Geliştirme

### Katkıda Bulunma
1. Bu repository'yi fork edin
2. Yeni bir branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Değişikliklerinizi commit edin (`git commit -m 'Add amazing feature'`)
4. Branch'inizi push edin (`git push origin feature/amazing-feature`)
5. Pull Request oluşturun

### Önerilen İyileştirmeler
- [ ] Daha fazla teknik gösterge desteği
- [ ] Backtest sonuçları analizi
- [ ] Risk yönetimi modülleri
- [ ] Multi-timeframe analiz
- [ ] Alert sistemi entegrasyonu

## 📈 Performans Metrikleri

Strateji aşağıdaki metrikleri takip eder:
- Net Profit
- Win Rate
- Maximum Drawdown
- Sharpe Ratio
- Break-even Point

## 🤝 Destek

Sorularınız veya önerileriniz için:
- GitHub Issues kullanın
- TradingView'da @zerolog profilini takip edin

## 📄 Lisans

Bu proje MIT lisansı altında lisanslanmıştır. Detaylar için [LICENSE](LICENSE) dosyasına bakın.

## 🙏 Teşekkürler

- TradingView Pine Script topluluğu
- Tüm katkıda bulunanlar
- Test eden ve geri bildirim veren kullanıcılar

---

**⚡ Not**: Bu strateji sürekli geliştirilmektedir. En güncel versiyonu için repository'yi takip edin.

**📊 Disclaimer**: Bu yazılım yalnızca eğitim amaçlıdır. Finansal tavsiye niteliği taşımaz. Yatırım kararlarınızı vermeden önce profesyonel finansal danışmanlık alın.
