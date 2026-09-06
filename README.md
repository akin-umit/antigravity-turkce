<div align="center">

# 🇹🇷 Antigravity Türkçe

### Antigravity için tek tık Türkçe yama ve güncelleme yöneticisi

**Yama Geliştiricisi: Ümit Akın**

[![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011-2b79ff)](https://github.com/akin-umit/antigravity-turkce/releases/latest)
[![Latest Release](https://img.shields.io/github/v/release/akin-umit/antigravity-turkce)](https://github.com/akin-umit/antigravity-turkce/releases/latest)
[![License](https://img.shields.io/badge/license-Proprietary-red)](#lisans)

</div>

## Antigravity artık Türkçe konuşuyor

**Antigravity Türkçe Manager**, Antigravity'nin kullanıcı arayüzünü Türkçeleştiren, sürüme özel yedek alan ve Antigravity güncellemelerinden sonra Türkçe yamayı otomatik olarak onarabilen bağımsız bir Windows uygulamasıdır.

### Öne çıkanlar

- Tek tık **Türkçe yama kur / onar**
- Ayarlar, Agent izin pencereleri, MCP, Beceriler, Kısayollar ve temel Electron menülerinde Türkçe arayüz
- Her Antigravity sürümü için ayrı **orijinal yedek**
- ASAR oluşturma sonrası **bütünlük doğrulaması**
- **Otomatik Koruma:** Antigravity güncellemesi yamayı kaldırırsa yeni sürüme yeniden uygular
- Tek tık **orijinale geri dön**
- Manager için GitHub üzerinden **güncelleme kontrolü**
- İndirilen güncellemede **SHA-256 doğrulaması**
- Telemetri yok

## İndir

En güncel sürüm için **Releases** bölümünü kullanın:

**`Antigravity-Turkce-Setup.exe`** — önerilen kurulum paketi  
**`AntigravityTurkceManager.exe`** — taşınabilir sürüm

> Windows SmartScreen ilk yayınlarda bilinmeyen geliştirici uyarısı gösterebilir. Kod imzalama sertifikası eklendiğinde Authenticode doğrulaması yayın zincirine dahil edilecektir.

## Kullanım

1. Manager'ı açın.
2. Antigravity kurulumunun algılandığını kontrol edin.
3. **Türkçe Yamayı Kur / Onar** düğmesine basın.
4. İsterseniz **Otomatik Koruma** özelliğini açın.
5. Antigravity Türkçe olarak açılır.

Orijinale dönmek için **Yedek & Kurtarma → Son Orijinale Geri Dön** seçeneğini kullanın.

## Neler Türkçeleştirilir?

Manager; kullanıcıya görünen arayüz metinlerini, ayar açıklamalarını, menüleri, izin pencerelerini, MCP/Beceri kartlarını ve yaygın sistem metinlerini Türkçeleştirir.

Kod, terminal komutları, dosya yolları, API isimleri, model isimleri, paket/skill kimlikleri ve teknik olarak değiştirilmemesi gereken metinler bilerek orijinal bırakılır.

## Güncelleme sistemi

Antigravity güncellendiğinde `app.asar` yeniden oluşturulabilir. Otomatik Koruma açıksa Manager:

1. Yeni/yamasız sürümü algılar.
2. Antigravity kapanana kadar bekler.
3. Yeni sürümün orijinal dosyasını ayrı yedekler.
4. Türkçe yamayı yeni ASAR yapısına yeniden uygular.
5. Paketi doğrular.
6. Antigravity'yi tekrar Türkçe olarak açar.

## Gizlilik

Antigravity Türkçe Manager telemetri toplamaz, kullanıcı konuşmalarını okumaz ve kullanıcı kodunu herhangi bir sunucuya göndermez. Güncelleme kontrolü yapılırken yalnızca GitHub Releases API'sine istek gönderilir.

Ayrıntılar: [PRIVACY.md](PRIVACY.md)

## Geliştirici

**Ümit Akın**  
GitHub: [@akin-umit](https://github.com/akin-umit)  
Instagram: [@umit.aakinn](https://www.instagram.com/umit.aakinn/)

## Lisans

Bu yazılım kapalı kaynak ve özel lisanslıdır. Son kullanıcılar resmi dağıtım kanalından indirip kullanabilir. Kaynak kodun çıkarılması, değiştirilmiş sürümün yayımlanması, yeniden paketleme, geliştirici bilgisinin kaldırılması ve ticari yeniden satış yasaktır.

Ayrıntılar: [LICENSE.txt](LICENSE.txt)

## Marka / bağımsızlık bildirimi

Bu proje Google tarafından geliştirilmemiştir, Google ile bağlantılı değildir ve Google'ın resmî Türkçe çevirisi değildir. **Antigravity** adı ilgili hak sahiplerine aittir. Bu yazılım bağımsız bir yerelleştirme aracıdır.
