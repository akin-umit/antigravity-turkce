# Kod İmzalama ve SmartScreen

Antigravity Türkçe Manager'ın Windows dışı GitHub dağıtımlarında hedefimiz, tüm `.exe` ve kurulum dosyalarını aynı doğrulanmış yayıncı kimliğiyle Authenticode imzalamaktır.

## Plan

1. Geçerli bir **OV Code Signing** sertifikası edinilir.
2. Her yayın aynı yayıncı kimliğiyle imzalanır.
3. İmza algoritması **SHA-256** olur.
4. Her imzaya **RFC 3161 SHA-256 zaman damgası** eklenir.
5. İmzalama tamamlandıktan sonra dosya yeniden değiştirilmez.
6. İmzalı dosyanın SHA-256 karması Release varlığı olarak yayımlanır.
7. Manager güncelleyicisi indirdiği sürümün checksum bilgisini doğrular.

## SmartScreen hakkında önemli not

Geçerli OV/EV kod imzası, Windows'ta doğrulanmış yayıncı kimliğinin görünmesini sağlar; ancak yeni bir uygulamada SmartScreen uyarısını ilk günden garanti olarak kaldırmaz. Microsoft, SmartScreen itibarını hem yayıncı kimliği hem de dosya itibarı üzerinden zaman içinde oluşturur.

EV sertifikaları artık SmartScreen için anında güven sağlamadığından yalnızca bu amaçla EV seçilmesi planlanmamaktadır.

## Dağıtım seçenekleri

- **GitHub Releases:** Authenticode imzalı EXE/Setup + SHA-256 checksum.
- **Microsoft Store (gelecekte isteğe bağlı):** MSIX üzerinden dağıtım yapılırsa Store paketi Microsoft tarafından imzalanabilir ve SmartScreen indirme uyarısı oluşmaz.

## Sertifika güvenliği

Özel anahtar veya imzalama kimlik bilgileri public repoya, uygulama paketine ya da son kullanıcı bilgisayarına düz metin olarak konulmaz. Sertifika/anahtar yalnızca kontrollü yayın ortamında kullanılır.

## Doğrulama

Yayın aşamasında imzadan sonra şu kontroller zorunludur:

- Authenticode imza doğrulaması
- Zaman damgası doğrulaması
- SHA-256 checksum üretimi
- Release dosyası ile checksum eşleşmesi

Bu belge teknik yayın planını açıklar; sertifika başvurusu ve kimlik/kuruluş doğrulaması ilgili sertifika sağlayıcısının kurallarına tabidir.
