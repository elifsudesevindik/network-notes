# IP, Subnet ve Gateway İlişkisi

## IP Adresi Nedir?
IP adresi, ağdaki her cihazın birbirini tanımasını sağlayan sayısal kimliktir.  
Bir cihazın ağda veri gönderebilmesi ve alabilmesi için benzersiz bir IP adresine sahip olması gerekir.

Örnek bir IP adresi:
192.168.1.10

---

## Subnet (Alt Ağ) Nedir?
Subnet, bir IP ağının daha küçük parçalara bölünmesidir.  
Bu bölme işlemi ağ trafiğini düzenlemek, performansı artırmak ve yönetimi kolaylaştırmak için yapılır.

Subnet maskesi, IP adresinin hangi kısmının ağ adresi hangi kısmının cihaz adresi olduğunu belirler.

Örnek:
IP: 192.168.1.10  
Mask: 255.255.255.0  

Bu durumda ağ adresi:
192.168.1.0

---

## Gateway Nedir?
Gateway, cihazın kendi ağı dışındaki ağlara ulaşmasını sağlayan çıkış noktasıdır.  
Genellikle bu adres router’ın IP adresidir.

Bir cihaz başka bir ağa veri göndermek istediğinde paketleri gateway’e yollar, gateway de doğru ağa yönlendirir.

Örnek:
Gateway: 192.168.1.1

---

## Üçünün Birlikte Çalışması

Bir cihazın internete çıkabilmesi için üç bilgi gerekir:

- IP adresi → cihazın kimliği
- Subnet maskesi → ağın sınırı
- Gateway → dış ağlara çıkış kapısı

Bu bilgiler olmadan cihaz yalnızca kendi içinde iletişim kurabilir veya hiç iletişim kuramaz.

---

## Gerçek Hayat Örneği

Bir ofiste:

Bilgisayar IP: 192.168.10.25  
Mask: 255.255.255.0  
Gateway: 192.168.10.1  

Bu durumda bilgisayar:
- Aynı ağdaki cihazlarla direkt konuşur
- İnternete gitmek için router’a (gateway) yönlenir

---

## Kısa Özet

IP → cihazın adresi  
Subnet → ağın sınırı  
Gateway → dış dünyaya açılan kapı
