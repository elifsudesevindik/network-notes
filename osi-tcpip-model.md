# OSI Modeli ve TCP/IP Modeli

## OSI Modeli

OSI (Open Systems Interconnection) modeli, ağ iletişiminin nasıl gerçekleştiğini açıklayan **7 katmanlı bir modeldir**.

Bu model, ağdaki veri iletişimini anlamayı ve sorunları analiz etmeyi kolaylaştırır.

### OSI Katmanları

1. Physical (Fiziksel Katman)
2. Data Link (Veri Bağlantı Katmanı)
3. Network (Ağ Katmanı)
4. Transport (Taşıma Katmanı)
5. Session (Oturum Katmanı)
6. Presentation (Sunum Katmanı)
7. Application (Uygulama Katmanı)

---

## 1. Physical Layer

Verinin fiziksel ortam üzerinden iletilmesini sağlar.

Örnekler:

- Ethernet kablosu
- Fiber kablo
- Elektrik sinyalleri

---

## 2. Data Link Layer

Aynı ağ içindeki cihazların iletişimini sağlar.

Özellikleri:

- MAC adresleri kullanılır
- Switch bu katmanda çalışır

---

## 3. Network Layer

Farklı ağlar arasındaki iletişimi sağlar.

Özellikleri:

- IP adresleri kullanılır
- Router bu katmanda çalışır

---

## 4. Transport Layer

Verinin doğru şekilde iletilmesini sağlar.

Örnek protokoller:

- TCP
- UDP

---

## 5. Session Layer

Cihazlar arasında oturum oluşturur ve yönetir.

---

## 6. Presentation Layer

Verinin formatını düzenler.

Örnekler:

- Şifreleme
- Veri sıkıştırma

---

## 7. Application Layer

Kullanıcıya en yakın katmandır.

Örnek protokoller:

- HTTP
- FTP
- SMTP
- DNS

---

## TCP/IP Modeli

TCP/IP modeli internetin kullandığı daha basit bir ağ modelidir.

Bu model **4 katmandan oluşur**.

### TCP/IP Katmanları

1. Network Interface
2. Internet
3. Transport
4. Application

---

## OSI ve TCP/IP Karşılaştırması

| OSI Modeli | TCP/IP Modeli |
|------|------|
| 7 Katman | 4 Katman |
| Daha teorik | Daha pratik |
| Ağ eğitiminde kullanılır | İnternette kullanılır |

---

## Özet

- **OSI modeli 7 katmandan oluşur**
- Ağ iletişimini anlamayı kolaylaştırır
- **TCP/IP modeli internetin kullandığı modeldir**
- TCP ve UDP transport katmanında çalışır
