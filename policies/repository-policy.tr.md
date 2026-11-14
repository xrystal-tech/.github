# Depo politikası — Xrystal (xrystal-tech)

**Yürürlük:** 2026-11-14  
**Kapsam:** `xrystal-tech` GitHub kuruluşundaki tüm depolar; belirli bir depoda açıkça istisna tanımlanmadıkça.

## 1. Amaç

Bu politika, xrystal-tech depolarının tutarlı, hukuki açıdan net ve İngilizce ile Türkçe katkı verenlere erişilebilir kalmasını sağlar.

## 2. Lisanslama (varsayılan: lisanslı)

Belirli bir depo için aksisi yazılmadıkça:

1. **Her kamuya açık depo bir lisans dosyasıyla gelmelidir:** kökte `LICENSE` veya `LICENSE.md`.
2. **Kuruluş varsayılan lisansı** [MIT Lisansı](../license-templates/LICENSE-MIT)dır. Yeni depo açarken ve o proje için başka lisans onaylanmamışsa bu şablonu kullanın.
3. **Depo istisnası:** Depo kökünde farklı bir lisansı belirten `LICENSE` veya `LICENSE.md` varsa (örneğin Apache License 2.0, GPL-3.0 veya dosyada belgelenmiş özel bir SPDX tanımı), **o dosya o depo için bağlayıcıdır**. Kuruluş varsayılanı onun yerine geçmez.
4. **Özel depolar** da README’de lisans niyetini belgelemelidir (kodu kimlerin hangi koşullarda kullanabileceği). Depo kamuya açılacaksa, görünürlük değişmeden önce uygun bir `LICENSE` ekleyin.
5. **Lisanssız / “tüm hakları saklıdır”** yalnızca o deponun README’sinde açıkça yazılı ve kuruluş sahipleri tarafından onaylanmışsa mümkündür (istisna yolu — varsayılan değil).

### Kısa özet

| Durum | Ne yapmalı |
| --- | --- |
| Yeni depo, özel talimat yok | `license-templates/LICENSE-MIT` ile org varsayılan MIT |
| Depoda zaten `LICENSE` var | O dosyayı koruyun; README’de belirtin |
| O depoda başka lisans kullan denmiş | Lisansı `LICENSE` içine koyun; README’de yazın |

## 3. Zorunlu depo düzeni

Kamuya açık depolarda olması beklenenler:

- `README.md` ([i18n politikası](../docs/i18n/POLICY.tr.md))
- `LICENSE` veya `LICENSE.md` (belgelenmiş özel istisna hariç)
- Güvenlik iletişimi: kuruluş [SECURITY.tr.md](../SECURITY.tr.md) veya yalnızca org politikasını **genişleten** (çelişmeyen) depo içi `SECURITY.md`

Önerilenler:

- `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md` (`.github` deposundaki org varsayılanları)
- `.github` şablonlarından issue ve PR şablonları

## 4. İsimlendirme ve görünürlük

- Depo adları: küçük harf, tire ile (`my-service`); yayımlanmış ürün adı gerektirmedikçe.
- Yeni iş için varsayılan görünürlük: kuruluş sahiplerinin kararı (kamuya açılmaya hazır olana kadar özel; proje baştan açık değilse).
- Arşivlenen depolar: GitHub’da arşiv işaretleyin; geçmiş uyum için `LICENSE` kalsın.

## 5. Bağımlılıklar ve uyum

- Gizli anahtar, üretim kimlik bilgisi veya projeyle ilgisiz kişisel veri commit’lenmez.
- Üçüncü taraf kod kendi lisansına uyar; gerekirse README veya `NOTICE` içinde yükümlülükler belirtilir (örneğin Apache-2.0).

## 6. İstisnalar

Bir depo, yalnızca şunları kapsayan `POLICY.override.md` ile (README’den bağlantılı) istisna tanımlayabilir:

- Lisans seçimi (yine de kökte `LICENSE` veya `LICENSE.md` olmalı)
- Daha sıkı güvenlik veya katkı kuralları

Bu depodaki kuruluş çapı poliçeleri, açıkça istisna olmayan konularda geçerliliğini korur.

## 7. Değişiklikler

Politika değişikliği önerileri: `xrystal-tech/.github` içinde issue veya PR; **İngilizce ve Türkçe** politika dosyaları birlikte güncellenir.