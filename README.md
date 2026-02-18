# 📖 Ramazan ve Yıllık Hatim Dağıtım Sistemi (v2)

Bu depo, Ramazan için günlük ve yıl boyunca haftalık Kur'an-ı Kerim okuma programları ile genel döngüsel okuma planları üretmek için geliştirilmiş, bağımlılıksız (vanilla) HTML tabanlı bir araçtır.

## 🌙 Özellikler

### `index.html` (Ramazan + Yıllık Hatim)
- 📅 **Ramazan Günlük Program**: 30 gün boyunca her gün bir cüz takibi
- 📆 **Yıllık Haftalık Program**: 46 haftalık döngü
- 🎯 **Farklı Başlangıç Cüzleri**: Her kişi farklı cüzden başlayabilir
- 🔎 **Tek Cüz Gösterimi**: Sadece seçilen cüz için çıktı üretimi
- 🔄 **İkisini Birlikte Getir**: Seçilen cüz için Ramazan ve yıllık programı tek sayfada yan yana üretim
- 🖨️ **Yazdırma**: A4 yatay yazdırma için optimize düzen
- 🔔 **Bildirimler**: Başarı/hata için toast bildirimler

### `program.html` (Genel Program Oluşturucu)
- 🧩 **Esnek Program Üretimi**: Kur'an hatimleri ve dönüşümlü kitap okumaları için parametreli üretim
- 👥 **Toplu ve Tekli Çıktı**: Tüm kişi listesi veya sadece seçilen kişi
- 🏷️ **Opsiyonel Etiketler**: Sağ sütun başlığı (Bölüm/Cüz), alt başlık
- 📝 **Opsiyonel İsimlendirme**: Bölüm adları ve kişi adları desteği
- 📄 **Sayfa Düzeni Kontrolü**: Sayfa başına kolon sayısı ayarı (maksimum 10)
- 🧷 **Tekli Çıktı Stabilitesi**: Tekli görünümde kolon yerleşimi sayfa ayarıyla tutarlı
- **Tarih sütunu boyutlandırma**: Bölüm kısmına sayı dışında değer yazılması durumunda esneklik

## 🚀 Kullanım

### Online
- Ana sayfa: [https://mn-su.github.io/hatim-dagitim](https://mn-su.github.io/hatim-dagitim)
- Genel oluşturucu: [https://mn-su.github.io/hatim-dagitim/program.html](https://mn-su.github.io/hatim-dagitim/program.html)

### Yerel
- `index.html` dosyasını açın (Ramazan + yıllık hatim)
- `program.html` dosyasını açın (genel program oluşturucu)

## 📋 Nasıl Çalışır?

### `index.html`
1. Ramazan veya yıllık başlangıç tarihini seçin.
2. `Liste Oluştur` butonuyla programı üretin.
3. (Opsiyonel) `Cüz Numarası` girip:
   - `Sadece Bu Cüzü Göster` ile tek cüz görünümü alın
   - `İkisini Birlikte Getir` ile Ramazan + yıllık planı tek sayfada birlikte alın
4. `Yazdır` ile PDF/kağıt çıktısı alın.

### `program.html`
1. Zorunlu alanları doldurun:
   - Program Başlığı
   - Başlangıç Tarihi
   - Toplam Bölüm/Cüz Sayısı
   - Toplam Satır (Dönem) Sayısı
   - Periyot (Gün)
   - Toplam Kişi Sayısı
   - Sayfa Başına Kolon
   - Tekli Çıktı Kolon No
2. İsteğe bağlı olarak bölüm adları ve kişi adları girin.
3. `Toplu Program Oluştur` veya `Tekli Program Oluştur` ile çıktıyı alın.
4. `Yazdır` ile çıktı alın.

## 🆕 v2 Güncellemeleri
- Hadis/bilgi kutusu ile üst panel tasarım iyileştirmesi
- Toast bildirim altyapısı (`showNotification`)
- Tek cüz gösterim akışının iyileştirilmesi (`showSingleCuz`)
- Birlikte görünüm üretimi (`showBothCuz`, `renderBothPrograms`)
- `program.html` ile genel amaçlı program üretim ekranı
- Kişi adı ve bölüm adı tabanlı özelleştirme
- Kolon sayısı doğrulamaları ve yazdırma düzeni iyileştirmeleri

## 🛠️ Teknik Detaylar
- Vanilla HTML/CSS/JS
- Ek bağımlılık yok
- Modern tarayıcı desteği
- `@media print` ile yazdırma optimizasyonu

## 📊 Kullanım Senaryoları
- Cami/kurumlarda toplu hatim ve dönüşümlü okuma planlama
- Bireysel Ramazan ve yıllık takip
- Farklı kitaplar için çok kişili, döngüsel okuma planları

## 🤝 Katkıda Bulunma
1. Fork edin
2. Yeni branch açın: `git checkout -b feature/YeniOzellik`
3. Değişiklikleri commit edin
4. Branch'i push edin
5. Pull request açın

---

## 🌍 English (Short)

A lightweight vanilla HTML tool for:
- Daily Ramadan juz schedule
- Weekly annual Quran schedule
- Flexible multi-person rotation builder (`program.html`)

Includes print-ready A4 layout, single/collective views, optional custom section/person names, and form validations.


---

Made with ❤️ — katkılarınız ve geliştirmeleriniz için teşekkürler.


