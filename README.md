# 🌳 Soy Ağacı

**Soy Ağacı**, tamamen tarayıcıda çalışan, sunucu gerektirmeyen Türkçe aile ağacı uygulamasıdır.

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
- **GEDCOM (.ged)** dışa aktarma
- **JSON** yedek dosyası dışa aktarma
- Sürükle-bırak ile dosya içe aktarma
- Yerleşik demo veri seti

---

## Teknoloji

| Katman | Kullanılan |
|--------|-----------|
| Arayüz | Vanilla HTML5 / CSS3 / JavaScript |
| Görselleştirme | Canvas API |
| Veri Saklama | `localStorage` → Supabase'e geçiş planlanıyor |
| Kimlik Doğrulama | Yok → Google OAuth planlanıyor |
| Bağımlılık | **Yok** — tek dosya, çevrimdışı çalışır |

---

## Kurulum

Herhangi bir kurulum gerekmez:

```
soy-agaci.html dosyasını tarayıcıda aç → kullanmaya başla
```

---

## Dosya Yapısı

```
temiz son/
├── soy-agaci.html   # Uygulamanın tamamı (HTML + CSS + JS)
├── temiz146.ged     # Örnek GEDCOM veri dosyası (146 kişi)
└── README.md        # Bu dosya
```

---

## Veri Yapısı (localStorage)

```
sa4   → { people: {...}, fams: {...}, nextId: number }
sa4nd → { [kişiId]: { x, y } }  // ağaç düğüm pozisyonları
```

---

## Planlanan Geliştirmeler

- [ ] **Supabase entegrasyonu** — çoklu cihaz senkronizasyonu, bulut yedekleme
  - `save()` → Supabase `upsert`
  - `load()` → Supabase `select`
  - `people` ve `nodeDrag` tabloları
- [ ] **Google ile giriş (OAuth)** — kişisel veri güvenliği
  - Supabase Auth + Google OAuth Provider
  - Kullanıcı bazlı veri izolasyonu
- [ ] **Kullanıcıya özel ağaç** — her kullanıcı kendi ağacını görür ve yönetir

---

## Sürüm Geçmişi

| Sürüm | Değişiklikler |
|-------|--------------|
| v3.0 | Fotoğraf galerisi, gelişmiş ilişki yönetimi, istatistik paneli |
| v2.0 | Canvas ağaç görselleştirme, GEDCOM içe/dışa aktarma |
| v1.0 | Temel kişi yönetimi, liste görünümü |

---

## Lisans

Kişisel kullanım.
