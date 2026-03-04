# TCP vs UDP

## TCP (Transmission Control Protocol)

TCP, **bağlantı tabanlı** bir protokoldür.  
Veriyi karşı tarafa **sıralı ve güvenli** şekilde iletir.  
Eksik paket olursa tekrar gönderilir, yani veri kaybı minimumdur.

Özellikleri:

- Bağlantı kurar (3-way handshake)  
- Paketlerin sırasını kontrol eder  
- Veri kaybı olursa yeniden gönderir  
- Ağda daha yavaştır ama güvenlidir  

Kullanım alanları:

- Web siteleri (HTTP/HTTPS)  
- E-posta (SMTP, POP3)  
- Dosya transferi (FTP)  

---

## UDP (User Datagram Protocol)

UDP, **bağlantısız** bir protokoldür.  
Veriyi hızlı gönderir fakat paket kaybı veya sırasızlık yaşanabilir.  
Kontrol mekanizması yoktur, bu yüzden daha hızlıdır.

Özellikleri:

- Bağlantı kurmaz  
- Paket sırasını kontrol etmez  
- Hata kontrolü sınırlıdır  
- Ağda hızlıdır, düşük gecikmeli uygulamalar için uygundur  

Kullanım alanları:

- Online oyunlar  
- Canlı yayın (streaming)  
- DNS sorguları  
- VoIP (Sesli iletişim)

---

## TCP ve UDP Arasındaki Farklar

| Özellik              | TCP                     | UDP                 |
|----------------------|------------------------|-------------------|
| Bağlantı             | Var                     | Yok               |
| Paket Sırası          | Kontrol edilir          | Kontrol edilmez   |
| Veri Güvenliği        | Yüksek                  | Düşük             |
| Hız                   | Daha yavaş              | Daha hızlı        |
| Örnek Kullanım        | Web, E-posta, FTP       | Oyun, Video, DNS  |

---

## Paket Yolculuğu

TCP ve UDP paketleri IP protokolü üzerinden iletilir.  
Yani önce **IP adresi ile yönlendirilir**, sonra TCP veya UDP protokol kuralları uygulanır.  

Örnek:

1. PC → Router → Switch → Internet  
2. Paket IP ile hedefe yönlendirilir  
3. TCP ise sıralama ve kontrol yapılır  
4. UDP ise hızlıca gönderilir, kayıp varsa kayıp olur

---

## Özet

- **TCP:** Güvenli, yavaş, bağlantı tabanlı  
- **UDP:** Hızlı, bağlantısız, paket kaybı olabilir  
- Hangi protokol kullanılacağı uygulamanın ihtiyacına bağlıdır  
