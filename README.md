# 🚗 STM32 Tabanlı Akıllı Araç (SmartCar)

STM32 mikrodenetleyici ile geliştirilen bu **akıllı araç projesi**, manuel ve otomatik kontrol modları, sensör destekli karar mekanizmaları ve IoT uyumlu haberleşme özellikleriyle donatılmıştır. Proje; gömülü sistemler, GPS ile yön bulma, engelden kaçınma ve kablosuz kontrol sistemlerini bir araya getirerek kapsamlı bir mühendislik çözümü sunar.

---

## 🔧 Özellikler

- 🚙 **Yön Kontrolü**  
  Temel hareket komutları ile manuel sürüş:  
  `ile`, `ger`, `sol`, `sag`, `dur`, `gnd`, `gnb`, `kyd`, `kyb`

- 🧭 **Otomatik Mod**  
  Sensör verilerine göre çevredeki engelleri algılayarak yön değiştirme ve durma.

- 🧱 **Engel Algılama**  
  Kızılötesi sensör ile engel algılama ve otomatik durma.

- 📡 **Kablosuz Kontrol**  
  UART üzerinden gelen metin tabanlı komutlarla yön kontrolü (Bluetooth modülü).

- 🧠 **Durum Makinesi (State Machine)**  
  GPS Verilerinden Gelen veriler işlenir ve göre önceden tanımlanmış hareket senaryoları uygulanır.

- 📊 **UART Debug ve İzleme**  
  Seri monitör ile veri izleme ve hata ayıklama desteği.

- 🌐 **IoT ve GPS Entegrasyonu**  
  - GPS modülünden alınan konumlar WiFi üzerinden IoT bulut ortamına gönderilir.  
  - Araç, hedef konuma/konumlara yaklaşık **2.5 metre hassasiyetle** yönelir.  
  - Buluttan gelen hedef koordinatına göre karar verme.

---

## 📦 Donanım Gereksinimleri

- STM32 Geliştirme Kartı (Örn: Nucleo-F429ZI)
- L293D  Motor Sürücü
- 4x 6V DC Motor + Tekerlekler
- HC-05 Bluetooth Modülü
- ESP8266 WiFi Modülü
- NEO-8M GPS Modülü
- Kızılötesi Engel Algılama Sensörü (MZ 80)
- 30000 mah Batarya / Powerbank
- Voltaj regülatörlerü(x2)
---

## 🧪 Komut Listesi

| Komut   | Açıklama              |
|---------|------------------------|
| `ile`   | İleri git              |
| `ger`   | Geri git               |
| `soll`  | Sola dön               |
| `sag`   | Sağa dön               |
| `dur`   | Dur                    |
| `gdogu` | Güneydoğu yönünde git |
| `gbati` | Güneybatı yönünde git |
| `kdogu` | Kuzeydoğu yönünde git |
| `kbati` | Kuzeybatı yönünde git |

---

## 📷 Görseller

> ![20250519_155545](https://github.com/user-attachments/assets/0c5c14c4-b15d-47e1-9ff1-af773716685f)

![20250519_155448](https://github.com/user-attachments/assets/3939bd2f-5b94-4849-994d-abd2171b44f6)

---

## 👨‍💻 Geliştirici Notları

Bu proje gömülü sistemler, robotik kontrol ve IoT alanında eğitim ve geliştirme amaçlıdır. Kod yapısı modüler ve genişletilebilir olacak şekilde tasarlanmıştır. Katkılarınız ve geri bildirimleriniz memnuniyetle karşılanır!

