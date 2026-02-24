#  Ağ ve Sistem Terimleri Sözlüğü

## Ağ Temelleri

IP Address: Ağdaki cihazın kimliğini belirleyen sayısal adrestir.  
Public IP / Private IP: Public IP internete açık adres, private IP yerel ağda kullanılan adrestir.  
Subnet: Bir ağın daha küçük parçalara bölünmüş halidir.  
Subnet Mask: IP’nin ağ kısmını ve cihaz kısmını belirleyen maskedir.  
CIDR: IP adreslerini maske ile birlikte kısa yazma yöntemidir (örn: /24).  
Gateway: Cihazın başka ağlara çıkış yaptığı router adresidir.  
DNS: Alan adlarını IP adreslerine çeviren sistemdir.  
DHCP: Cihazlara otomatik IP dağıtan servistir.  
MAC Address: Ağ kartına ait fiziksel donanım adresidir.  
ARP: IP adresinden MAC adresi öğrenmeyi sağlar.  
Broadcast: Ağdaki tüm cihazlara gönderilen veri türüdür.  
Unicast: Tek bir cihaza gönderilen veri türüdür.  
Multicast: Belirli cihaz grubuna gönderilen veri türüdür.  
Packet: Ağda taşınan küçük veri parçasıdır.

---

##  Protokoller

TCP: Güvenilir ve sıralı veri ileten bağlantılı protokoldür.  
UDP: Hızlı ama kontrolsüz veri ileten bağlantısız protokoldür.  
ICMP: Ağ hatalarını ve ping iletişimini sağlayan protokoldür.  
HTTP: Web sayfalarının iletiminde kullanılan protokoldür.  
HTTPS: HTTP’nin şifrelenmiş güvenli versiyonudur.  
FTP: Dosya transferi için kullanılan protokoldür.  
POP3: E-postaları sunucudan indiren protokoldür.  
DNS Protocol: Alan adı sorgularını yöneten iletişim protokolüdür.

---

##  Routing

Routing: Verinin ağlar arasında yönlendirilmesidir.  
Static Routing: Yolların manuel olarak tanımlanmasıdır.  
Dynamic Routing: Routerların otomatik yol öğrenmesidir.  
Routing Table: Router’ın bildiği ağ yolları listesidir.  
Default Route: Bilinmeyen ağlar için kullanılan varsayılan yoldur.  
NAT: Yerel IP’leri tek public IP üzerinden internete çıkarma işlemidir.  
PAT: NAT’ın port bazlı çalışan versiyonudur.  
Port Forwarding: Dış istekleri iç ağdaki belirli cihaza yönlendirmedir.  
Tracert: Paketlerin geçtiği routerları gösteren teşhis komutudur.

---

##  Ağ Donanımı

Router: Ağlar arasında veri yönlendiren cihazdır.  
Switch: Aynı ağdaki cihazları birbirine bağlayan cihazdır.   
Access Point: Kablosuz ağ erişimi sağlayan cihazdır.  
Modem: İnternet hattını dijital ağa çeviren cihazdır.  
Firewall Appliance: Ağ trafiğini filtreleyen güvenlik cihazıdır.  
Patch Panel: Ağ kablolarının düzenli bağlandığı dağıtım panelidir.

---

##  VLAN

VLAN: Ağı mantıksal olarak bölmeye yarayan yapı.  
Access Port: Tek VLAN’a bağlı switch portudur.  
Trunk Port: Birden fazla VLAN taşıyan porttur.  
VLAN ID: VLAN’ın numarasıdır.

---

##  Sistem Temelleri

Server: Ağda hizmet sağlayan bilgisayardır.  
Client: Sunucudan hizmet alan cihazdır.  
Host: Ağda IP’si olan her cihazdır.  
Service: Arka planda çalışan sistem uygulamasıdır.  
Process: İşletim sisteminde çalışan programdır.  
Port: Servislerin iletişim kapısıdır.  
Socket: IP ve port birleşiminden oluşan iletişim noktasıdır.  
Virtual Machine: Sanal olarak çalışan bilgisayardır.  
Hypervisor: Sanal makineleri yöneten yazılımdır.

---

##  Linux

Kernel: İşletim sisteminin çekirdeğidir.  
Shell: Komut yorumlayıcısıdır.  
Terminal: Komut yazılan arayüzdür.  
Directory: Klasör yapısıdır.  
File Permissions: Dosya erişim yetkileridir.  
Root User: Sistem yöneticisi hesabıdır.  
Package Manager: Yazılım kurma aracıdır.  
Repository: Yazılım depolarıdır.  
SSH: Güvenli uzaktan bağlantı protokolüdür.  
Cron: Zamanlanmış görev çalıştırma sistemidir.

---

##  Web ve Domain

Web Server: Web sitelerini yayınlayan yazılımdır.  
Reverse Proxy: İstekleri arka sunuculara yönlendiren ara katmandır.  
Load Balancer: Trafiği sunucular arasında dağıtan sistemdir.  
Virtual Host: Tek sunucuda birden fazla site çalıştırma yöntemidir.  
SSL/TLS: Veri şifreleme protokolleridir.  
Certificate: Güvenli bağlantıyı doğrulayan dijital belgedir.  
Domain: Web adresidir.  
Subdomain: Ana domainin alt adresidir.  
DNS Record: Alan adı yönlendirme kayıtlarıdır.

---

##  Kurumsal Sistemler

Active Directory: Merkezi kullanıcı yönetim sistemidir.  
Domain Controller: AD verisini yöneten sunucudur.  
Group Policy: Bilgisayar ayarlarını merkezi yönetme aracıdır.  
LDAP: Dizin sorgulama protokolüdür.  
Authentication: Kullanıcı doğrulama işlemidir.  
Authorization: Kullanıcı yetkilendirme işlemidir.

---

##  Güvenlik

Firewall: Ağa gelen trafiği filtreleyen güvenlik sistemidir.  
IDS: Saldırıları tespit eden sistemdir.  
IPS: Saldırıları engelleyen sistemdir.  
SIEM: Log analiz edip tehdit tespit eden platformdur.  
DLP: Veri sızıntısını önleyen sistemdir.  
VPN: Güvenli tünel bağlantısıdır.  
Encryption: Veriyi şifreleme işlemidir.  
Hashing: Veriyi geri döndürülemez özet haline getirmedir.  
Brute Force: Şifre deneme saldırısıdır.  
Phishing: Sahte içerikle bilgi çalma yöntemidir.  
Malware: Zararlı yazılımdır.  
Exploit: Güvenlik açığını kullanan saldırı kodudur.

---

##  İzleme

Network Monitoring: Ağın sürekli izlenmesidir.  
Logging: Olay kayıtlarının tutulmasıdır.  
Alerting: Kritik durumlarda uyarı üretmedir.  
Metrics: Sistem performans verileridir.  
Dashboard: İzleme ekranıdır.  
Uptime: Sistem çalışma süresidir.  
Availability: Sistemin erişilebilirlik oranıdır.

---

##  Donanım

CPU: İşlem yapan ana donanım birimidir.  
RAM: Geçici veri belleğidir.  
Cache: Hızlı ara bellek alanıdır.  
SSD: Flash tabanlı hızlı depolama birimidir.  
NVMe: SSD’lerin yüksek hızlı bağlantı standardıdır.
