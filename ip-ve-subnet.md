# IP, Subnet ve Gateway İlişkisi

## IP Address (IP Adresi) Nedir?

IP adresi, ağ üzerindeki her cihazın birbirini tanıyabilmesini sağlayan benzersiz sayısal kimliktir.  
Bir cihazın veri gönderebilmesi ve alabilmesi için mutlaka bir IP adresine sahip olması gerekir.

IP adresi iki bölümden oluşur:

- Network kısmı → cihazın hangi ağa ait olduğunu gösterir  
- Host kısmı → o ağ içindeki cihazı temsil eder  

Örnek IP:
```
192.168.1.10
```

---

## Subnet (Alt Ağ) Nedir?

Subnet, büyük bir IP ağının daha küçük mantıksal ağlara bölünmesidir.

Bu işlem:

- Ağ trafiğini azaltır  
- Performansı artırır  
- Yönetimi kolaylaştırır  
- Broadcast yayılımını sınırlar  

Subnet maskesi, IP adresinin hangi kısmının **network**, hangi kısmının **host** olduğunu belirler.

Örnek:

```
IP Address: 192.168.1.10
Subnet Mask: 255.255.255.0
```

Bu durumda:

- Network adresi → 192.168.1.0  
- Host aralığı → 192.168.1.1 – 192.168.1.254  
- Broadcast adresi → 192.168.1.255  

---

## Gateway (Varsayılan Ağ Geçidi) Nedir?

Gateway, bir cihazın kendi ağı dışındaki ağlara ulaşmasını sağlayan çıkış noktasıdır.

Çoğu ağda gateway adresi, router’ın yerel IP adresidir.

Cihaz başka bir ağa paket göndermek istediğinde:

1. Hedef IP kendi subnetinde mi kontrol edilir  
2. Değilse paket gateway’e gönderilir  
3. Gateway paketi doğru ağa yönlendirir  

Örnek:
```
Gateway: 192.168.1.1
```

---

## IP, Subnet ve Gateway Nasıl Birlikte Çalışır?

Bir cihazın internete veya başka ağlara erişebilmesi için üç bilgi gerekir:

- IP Address → cihazın ağdaki kimliği  
- Subnet Mask → hangi cihazların aynı ağda olduğunu belirler  
- Gateway → diğer ağlara çıkış yoludur  

Bu bilgiler olmadan:

- cihaz paketlerin nereye gideceğini bilemez  
- ağ dışına çıkamaz  
- iletişim kurulamaz  

---

## Gerçek Ağ Örneği

Bir ofis ağı:

```
IP Address: 192.168.10.25
Subnet Mask: 255.255.255.0
Gateway: 192.168.10.1
```

Bu durumda bilgisayar:

- Aynı subnet içindeki cihazlarla direkt haberleşir  
- Farklı ağlara gitmek için gateway’i kullanır  
- İnternete çıkarken router üzerinden yönlendirilir  

---

## Kısa Özet

- IP Address → cihazın adresi  
- Subnet → ağın sınırı  
- Gateway → dış ağlara açılan kapı  
