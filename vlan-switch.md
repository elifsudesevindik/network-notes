# VLAN ve Switch Port Türleri

## VLAN (Virtual Local Area Network)

VLAN, **aynı fiziksel ağ üzerindeki cihazları mantıksal olarak farklı ağlara ayırma yöntemidir**.  
Bu sayede ağ daha düzenli, güvenli ve yönetilebilir olur.

### VLAN'ın Avantajları

- Ağ trafiğini azaltır
- Güvenliği artırır
- Farklı departmanları ayırmayı sağlar
- Ağ yönetimini kolaylaştırır

### Örnek

Bir şirkette:

- VLAN 10 → Muhasebe
- VLAN 20 → IT
- VLAN 30 → İnsan Kaynakları

Bu VLAN’lar aynı switch üzerinde olsa bile **birbirleriyle doğrudan iletişim kuramaz**.

---

## Switch

Switch, **aynı ağ içindeki cihazların birbirleriyle iletişim kurmasını sağlayan ağ cihazıdır**.  
Switch, gelen veriyi MAC adresine göre doğru porta gönderir.

### Switch Özellikleri

- MAC adres tablosu tutar
- Veriyi doğru cihaza iletir
- Ağ performansını artırır

---

## Access Port

Access port, **tek bir VLAN'a bağlı olan switch portudur**.

Genellikle:

- Bilgisayarlar
- Yazıcılar
- IP telefonlar

gibi cihazlar access port üzerinden bağlanır.

Örnek:

```
Switch Port: Fa0/1
Mode: Access
VLAN: 10
```

Bu durumda porta bağlı cihaz **VLAN 10 içinde çalışır**.

---

## Trunk Port

Trunk port, **birden fazla VLAN trafiğini taşıyan switch portudur**.

Genellikle şu cihazlar arasında kullanılır:

- Switch ↔ Switch
- Switch ↔ Router
- Switch ↔ Firewall

Trunk bağlantı **802.1Q (dot1q)** protokolünü kullanır.

Örnek:

```
Switch Port: Fa0/24
Mode: Trunk
Allowed VLANs: 10,20,30
```

Bu port üzerinden **birden fazla VLAN taşınabilir**.

---

## VLAN Nasıl Çalışır?

1. Cihaz switch'e bağlanır  
2. Switch portu bir VLAN'a atanır  
3. Aynı VLAN içindeki cihazlar iletişim kurabilir  
4. Farklı VLAN’lar arasında iletişim için **router veya layer 3 switch** gerekir  

---

## Özet

- **VLAN:** Ağı mantıksal olarak bölmek için kullanılır  
- **Switch:** Ağ içindeki cihazların iletişimini sağlar  
- **Access Port:** Tek VLAN taşır  
- **Trunk Port:** Birden fazla VLAN taşır  
- VLAN’lar ağ güvenliği ve yönetimi için çok önemlidir
