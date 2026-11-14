# Dokümantasyon dil politikası (EN / TR)

**Kuruluş:** xrystal-tech  
**Yürürlük:** 2026-11-14

## İlkeler

1. **Kullanıcıya dönük org politika ve sağlık dosyaları** **eşli belgeler** olarak tutulur: İngilizce (`.en.md` veya varsayılan `NAME.md`) ve Türkçe (`NAME.tr.md` veya `policies/NAME.tr.md`).
2. Politika metni için **her iki dil eşit yetkilidir**. Politika güncellerken aynı pull request’te iki dosyayı da değiştirin.
3. xrystal-tech **depo README** dosyalarında şunlar olmalıdır:
   - İngilizce `README.md`, ve
   - Türkçe `README.tr.md`, **veya** tek README içinde net `## English` ve `## Türkçe` bölümleri (uzun metinlerde ayrı dosya tercih edilir).

## Yalnızca İngilizce kalanlar

Araçlar ve API’lerin tutarlı kalması için uygulama depolarında şunlar yalnızca İngilizce kalabilir:

- Kaynak kod, tanımlayıcılar, commit mesajları (İngilizce tercih)
- OpenAPI / JSON Schema alan adları ve hata kodları
- CI iş akışı ve yapılandırma anahtarları

Katkı veren veya kullanıcıyı etkileyen davranışı dokümantasyonda EN/TR açıklayın.

## Depo politika dosyaları

| Dosya | English | Türkçe |
| --- | --- | --- |
| Depo politikası | `policies/repository-policy.en.md` | `policies/repository-policy.tr.md` |
| Gizlilik politikası | `policies/privacy-policy.en.md` | `policies/privacy-policy.tr.md` |

## İnceleme kontrol listesi

- [ ] Türkçe ve İngilizce bölümler aynı yükümlülükleri ve tarihleri taşıyor.
- [ ] Bağlantılar eş dosyaya gidiyor.
- [ ] Lisans bölümü [depo politikası](../../policies/repository-policy.tr.md) ile uyumlu (varsayılan lisanslı; depo `LICENSE` istisnası geçerli).