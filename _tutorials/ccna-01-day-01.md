---
layout: tutorial
title: "CCNA Gün 1 - Ağ Cihazları"
course: ccna
order: 1
excerpt: "CCNA networking devices: networks, nodes, clients, servers, switches, routers, and firewalls."
permalink: /tutorials/ccna/day-01/
---

Yazı İçeriği

1. [Network Nedir?](#Network_Nedir)[Düğüm (Node) Nedir?](#D___m__Node__Nedir)[Client](#Client)[Server](#Server)
2. [Switch](#Switch)
3. [Router](#Router)
4. [Firewall](#Firewall)

Bu Yazıda Modern Ağlarda Kullanılan Cihaz Türleri, Ağdaki İşlevleri ve Farklılıkları Hakkında Bilgi Edineceğiz.

## Network Nedir?

Network'ün Wikipedia'daki Tanımına Bakalım:

**A Computer Network is a Digital Telecommunications Network Which Allows Nodes to Share Resources.**

**Bir Bilgisayar Ağı, Düğümlerin Kaynaklarını Paylaşmasına İzin Veren Bir Dijital Telekomünikasyon Ağıdır.**

### Düğüm (Node) Nedir?

![Bilgisayar Ağlarında Düğüm Nedir? (What is Node in Computer Network?)]({{ '/assets/images/tutorials/ccna/day-01/image-01.jpg' | relative_url }})

Router, Switch, Firewall, Server, Client, vb.

Şimdi En Basit Haliyle Bir Network Kuralım. Client ve Server'ın Tanımlarını Yapalım.

### Client

Server Tarafından Sağlanan Bir Hizmete Erişen Cihazdır.

### Server

Client için Fonksiyonlar veya Hizmetler Sağlayan Cihazdır.

Server ve Client'e **End Host** veya **Endpoint** de Denilmektedir.

Şimdi İki Bilgisayarı Birbirine Bir Kablo ile Bağladığımızı Düşünelim.

![İstemci/Sunucu Modeli (Client/Server Model)]({{ '/assets/images/tutorials/ccna/day-01/image-02.jpg' | relative_url }})

PC1, PC2'den Bir Resim İstedi. PC2 ise PC1'e Resmi Gönderdi. Bu Durumda PC1 Client, PC2 ise Server Olur. İşte Bu Çok Basit Bir Network Örneğidir. Ayrıca Buradaki Yapıya Client-Server Modeli / Mimarisi Denilmektedir.

İşte Başka Bir Network Örneği:

![İstemci/Sunucu Modeli (Client/Server Model)]({{ '/assets/images/tutorials/ccna/day-01/image-03.jpg' | relative_url }})

Burada Önceki Network Örneğinden Farklı Olarak Bilgisayarımız ile YouTube Server'ı Arasında İnternet Var. İnternetin Bir Bulut Resmi ile Temsil Edildiğine Dikkat Edin. Şuan için İnternetin İçinde Neler Olduğunu Bilmemize Gerek Yok. İlerleyen Konularda Kolaydan Zora Doğru Öğreneceğiz.

**Önemli Bilgi:** Aynı Cihaz Bazı Durumlarda Client, Bazı Durumlarda Server Olabilir.

## Switch

- Hostların Bağlanabileceği Çok Sayıda Porta Sahiptir (Genellikle +24).
- Aynı LAN (Local Area Network) İçindeki Hostlar Arasında Bağlantı Sağlar.
- LAN'lar Arasında İnternet Üzerinden Bağlantı **Sağlamaz.**

Bir Şirketin Birden Çok Şubesi Olduğunu Düşünün. Şubelerin Her Birini Bir LAN Olarak Düşünebilirsiniz. LAN İçindeki Hostların Birbirleri ile Haberleşebilmesi için Switch'e İhtiyaç Vardır. Bu Arada Switch'den Önce LAN'da Hub ve Bridge Kullanılıyordu, Ama Bunlar Artık Eskide Kaldı :)

Switch LAN'ları Birbirine Bağlamaz. Bu İşi Bir Sonraki Bölümde Anlatacağımız **Router** Yapar. Örnek Olarak Şirketin İki LAN'ını Birbirine Bağlamak İstiyorsak Bu İşi Sadece Switch ile Yapamayız, Router'a İhtiyacımız Olacaktır.

![What is a Switch? LAN (Local Area Network)]({{ '/assets/images/tutorials/ccna/day-01/image-04.jpg' | relative_url }})

Yukarıdaki Resimde Bir Şirketin New York ve Tokyo Olmak Üzere İki Şubesi Görülmekte. New York Şubesindeki Hostların Switch 1'e Bağlandığına Dikkat Edin. Böylece Birbirleri ile Haberleşebilecekler. Aynısı Tokyo Şubesi için de Geçerli. Bu İki Şube de Bir LAN'dır.

Switch, Doğrudan İnternete Bağlanamaz.

Bazı Cisco Switch Modelleri:

![Örnek Cisco Switch Modelleri (Example Cisco Switch Models)]({{ '/assets/images/tutorials/ccna/day-01/image-05.jpg' | relative_url }})

Cisco Catalyst 9200, Cisco Catalyst 3650, Cisco Catalyst 2960, ...

## Router

- Switch'den Daha Az Porta Sahiptir.
- LAN'lar Arasında Bağlantı Sağlamak için Kullanılır.
- İnternet Üzerinden Veri Göndermek için Kullanılır.

Switch Bölümünde Bir Şirketin İki Şubesinden Bahsetmiştik. Bu Şubeler İnternet Üzerinden Birbirleri ile İletişim Kurmak İstiyorsa Router Kullanmaları Gerekir.

![Router Nedir? LAN'lar Arası Haberleşme (What is a Router? Communication Between LANs)]({{ '/assets/images/tutorials/ccna/day-01/image-06.jpg' | relative_url }})

New York Şubesindeki PC1, Tokyo Şubesindeki SRV1'e Ulaşmak İstiyor. İlk Resimde Mavi Oklar ile Gidilen Yolu Görüyorsunuz. SRV1'in Cevabı ise İkinci Resimde Kırmızı Oklarla Belirtilmiştir, Gelen Yolun Tam Tersi.

Bazı Cisco Router Modelleri:

![Örnek Cisco Router Modelleri (Example Cisco Router Models)]({{ '/assets/images/tutorials/ccna/day-01/image-07.jpg' | relative_url }})

## Firewall

Firewall, Network'e Giren ve Çıkan Trafiği Kontrol Eden Özel Güvenlik Cihazlarıdır.

![Firewall Nedir? Örnek Firewall Topolojisi (What is a Firewall? Example Firewall Topology)]({{ '/assets/images/tutorials/ccna/day-01/image-08.jpg' | relative_url }})

Firewall, FW1 Gibi Router'ın **Outside** veya FW2 Gibi **Inside** Tarafına Yerleştirilebilir. Önemli Olan Bu Ağdaki PC'ler ve Server'lar Gibi İçerideki Hostların Korunmasıdır.

Hangi Ağ Trafiğine İzin Verileceğini ve Hangilerinin Reddedileceğini Belirlemek için Firewall, Güvenlik Kuralları ile Yapılandırılır. Kuralları Doğru Yapılandırırsanız PC1, SRV1'e Erişebilmelidir. SRV1'den PC1'e Dönüş Trafiğine de İzin Verilmelidir. Ancak Saldırgan Ağlarımız İçindeki Herhangi Bir Şeye Erişmeye Çalışırsa, Firewall Bunu Engellemelidir.

Bazı Cisco Firewall Modelleri:

![Örnek Cisco Firewall Modelleri (Example Cisco Firewall Models)]({{ '/assets/images/tutorials/ccna/day-01/image-09.jpg' | relative_url }})

IPS (Intrusion Prevention System) ve Daha Detaylı Filtreleme Gibi Özelliklere Sahip Firewall'lar, **Next Generation Firewall** Olarak Adlandırılır.

Cisco ASA 5500-X ve Cisco Firepower 2100, Next Generation Firewall'dır.

Özetle Firewall...

- Yapılandırılmış Kurallara Bağlı Olarak Ağ Trafiğini İzler ve Kontrol Eder.
- Firewall, Trafiği Router'a Ulaşmadan Önce veya Router'dan Geçtikten Sonra Filtreleyebilir. Bazı Durumlarda Ağın İçinde ve Dışında Firewall Olabilir.
- Firewall, Daha Modern ve Kullanışlı Özelliklere Sahip Olduğunda Next Generation Firewall Olarak Bilinir.

Peki Bilgisayarımızdaki Firewall Ne Olacak? Firewall'ın İki Türü Vardır:

- **Network Firewall (Cisco ASA ve Cisco Firepower)**
- **Host-Based Firewall**

**CCNA Sınavı İlgili Bir Not:** Bazı Sorularda Doğru Olabilecek Birden Fazla Cevap Olabilir, Ancak Her Zaman Biri En İyi Seçenek Olacaktır. Cisco Sınavlarında Bunun Gibi Pek Çok Soru Vardır.

**Quizs**

**![CCNA Gün 1 Quiz (CCNA Day 1 Quiz)]({{ '/assets/images/tutorials/ccna/day-01/image-10.jpg' | relative_url }})**

**Cevaplar (Sırası ile):**

- c
- a
- c
- d
- c

[LAB](https://drive.google.com/file/d/1LFUwjUziqoI8USzLMfkjx6vuMQRdTd7b/view?usp=drive_link) - [ANKI](https://drive.google.com/file/d/1VfkbBFeC5ga3wXQvFZi55CcpnD-HgD-G/view?usp=drive_link)

Bu Konu CCNA Eğitiminin İlk Dersi Olduğu için Packet Tracer Simulator Programı ile LAB Yapabilmeniz için Aşağıdaki Videoyu İzlemenizi Tavsiye Ediyorum. Video YouTube Üzerinde Olduğu için Altyazıyı Aktif Edin ve Otomatik Çevir Özelliğinden Türkçe Seçin.

Okuduğunuz için Teşekkürler.
