<div align="center">

<img src="assets/viacore-logo.png" width="104" height="104" alt="ViaCore logosu" />

# ViaCore Proxy Management

**Windows için uygulama bazlı proxy yönetimi**

Hangi uygulamanın internete proxy üzerinden, doğrudan ya da hiç çıkmayacağına siz karar verin.

[![Son sürüm](https://img.shields.io/github/v/release/yigitira92/viacore-releases?style=flat-square&label=s%C3%BCr%C3%BCm&color=7C3AED)](https://github.com/yigitira92/viacore-releases/releases/latest)
[![İndirme](https://img.shields.io/github/downloads/yigitira92/viacore-releases/total?style=flat-square&label=indirme&color=3B82F6)](https://github.com/yigitira92/viacore-releases/releases)
[![Windows](https://img.shields.io/badge/Windows-7%20%E2%80%93%2011-0078D4?style=flat-square&logo=windows&logoColor=white)](#sistem-gereksinimleri)
[![Mimari](https://img.shields.io/badge/mimari-x64-475569?style=flat-square)](#sistem-gereksinimleri)

<br />

<a href="https://github.com/yigitira92/viacore-releases/releases/latest/download/ViaCore-Setup.msi"><img src="https://img.shields.io/badge/%C4%B0ND%C4%B0R-Windows%20x64-7C3AED?style=for-the-badge&logo=windows&logoColor=white" height="40" alt="İndir (Windows x64)" /></a>

<sub>Her zaman son sürüm (.msi) · Türkçe ve İngilizce arayüz · Otomatik güncelleme · <a href="https://github.com/yigitira92/viacore-releases/releases">Tüm sürümler</a></sub>

</div>

---

## Neler yapabilirsiniz

<table>
<tr>
<td width="50%" valign="top">

### 🎯 Uygulama bazlı kurallar

Uygulamaya, hedef adrese (IP, CIDR, aralık, alan adı) ve porta göre kurallar yazın. Kurallar yukarıdan aşağı değerlendirilir; ilk eşleşen kazanır, hiçbirine uymayan bağlantı varsayılan kurala gider.

</td>
<td width="50%" valign="top">

### 🔌 Yaygın proxy türlerinin hepsi

SOCKS5, SOCKS4/4A, HTTPS (CONNECT) ve HTTP proxy'leri. Kimlik doğrulama: kullanıcı adı ve parola, NTLM, Kerberos, Negotiate ya da Windows oturumunuz.

</td>
</tr>
<tr>
<td valign="top">

### ⛓️ Proxy zincirleri

Basit zincirler, bir proxy yanıt vermezse sıradakine geçen yedekli zincirler ve yükü proxy'ler arasında paylaştıran zincirler.

</td>
<td valign="top">

### 🌐 Ad çözümleme proxy üzerinden

Proxy'ye yönlendirilen alan adları yerel DNS sunucusuna sorulmaz; proxy tarafında çözülür.

</td>
</tr>
<tr>
<td valign="top">

### 📊 Canlı bağlantılar

Hangi uygulamanın nereye, hangi kuralla ve hangi proxy üzerinden bağlandığını, gecikmesini ve aktardığı veriyi anlık izleyin.

</td>
<td valign="top">

### 🎮 GamingProxy hesabı

İsteğe bağlı: GamingProxy hesabınızla giriş yapın, satın aldığınız proxy'leri tek tıkla içe aktarın.

</td>
</tr>
<tr>
<td valign="top">

### 🗂️ Profiller

Ayarlarınızı profil olarak saklayın, dışa ve içe aktarın; isterseniz profil bir adresten kendiliğinden güncellensin.

</td>
<td valign="top">

### 🔄 Otomatik güncelleme

Yeni sürümler arka planda iner, imzası doğrulanır ve kendiliğinden kurulur.

</td>
</tr>
</table>

## Kurulum

1. **[ViaCore-Setup.msi](https://github.com/yigitira92/viacore-releases/releases/latest/download/ViaCore-Setup.msi)** dosyasını indirin. Bu bağlantı her zaman son sürümü indirir.
2. Dosyayı çalıştırın ve sihirbazı izleyin. Kurulum yönetici izni ister.
3. Kurulum bitince ViaCore açılır. ViaCore hizmeti Windows ile birlikte kendiliğinden başlar; pencereyi kapatsanız da yönlendirme sürer.

Kurulum sihirbazı, Windows dilinize göre Türkçe ya da İngilizce açılır.

## Güncellemeler

Ayrı bir yama dosyası yoktur: her sürüm, hem yeni kurulumda hem güncellemede kullanılan tek bir kurulum dosyasıdır.

Kurulu ViaCore yeni sürümü bir sonraki açılışta, yönetim penceresi açıldığında ya da en geç 12 saat içinde bu depoda bulur. Dosyayı indirir, ViaCore'un güncelleme anahtarıyla imzalandığını ve dosyanın değişmediğini doğrular, sonra kendiliğinden kurar. İmzası doğrulanmayan hiçbir dosya kurulmaz.

Tüm sürümler ve değişiklik notları: **[Sürümler](https://github.com/yigitira92/viacore-releases/releases)**

## Sistem gereksinimleri

| | |
|---|---|
| **Windows** | Windows 7 SP1, 8, 8.1, 10 veya 11, 64 bit |
| **.NET** | .NET Framework 4.6.1 veya üzeri (Windows 10 ve 11'de yerleşik; Windows 7 ve 8'de Microsoft'tan kurulur, kurulum eksikse söyler) |
| **Yetki** | Kurulum için yönetici hakkı |

> Windows 7 SP1'de Microsoft'un SHA-2 imza desteği güncellemesi (KB4474419) kurulu olmalıdır; Windows Update bunu 2019'dan beri sunar. Kurulum, Windows sürümünüze uygun trafik yakalama sürücüsünü kendisi seçer. Windows 8 ve 8.1 desteklenmek üzere hazırlandı, henüz test edilmedi.

## Güvenlik

- Proxy parolaları Windows DPAPI ile şifrelenerek saklanır.
- Yönetim penceresi hizmete yalnızca bu bilgisayarın içindeki, erişimi sınırlı bir kanal üzerinden bağlanır.
- Güncellemeler imzalıdır ve yalnızca bu depodan alınır.

## Üçüncü taraf bileşenler

ViaCore, [WinDivert 2.2](https://github.com/basil00/WinDivert) bileşenini LGPLv3 lisansıyla, değiştirmeden kullanır. Ayrıntılar ve lisans metni: [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) · [third_party/WinDivert/LICENSE](third_party/WinDivert/LICENSE)

---

<details>
<summary><b>English</b></summary>

<br />

**ViaCore Proxy Management** sends each Windows application through a proxy, directly, or blocks it, by rules on the application, the destination and the port.

- **Download:** [ViaCore-Setup.msi](https://github.com/yigitira92/viacore-releases/releases/latest/download/ViaCore-Setup.msi), always the newest version ([all releases](https://github.com/yigitira92/viacore-releases/releases)). Setup needs administrator rights; the wizard opens in English or Turkish, following Windows.
- **Proxies:** SOCKS5, SOCKS4/4A, HTTPS (CONNECT) and HTTP, with user name and password, NTLM, Kerberos, Negotiate or your Windows login; chains with failover and load balancing; name resolution through the proxy.
- **Live view:** which application connects where, by which rule and through which proxy, with latency and traffic.
- **Updates:** there are no separate patches. Every release is one installer that also updates existing installations. Installed copies find a new release at their next start, when the window opens, or within 12 hours, verify its signature and install it themselves.
- **Requirements:** Windows 7 SP1, 8, 8.1, 10 or 11, 64-bit, .NET Framework 4.6.1 or later. Windows 7 SP1 needs Microsoft's SHA-2 code signing update (KB4474419). Setup picks the interception driver build your Windows accepts. Windows 8 and 8.1 are prepared for but not yet tested.
- **Third-party:** WinDivert 2.2 under the LGPLv3, redistributed unmodified. See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

</details>

---

<div align="center">
<sub>© 2026 SERVERVİA BİLİŞİM YAZILIM VE TELEKOMÜNİKASYON HİZMETLERİ LİMİTED ŞİRKETİ · Tüm hakları saklıdır.</sub>
</div>
