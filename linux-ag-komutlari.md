# Temel Linux Ağ Komutları

## ping

Bir cihaza erişim olup olmadığını kontrol eder.

```
ping 8.8.8.8
```

---

## traceroute

Paketin geçtiği yolları gösterir.

```
traceroute google.com
```

---

## ip addr

IP adres bilgilerini gösterir.

```
ip addr
```

---

## netstat

Açık portları ve bağlantıları listeler.

```
netstat -tuln
```

---

## ss

Netstat’ın daha hızlı versiyonudur.

```
ss -tuln
```

---

## nslookup

DNS sorgusu yapar.

```
nslookup google.com
```

---

## curl

Web isteği gönderir.

```
curl http://example.com
```

---

## Özet

- ping → bağlantı kontrol  
- traceroute → yol analizi  
- ip addr → IP bilgisi  
- netstat / ss → port kontrol  
