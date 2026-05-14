# Soy Ağacı

**Soy Ağacı v4.7** 

v4.7 — Ağaçta yeni kişi akıllı konumlandırma (eş yana, çocuk alta, ebeveyn üste), yaklaşan doğum günleri istatistiği, bulut/yerel mod veri ayrımı, otomatik güncelleme cache-buster düzeltmesi

v4.5 — Otomatik güncelleme, ana ekran ikonu, anne/baba cinsiyet filtresi, form düzeni iyileştirmesi, tarih dönüştürücü, modal ortalama

tamamen tarayıcıda çalışan Türkçe aile ağacı uygulamasıdır. Google hesabıyla giriş yaparak verilerini bulutta sakla ya da çevrimdışı yerel olarak kullan.

---

## Özellikler

### Kişi Yönetimi
- Kişi ekleme, düzenleme ve silme
- Ad, soyad, kızlık soyadı, cinsiyet bilgileri
- Doğum / ölüm tarihi ve yeri
- Meslek ve notlar
- Ana fotoğraf + fotoğraf galerisi desteği

### Aile İlişkileri
- Anne / baba bağlantıları
- Eş / partner bağlantıları (evli, boşanmış, dul, partner)
- Çocuk bağlantıları
- Düzenleme sırasında hızlı kişi ekleme

### İnteraktif Ağaç Görselleştirme
- Canvas tabanlı aile ağacı
- Sürükle-bırak ile gezinme ve düğüm taşıma
- Mouse tekerleği ve pinch zoom (mobil)
- Çift tıklama ile kişi detayı
- Renk kodlaması: mavi (erkek), pembe (kadın)
- Evlilik / boşanma simgeleri (♥ / 💔)

### Liste Görünümü
- Ad ile arama ve filtreleme
- Filtreler: Tümü, Erkek, Kadın, Yaşıyor, Vefat etti
- Toplu seçim ve silme

### İstatistik Paneli
- Toplam kişi, cinsiyet dağılımı
- Yaşayan / vefat etmiş sayısı
- Ortalama yaşam süresi
- En yaşlı / en genç vefat kaydı
- En çok tekrarlanan isimler
- Doğum on yılı dağılımı
- En sık doğum yerleri, soyadı listesi

### Eksik Veri Raporu
- Ad, soyad, doğum tarihi olmayan veya bağlantısız kişiler
- Hızlı düzenleme erişimi

### İçe / Dışa Aktarma
- **GEDCOM (.ged)** içe aktarma — MyHeritage, Ancestry uyumlu
- **GEDCOM (.ged)** dışa aktarma (INDI + FAM kayıtları)
- **JSON** yedek dosyası dışa aktarma
- Sürükle-bırak ile dosya içe aktarma
- Yerleşik demo veri seti

---

## Teknoloji

| Katman | Kullanılan |
|--------|-----------|
| Arayüz | Vanilla HTML5 / CSS3 / JavaScript |
| Görselleştirme | Canvas API |
| Veri Saklama | `localStorage` + Supabase (bulut) |
| Kimlik Doğrulama | Supabase Auth — Google OAuth |
| Bağımlılık | Supabase JS v2 CDN (opsiyonel) |

---

## Kurulum

Herhangi bir kurulum gerekmez:

```
soy-agaci.html dosyasını tarayıcıda aç → kullanmaya başla
```

Google ile giriş yaparak Supabase bulut yedeklemesini etkinleştirebilir ya da "Yerel olarak kullan" butonuyla çevrimdışı devam edebilirsin.

---

## Dosya Yapısı

```
temiz son/
├── soy-agaci.html   # Uygulamanın tamamı (HTML + CSS + JS)
├── temiz146.ged     # Örnek GEDCOM veri dosyası (146 kişi)
└── README.md        # Bu dosya
```

---

## Veri Yapısı

**localStorage (çevrimdışı mod):**
```
sa4   → { people: {...}, fams: {...}, nextId: number }
sa4nd → { [kişiId]: { x, y } }  // ağaç düğüm pozisyonları
```

**Supabase (bulut mod):**
```
family_data   → { user_id, people, fams, next_id }
node_positions → { user_id, positions }
```

---

## Sürüm Geçmişi

| Sürüm | Değişiklikler |
|-------|--------------|
| v4.0 | Google ile giriş (Supabase Auth), bulut yedekleme, aile arması logosu, PWA favicon, mobil alt menü, animasyonlu simgeler |
| v3.0 | Fotoğraf galerisi, gelişmiş ilişki yönetimi, istatistik paneli, eksik veri raporu |
| v2.0 | Canvas ağaç görselleştirme, GEDCOM içe/dışa aktarma |
| v1.0 | Temel kişi yönetimi, liste görünümü |

---

## Lisans

Kişisel kullanım.
