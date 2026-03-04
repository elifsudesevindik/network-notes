# DNS ve DHCP

## DNS (Domain Name System)

DNS, **alan adlarını IP adresine çeviren sistemdir**.  
İnternete her siteyi IP ile bulmak zor olurdu, DNS sayesinde `www.google.com` gibi isimleri kullanabiliyoruz.

Özellikleri:

- Alan adı → IP adresi çevirir  
- Hiyerarşik bir yapı vardır (root, TLD, authoritative server)  
- Web sitelerine hızlı erişim sağlar  

Örnek:

- `www.stajnotlari.com` → `192.168.1.10`  

DNS türleri:

- **A kaydı:** Alan adını IPv4 adresine çevirir  
- **AAAA kaydı:** Alan adını IPv6 adresine çevirir  
- **CNAME:** Alan adını başka bir alan adına yönlendirir  
- **MX:** E-posta sunucusu kaydı  

---

## DHCP (Dynamic Host Configuration Protocol)

DHCP, **cihazlara otomatik IP dağıtan servistir**.  
Bu sayede her cihaz için manuel IP ayarlamaya gerek kalmaz.

Özellikleri:

- IP, subnet mask ve gateway verir  
- Kiralama (lease) süresi vardır  
- DHCP server ile cihaz (client) iletişim kurar  

Çalışma Adımları (DORA):

1. **Discover:** Cihaz ağda DHCP server arar  
2. **Offer:** Server uygun IP’yi teklif eder  
3. **Request:** Cihaz teklifi kabul eder  
4. **Acknowledge:** Server IP’yi atar ve onaylar  

Örnek:

- IP Address: 192.168.1.25  
- Subnet Mask: 255.255.255.0  
- Gateway: 192.168.1.1  
- DNS Server: 192.168.1.2  

---

## DNS ve DHCP Birlikte Çalışması

- DHCP ile cihaz IP alır  
- DNS ile cihaz web sitelerine isimle erişir  
- Her ikisi de ağın düzgün çalışması için kritik öneme sahiptir  

---

## Özet

- **DNS:** Alan adı ↔ IP çevirir  
- **DHCP:** Cihazlara otomatik IP verir  
- DNS ve DHCP olmadan ağ yönetimi çok zor olur
