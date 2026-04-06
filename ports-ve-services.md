# Portlar ve Yaygın Servisler

## Port Nedir?

Port, bir cihazda çalışan servislerin dış dünya ile iletişim kurduğu **mantıksal kapıdır**.

Bir IP adresi cihazı temsil ederken, port numarası o cihazdaki **hangi servise gidileceğini** belirler.

Örnek:

- 192.168.1.10 → cihaz
- :80 → web servisi

Yani:
```
192.168.1.10:80
```
→ Bu adres, o cihazdaki web sunucusunu ifade eder.

---

## Port Türleri

### Well-Known Ports (0 – 1023)

- Standart servisler için ayrılmıştır
- En çok kullanılan portlardır

### Registered Ports (1024 – 49151)

- Uygulamalar için ayrılmıştır

### Dynamic / Private Ports (49152 – 65535)

- Geçici bağlantılar için kullanılır

---

## Yaygın Portlar ve Servisler

| Port | Protokol | Açıklama |
|------|----------|---------|
| 20-21 | FTP | Dosya transferi |
| 22 | SSH | Güvenli uzaktan bağlantı |
| 23 | Telnet | Güvensiz uzaktan bağlantı |
| 25 | SMTP | E-posta gönderme |
| 53 | DNS | Alan adı çözümleme |
| 67-68 | DHCP | Otomatik IP dağıtımı |
| 69 | TFTP | Basit dosya transferi |
| 80 | HTTP | Web trafiği |
| 110 | POP3 | E-posta alma |
| 143 | IMAP | E-posta yönetimi |
| 161 | SNMP | Ağ yönetimi |
| 179 | BGP | Routerlar arası yönlendirme |
| 389 | LDAP | Dizin servisi |
| 443 | HTTPS | Güvenli web trafiği |
| 445 | SMB | Windows dosya paylaşımı |
| 3389 | RDP | Uzak masaüstü |

---

## TCP ve UDP Port Kullanımı

- Bazı portlar **TCP** kullanır (HTTP, HTTPS, SSH)
- Bazıları **UDP** kullanır (DNS, DHCP)
- Bazıları her ikisini de kullanabilir

---

## Port Neden Önemlidir?

- Servislerin çalıştığı noktayı belirler  
- Güvenlikte kritik rol oynar  
- Açık portlar saldırı yüzeyini artırır  

Örnek:

- Açık 22 → SSH saldırılarına açık olabilir  
- Açık 80 → Web sunucusu çalışıyor demektir  

---

## Güvenlik Açısından Portlar

- Gereksiz portlar kapatılmalıdır  
- Firewall ile port erişimi kontrol edilir  
- Açık portlar saldırganlar tarafından taranır (Nmap gibi araçlarla)

---

## Özet

- Port → servise açılan kapıdır  
- IP + Port → hedef servisi belirler  
- Well-known portlar en yaygın servisleri içerir  
- Açık portlar güvenlik açısından dikkat edilmesi gereken noktalardır
