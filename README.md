# 🎮 Discord Quest Automator

Discord üzerindeki tüm aktif ödüllü görevleri (Quest), uygulamanın dahili Webpack modüllerini kullanarak otomatik olarak simüle eden ve arka planda kendi kendine tamamlayan gelişmiş bir JavaScript otomasyon scripti.

---

## ✨ Özellikler ve Desteklenen Görevler

Script, Discord'un kendi API uç noktalarına doğrudan güvenli heartbeat (nabız) sinyalleri göndererek görevleri otomatik olarak listeler ve sırayla tamamlar:

| Görev Türü | Açıklama | Platform Desteği |
| :--- | :--- | :--- |
| `WATCH_VIDEO` | Video İzleme Görevleri | Tarayıcı & Masaüstü Uygulaması |
| `WATCH_VIDEO_ON_MOBILE` | Mobil Video Görevleri | Tarayıcı & Masaüstü Uygulaması |
| `PLAY_ACTIVITY` | Discord Aktivite Görevleri | Tarayıcı & Masaüstü Uygulaması |
| `PLAY_ON_DESKTOP` | Masaüstü Oyun Görevleri | **Sadece Masaüstü Uygulaması** |
| `STREAM_ON_DESKTOP` | Yayın Açma Görevleri | **Sadece Masaüstü Uygulaması** (+1 İzleyici) |

---

## 🛠️ Kullanım Rehberi (Adım Adım)

1. **VPN Bağlantınızı Sağlayın:** Discord Quest sistemi genellikle belirli bölgelere (Örn: ABD/Avrupa) açık olduğundan bilgisayarınızda bir VPN açık olmalıdır.
2. **Görevler Sekmesine Geçin:** Discord Ayarları altındaki **Görevler (Quests)** sayfasını açın.
3. **Geliştirici Konsolunu Açın:** Discord üzerindeyken `Ctrl + Shift + I` (Mac için `Cmd + Option + I`) tuşlarına basarak geliştirici araçlarını açın ve üstten **Console** sekmesine tıklayın.
4. **Güvenlik Engelini Kaldırın:** Eğer konsola ilk kez kod yapıştırıyorsanız, önce `allow pasting` yazıp `Enter` tuşuna basın.
5. **Kodu Çalıştırın:** Projedeki `script.js` dosyasının içindeki kodun tamamını kopyalayıp konsola yapıştırın ve `Enter`a basın.
6. **Keyfinize Bakın:** Script çalışmaya başladıktan sonra sekmeyi veya uygulamayı simge durumuna küçülterek arka planda bırakabilirsiniz. Script tüm görevleri sırasıyla bitirecektir.

---

## ⚠️ Önemli Detaylar ve Sınırlandırmalar

* **Masaüstü Gereksinimi:** Oyun oynama (`PLAY_ON_DESKTOP`) ve Yayın açma (`STREAM_ON_DESKTOP`) görevleri tarayıcı mimarisinde çalışmaz. Bu görevlerin ilerlemesi için script kesinlikle **Discord Masaüstü Uygulaması** üzerinde çalıştırılmalıdır.
* **Yayın Görevi Kuralı:** `STREAM_ON_DESKTOP` görevinin süresinin sayması için, bulunduğunuz ses kanalında yayınınızı izleyen **en az 1 kişinin (veya yan hesabınızın)** bulunması Discord API kuralları gereği zorunludur. İzleyici yoksa süre ilerlemez.

## ⚖️ Sorumluluk Reddi (Disclaimer)

Bu yazılım tamamen eğitim, test ve Discord'un dahili Webpack/API mimarisini analiz etme amacıyla geliştirilmiştir. Konsola harici script enjekte etmek ve otomatik istekler göndermek (self-botting) Discord Hizmet Şartları'na (ToS) aykırıdır. Hesabınızın güvenliği ve doğabilecek yaptırımlar tamamen kullanıcının sorumluluğundadır.

---
⭐ Bu proje işinize yaradıysa bir yıldız bırakarak destek olabilirsiniz!
