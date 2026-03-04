# Routing ve NAT

## Routing (Yönlendirme)

Routing, **verinin ağlar arasında doğru yoldan iletilmesi işlemidir**.  
Router, paketleri hedef IP’ye göre en uygun yoldan yollar.

### Routing Türleri

- **Static Routing:** Yollar manuel olarak tanımlanır.  
  - Avantaj: Basit ve kontrol kolay  
  - Dezavantaj: Ağ büyüdükçe yönetimi zor  
- **Dynamic Routing:** Routerlar yolları otomatik öğrenir (RIP, OSPF gibi protokollerle)  
  - Avantaj: Ağ değişikliklerine otomatik uyum  
  - Dezavantaj: Daha karmaşık

### Routing Table

Router’ın bildiği tüm yolların listesi.  
Her paket, routing table’a bakarak hedefe gönderilir.

### Default Route

Bilinmeyen IP’ler için kullanılan varsayılan yol.  
Örneğin internet trafiği için çoğu zaman router üzerindeki default route kullanılır.

---

## NAT (Network Address Translation)

NAT, **iç ağdaki IP’leri tek bir public IP üzerinden internete çıkarma işlemidir**.  

### NAT Türleri

- **Static NAT:** İç IP → Tek bir dış IP’ye eşlenir  
- **Dynamic NAT:** İç IP → Dış IP havuzundan rastgele atanır  
- **PAT (Port Address Translation / NAT Overload):**  
  - Tek public IP’yi birden fazla cihaz için port bazlı kullanır  
  - İnternete çıkış yapan cihazların port numaraları ile ayrılır

### NAT Kullanım Amacı

- İç ağ güvenliği  
- IP adres tasarrufu  
- İnternet çıkışı kontrolü  

---

## Routing ve NAT Birlikte Çalışması

1. Paket, cihazdan router’a gelir  
2. Router, IP’ye göre doğru ağa yönlendirir (Routing)  
3. Eğer paket internet çıkışı ise NAT uygulanır  
4. Hedefe ulaşan paket karşı tarafta doğru cihazı bulur

---

## Özet

- **Routing:** Paketlerin hedefe ulaşmasını sağlar  
- **NAT:** İç IP’leri dış IP’ye çevirir, IP tasarrufu ve güvenlik sağlar  
- Static vs Dynamic Routing, farklı ağ senaryolarında kullanılır  
- PAT, aynı public IP’yi birden fazla cihaz için kullanmayı sağlar
