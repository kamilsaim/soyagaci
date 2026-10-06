<div align="center">

<img src="logo.png" alt="Soy Ağacı" width="220">

# Soy Ağacı

**Ailenin hikâyesini tek yerde topla**

_Tarayıcıda çalışan, Türkçe, kurulum gerektirmeyen aile ağacı uygulaması_

[![Uygulamayı Aç](https://img.shields.io/badge/▶_Uygulamayı_Aç-c8855a?style=for-the-badge)](https://kamilsaim.github.io/soyagaci/)

![Sürüm](https://img.shields.io/badge/sürüm-5.2-8faa8a?style=flat-square)
![Tek dosya](https://img.shields.io/badge/tek_dosya-HTML-7ba3b8?style=flat-square)
![Bağımlılık](https://img.shields.io/badge/framework-yok-c9a87c?style=flat-square)
![Dil](https://img.shields.io/badge/dil-Türkçe-b89ab8?style=flat-square)

</div>

---

## Soy Ağacı nedir?

Ailenizin nesiller boyu bilgisini — kim kiminle evli, kimin çocuğu kim, kim ne zaman doğmuş ya da vefat etmiş — tek bir yerde toplayıp görsel bir ağaç hâlinde gezmenizi sağlar.

Kurulum yok, hesap açma zorunluluğu yok. Bağlantıyı açtığınız anda çalışır.

- **Google ile giriş yaparsanız** verileriniz bulutta saklanır ve tüm cihazlarınızdan aynı ağaca ulaşırsınız.
- **Giriş yapmazsanız** uygulama tamamen çevrimdışı çalışır; veriler yalnızca o cihazın tarayıcısında kalır.

---

## Hızlı başlangıç

| Adım | Ne yapılır |
|:---:|---|
| **1** | [Uygulamayı aç](https://kamilsaim.github.io/soyagaci/) → Google ile giriş yap veya **Yerel olarak kullan**'a tıkla |
| **2** | **+ Kişi** ile ilk kişiyi ekle — ya da elinizde `.ged` dosyası varsa **GED Yükle** ile hepsini birden aktar |
| **3** | Formdaki **Anne / Baba / Eşler / Çocuklar** alanlarından bağlantıları kur. Kişi listede yoksa **➕ Yeni … Ekle** ile aynı ekrandan oluştur |
| **4** | **🌳 Ağaç** sekmesinde sürükleyerek gez, düğümleri istediğin yere taşı |
| **5** | **⚙️ Ayarlar → JSON Yedek Al** ile düzenli yedek al |

---

## Özellikler

### 🌳 Ağaç görünümü
Canvas üzerinde sürüklenebilir, yakınlaştırılabilir aile ağacı. Kuşaklar otomatik hizalanır, beğenmediğiniz yerleşimi elle düzeltebilirsiniz — taşıdığınız her düğüm kendiliğinden kaydedilir.

| Hareket | Sonuç |
|---|---|
| Sürükle | Ağacı kaydır |
| Tık / dokunuş | Kişi kartını aç |
| Uzun bas + sürükle | Düğümü taşı (otomatik kaydedilir) |
| Fare tekerleği / iki parmak | Yakınlaştır–uzaklaştır |
| `⛶` | Tüm ağacı ekrana sığdır |
| `↺` | Elle yapılan yerleşimi sıfırla |

### 💑 Zengin aile ilişkileri
Çoklu eş desteği — her eş için ayrı durum: **evli**, **boşanmış** 💔, **dul** 🕊️, **birlikte** 🤝. Kızlık soyadı, tek ebeveynli çocuklar ve üvey bağlar doğru biçimde saklanır. Kişinin kendi atası olmasını engelleyen döngü koruması vardır.

### 📸 Fotoğraf galerisi
Kişi başına bir ana fotoğraf ve sınırsız galeri. Sürükle-bırak ile yükleyin, tam ekran lightbox'ta gezin, ok tuşlarıyla ilerleyin.

Fotoğraflar yüklenirken otomatik küçültülür (en uzun kenar 1400 px, JPEG) ve **buluttaki özel deponuza** kaydedilir — ağaç verisinin kendisi küçük ve hızlı kalır. Depo herkese kapalıdır; görüntüleme kısa ömürlü imzalı bağlantılarla yapılır ve yalnızca sizin oturumunuz erişebilir. Bir fotoğraf artık hiçbir kişide kullanılmıyorsa kendiliğinden silinir.

### 📊 İstatistikler
Toplam kişi, hayatta olanlar, **kuşak sayısı**, vefat edenlerin ortalama ömrü, yaşayanların ortalama yaşı, yaşam rekorları, en sık isimler, on yıllara göre doğum grafiği, doğum yerleri ve soyadı dağılımı. Ayrıca **30 gün içindeki doğum günleri** 🎂 listelenir.

### 🔍 Eksik veri raporu
Hangi kişide ad, soyad, doğum tarihi, fotoğraf ya da bağlantı eksik — tek listede görün, tıklayıp tamamlayın.

### 📁 İçe / dışa aktarma
- **GEDCOM 5.5.1** — MyHeritage, Ancestry ve benzeri programlarla iki yönlü uyum. Dışa aktarımda `FAMC`/`FAMS` işaretçileri, kızlık soyadı ve standart tarih biçimi yazılır.
- **JSON yedek** — tüm kişileri, bağlantıları ve fotoğraf referanslarını içerir; aynı butonla geri yüklenir. Bulut fotoğraflarının kendisi ayrı depoda durur, yedek dosyasında yalnızca bağlantıları bulunur (yani yedek aynı hesapta geri yüklenmelidir).
- Üzerine yazacak her içe aktarma işlemi önce onay sorar.

### ☁️ Güvenli senkronizasyon
Değişiklikler önce cihaza, ardından buluta yazılır. Başlıktaki küçük gösterge kaydın durumunu belli eder (⟳ kaydediliyor · ✓ kaydedildi · ! hata). Aynı ağacı iki cihazdan düzenlerseniz uygulama üzerine yazmadan önce sizi uyarır; "buluttakini yükle" derseniz bulut sürümü korunur. Bağlantı koparsa değişiklikler cihazda bekler ve bağlantı gelince gönderilir — cihaz saatinin yanlış olması başka cihazdaki değişiklikleri silemez. Buluta gönderilmemiş değişiklik varken çıkış yapmak isterseniz uygulama sizi uyarır.

---

## Veri ve gizlilik

- Veriler kişisel Supabase projesinde, **satır bazlı güvenlik (RLS)** ile saklanır: her kullanıcı yalnızca kendi satırını okuyabilir ve yazabilir.
- Giriş yapmadan kullanırken hiçbir veri cihazdan dışarı çıkmaz.
- Fotoğraflar ayrı, **herkese kapalı** bir Supabase Storage kovasında `{kullanıcı-kimliği}/…` yolunda saklanır; depo politikaları başka kimsenin klasörünüze erişmesine izin vermez.
- Giriş yapmadan kullanırken fotoğraflar (küçültülmüş hâlde) tarayıcıda saklanır; çok sayıda fotoğrafta depolama sınırı dolabilir, uygulama sizi uyarır.
- **Düzenli JSON yedeği alın.** Ayarlar → *JSON Yedek Al*.

---

## Teknoloji

| | |
|---|---|
| Arayüz | Saf HTML + CSS + JavaScript — framework yok, derleme adımı yok |
| Dağıtım | Tek `index.html` dosyası, GitHub Pages üzerinden yayınlanır |
| Kimlik | Supabase Auth (Google OAuth) |
| Veri | Supabase Postgres (`soy_family_data`, `soy_node_positions`), RLS açık |
| Fotoğraf | Supabase Storage — özel `soy-fotograf` kovası, kullanıcı bazlı erişim politikaları |
| Çizim | HTML5 Canvas, `devicePixelRatio` desteğiyle retina/mobil ekranlarda net |
| Mobil | Capacitor ile Android APK olarak paketlenebilir |

---

## Sürüm geçmişi

| Sürüm | Öne çıkanlar |
|---|---|
| **5.2** | **Güvenlik ve senkronizasyon denetimi.** Çakışmada bulut sürümü artık korunuyor · cihaz saati farkı veri silemiyor · bağlantı hatasında eski veri buluta gönderilmiyor · çıkışta kaydedilmemiş değişiklik uyarısı · düzenleme formunda bulut fotoğrafı görünüyor · GED aktarımında kızlık soyadı ve çok satırlı notlar korunuyor · ebeveyn/eş bağlantı düzeltmeleri · JSON yedek dosyası doğrulaması |
| **5.1** | Fotoğraflar Supabase Storage'a taşındı, yüklemede otomatik küçültme, kullanılmayan fotoğrafların otomatik temizliği; kullanılmayan `fams` alanı kaldırıldı |
| **5.0** | **Büyük kararlılık sürümü.** Çoklu eş düzenlemede artık kaybolmuyor · GED/JSON/demo yüklemeden önce onay · JSON yedeği geri yükleme · bulut hata ve çakışma bildirimi · Türkçe büyük harf düzeltmesi (İbrahim) · tüm tarih biçimleri tek kalıba · retina/mobil net çizim · tek tıkla kart açma · düğüm konumları otomatik kayıt · soy döngüsü koruması · kuşak sayısı istatistiği · XSS koruması |
| **4.7** | Yeni kişi eklerken akıllı otomatik yerleşim, yaklaşan doğum günleri |
| **4.5** | Otomatik güncelleme sistemi, ana ekran ikonu, gelişmiş form düzeni |
| **4.0** | Google ile giriş, bulut yedekleme, aile arması logosu, mobil alt menü |
| **3.0** | Eksik veri raporu, hızlı kişi ekleme, ağaç konumlarını hatırlama |
| **2.5** | Boşanmış eşler 💔, kızlık soyadı, yaşam istatistikleri |
| **2.0** | Sürüklenebilir canvas ağaç görünümü |
| **1.5** | Fotoğraf galerisi ve toplu silme |
| **1.0** | İlk sürüm — GEDCOM içe/dışa aktarma, liste ve ağaç görünümü |

---

## Katkı

Ailenden biri misin? [Uygulamayı aç](https://kamilsaim.github.io/soyagaci/), kendi Google hesabınla giriş yap ve bildiklerini ekle. Her hesap kendi ağacını tutar; eksik bir dal fark edersen bize ulaştır, birleştirelim.

---

<div align="center">
<sub>🌳 Aile, nesilden nesile aktarılan bir hikâyedir — Soy Ağacı onu yaşatır.</sub>
</div>
