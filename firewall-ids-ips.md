# Firewall, IDS ve IPS

## Firewall

Firewall, **ağ trafiğini kontrol eden ve güvenlik kurallarına göre izin veren veya engelleyen sistemdir**.

Firewall, iç ağ ile dış ağ (internet) arasında bir güvenlik duvarı görevi görür.

### Firewall Ne Yapar?

- Gelen ve giden trafiği kontrol eder
- Belirli portları açar veya kapatır
- Zararlı bağlantıları engeller
- Ağ güvenliğini artırır

### Firewall Türleri

**Packet Filtering Firewall**

- Paketleri IP ve port bilgisine göre kontrol eder

**Stateful Firewall**

- Bağlantının durumunu takip eder
- Daha gelişmiş güvenlik sağlar

**Application Firewall**

- Uygulama seviyesinde trafiği inceler
- Örneğin HTTP veya FTP trafiğini analiz eder

---

## IDS (Intrusion Detection System)

IDS, **ağdaki şüpheli veya saldırı davranışlarını tespit eden sistemdir**.

IDS saldırıyı **engellemez**, sadece **tespit eder ve uyarı verir**.

### IDS Ne Yapar?

- Şüpheli ağ trafiğini analiz eder
- Saldırı imzalarını kontrol eder
- Sistem yöneticisine uyarı gönderir

### IDS Türleri

**Network IDS (NIDS)**

- Ağ trafiğini izler

**Host IDS (HIDS)**

- Tek bir bilgisayarı veya sunucuyu izler

---

## IPS (Intrusion Prevention System)

IPS, IDS’e benzer ancak **saldırıları tespit etmekle kalmaz, aynı zamanda engeller**.

IPS genellikle **ağ trafiğinin ortasında çalışır** ve zararlı paketleri doğrudan durdurabilir.

### IPS Ne Yapar?

- Zararlı paketleri engeller
- Şüpheli IP adreslerini bloklar
- Saldırıları otomatik durdurur

---

## IDS ve IPS Arasındaki Fark

| Özellik | IDS | IPS |
|------|------|------|
| Amaç | Saldırıyı tespit etmek | Saldırıyı tespit edip engellemek |
| Trafik | Trafiği izler | Trafiği aktif olarak kontrol eder |
| Müdahale | Uyarı verir | Trafiği bloklar |

---

## Firewall, IDS ve IPS Birlikte Kullanımı

Modern ağ güvenliğinde bu sistemler birlikte kullanılır.

Örnek bir yapı:

Internet → Firewall → IPS → İç Ağ

Bu yapı sayesinde:

- Firewall temel filtreleme yapar
- IPS saldırıları engeller
- IDS ise analiz ve uyarı sağlar

---

## Özet

- **Firewall:** Ağ trafiğini kurallara göre kontrol eder
- **IDS:** Saldırıları tespit eder ve uyarı verir
- **IPS:** Saldırıları tespit eder ve engeller

Bu üç sistem, ağ güvenliğinin temel yapı taşlarıdır.
