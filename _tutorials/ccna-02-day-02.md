---
layout: tutorial
title: "CCNA Gün 2 - Network Cihaz Arayüzleri, Portları ve Kablolar"
course: ccna
order: 2
excerpt: "Network interfaces, Ethernet, RJ45, UTP, fiber optics, and cable standards."
permalink: /tutorials/ccna/day-02/
---

Yazı İçeriği

1. [RJ45](#RJ45)
2. [Ethernet](#Ethernet)[Bit/Byte](#Bit_Byte)[Ethernet Standartları](#Ethernet_Standartlar)
3. [UTP Kablo](#UTP_Kablo)[UTP Kablo (10BASE-T, 100BASE-T)](#UTP_Kablo__10BASE_T__100BASE_T)[Straight-Through Cable](#Straight_Through_Cable)[Crossover Cable](#Crossover_Cable)[UTP Kablo (1000BASE-T, 10GBASE-T)](#UTP_Kablo__1000BASE_T__10GBASE_T)
4. [Fiber-Optik Kablo](#Fiber_Optik_Kablo)[SFP Transceiver](#SFP_Transceiver)[Fiber-Optik Kablo Yapısı](#Fiber_Optik_Kablo_Yap_s)[Fiber-Optik Kablo Türleri](#Fiber_Optik_Kablo_T_rleri)[Multimode Fiber](#Multimode_Fiber)[Single Mode Fiber](#Single_Mode_Fiber)[Fiber-Optik Kablo Standartları](#Fiber_Optik_Kablo_Standartlar)
5. [UTP ve Fiber Optik Kablo Karşılaştırması](#UTP_ve_Fiber_Optik_Kablo_Kar__la_t_rmas)

![]({{ '/assets/images/tutorials/ccna/day-02/image-01.jpg' | relative_url }})

Bu Yazıda Cihazları Birbirine Bağlamak için Kullanılan Portlar ve Kablo Türleri Hakkında Bilgi Edineceğiz.

### RJ45

İlk Olarak Switch Cihazının Portlarını İnceleyelim.

[![switch ports example]({{ '/assets/images/tutorials/ccna/day-02/image-02.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgV4EoOUAiizZXaXh0DPorNR2LBzWFSeQNNry8yC9r-_GXhZQPYWJ8tz05ehP4ICebdASqFJi_xvTjtw0OTtQUOnktycDKTq7_hHKhLPxfqQFXbr2OXXaYaDUALW1BfZK33QeMbeqVml2cNxzUEcSC_EwHrWSCJ4QLE69nNkEiJiR0zk33o0Qv2v73Y/s1472/switch-ports-example.webp)

Yukarıdaki Switch'in 24 Portu Vardır. Switch, Hostları LAN'a Bağladığı için Port Sayısı Fazladır.

Portların Üzerinde *10/100/1000Base-T Ports (1 - 24) - Ports are Auto-MDIX* Gibi Bilgiler Yazmakta. Bu Bilgiler Portun Özelliklerini Belirtir.

Bir Host, Kablolu Ağa Bağlanmak için Mutlaka Yukarıdaki Gibi Bir Port Kullanıyordur. Bunlara **RJ-45 Port** Denir.

RJ-45 Konnektörüne Bakalım.

[![rj45 konnektörü]({{ '/assets/images/tutorials/ccna/day-02/image-03.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEg-PqztKP_U-W_zXYB0hi_X6p75o-keOU3h4-C2YUrxKg2TfLXMMqIfDYIFuC6r-wqihtTevG4ZbCoFr64sLkoaLX5sU2Mc31rL7g225uz1WEUF07D1oWD3PPd-e0uflB1NBRIW-7X1GpORh_FC6uYbYjqBlW10-SOecj0L6_vLjphT42aEduCy7kSCjw/s569/rj45-konnektor.jpg)

RJ-45 Konnektörü, Bakır Ethernet Kablosunun Uçlarında Kullanılır.

### Ethernet

**Ethernet,** Genellikle Yerel Alan Ağlarındaki (LAN) Cihazları Birbirine Bağlamak için Kullanılan Standart Bir İletişim Protokolüdür.

Bu Yazıda Ethernet Protokolünde Tanımlanan Kablolama Türlerine Odaklanacağız.

#### Bit/Byte

[![bit byte dönüşümü]({{ '/assets/images/tutorials/ccna/day-02/image-04.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEg5DZJjHDvXJg3AJ0WPHvtoWkLX9vMCX35vtMuoNgyyIY0Xa5fA7vJwnoj7I7o5HkKCFLUZDbB-yi6-XYkg7nmw6Lhj4Q9cTR3oVtGW_rBCbV5OG1JOLpaj2uGMrTDvgzejcaIabupxaxc91NBh1_dfMp0ZNk3pMblVYXeS1rACgv_a7syygGQkAzeDNw/s464/bit-byte-donusumu.jpg)

Ağdaki Cihazlar Arasındaki Bağlantılar Belirli Bir Hızda Çalışır.

**Hız (Speed),** ***Bits Per Second*** (Kbps, Mbps, Gbps, ..) Cinsinden Ölçülür.

[![ağ hız birimleri bit per second]({{ '/assets/images/tutorials/ccna/day-02/image-05.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgndXcURF7i7w7QGhQYrSQVZrWsIuCwUQJFwUlajEyU6dNTXN7hrNHWKPxzAk1_04afnvG2QTJh7JoMCMUzIQiZffHpH63sUYJFG7jAjZzcKg2hz9ruJzvrIHgcv-P3Vz9bCh2xaz4HCeIpr09gCGa2tBnUs5LQv5PL60lGtK3WwUW53Kh34lmQZelovA/s481/bit-per-second-network.jpg)

#### Ethernet Standartları

**Ethernet**Standartları **IEEE 802.3** Tarafından Belirlenmektedir.  
**IEEE**Açılımı: Instute of Electrical and Electronics Engineers.

[![ethernet standartları]({{ '/assets/images/tutorials/ccna/day-02/image-06.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjHr7k4PkulOswZH39px9R6zmqGp86kY5cJpV7euqLhNIqWCd7Rcu8QFQFbW-8gz62zfMJFSIBj2kvduiPoCQ9MSo0Q6dWhbNc0kennwzt_WAnYmIAzr3J2tKbvBd6iU4q-BQuKN78pdnEaqMjiWu5IOQnuMk1OzNkHAwuY69pWSEMF5PUoPEk4ppVbgQ/s634/ethernet-standartlari.jpg)

### UTP Kablo

[![utp kablosu]({{ '/assets/images/tutorials/ccna/day-02/image-07.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhfgf4mq_w2GGTDGzah5cCW28FRwOWQFxmCUOmyGV4pBYSowKOv2ERKTKOEgzDG1Su3Qqpgol91-2nlcRbnxukI1iaeKXLV8UdqLE8x1g8z1YO-PTcu5tapcp8wLAAsTuj2eFj9s-5SXV_zp_SskUxrNhAEalQsZionwx67X9gucv8SL33bHjcGHCR3PQ/s681/utp-kablo.jpg)

**UTP**Açılımı: **U**nshielded **T**wisted **P**air.

Unshielded, Kablo İçindeki Tellerin Metalik Bir Kalkana Sahip Olmadığı Anlamına Gelir. Bu Durum Kablonun

**Elektromanyetik Parazite (Electromagnetic Interference - EMI)**

Karşı Savunmasızlığını Arttırır.

Kablonun İçinde Birlikte Bükülmüş Dört Çift Vardır, Bu da Toplamda Sekiz Tel Yapar. **Bükümlü Çiftler (Twisted Pair),** Elektromanyetik Parazite (EMI) Karşı Korumaya Yardımcı Olur.

RJ-45 Konnektöründe 8 Pin Vardır.

[![rj45 konnektörü pin]({{ '/assets/images/tutorials/ccna/day-02/image-08.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgaKds5XZBjC1AtMrDHqd7QSnlRMwfa2stQ4j8QskNs91N4In27xM9rRThnsXv8N1gMm5BDeHtgF5NldyLlvDXbjkbUW99bAydBtdjPPhW_yVy08E0i9ZmWl6xSc629fsCOSATW235O6MugXxU6m3N5Q-3sF3nlwE9dhYL29kY6Y6nzef9TGm2HtFDXlw/s390/rj45-konnektor-pin.jpg)

Daha Önce Gördüğümüz Ethernet Standartlarının Tümü Aslında 8 Pinin / Telin Tümünü Kullanmaz.

[![ethernet standartları kablo çift ve tel kullanımı]({{ '/assets/images/tutorials/ccna/day-02/image-09.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjsG3GiQVNMd7rYAoDeAf_cl2xOTVyB2nlxxA4Mfd_rUKeLQ2jYSnqJeFsl63Yxx1_Iubsnr9Z2pSzLgK1e5kciTiW3G8XJit_zwVtp1Wyq9_i63BUfNWSHFksJZN7tIevbTLhXKQuF6rVJ2Djqir3tPKFCzns_fDno_G85cLjWPA-kThOepMgjAC3eIQ/s378/ethernet-standart-tel-ve-cift-kullanimi.jpg)

#### UTP Kablo (10BASE-T, 100BASE-T)

Bir Hostu FastEthernet Bağlantısı Olan Bir Switch'e Bağladığımızı Düşünelim.

[![]({{ '/assets/images/tutorials/ccna/day-02/image-10.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhovb3YNrSCCFc6zGoqYTjkxSpkRB2SJ2DhmRTzgSacnt1mokwW5Jawsy0pdfbGApjbKbRsG7KSdR88By6c7PCVtscP1kfn-wmYW5nncXQhoifCWDk8U1Dmog0ui_k3I6PL7YUD-EGn_7F8cfou59HhyZz15ojXXSosvpCRL-Tt1xsxo2W5BnVuknTePA/s695/resim1.jpg)

Bu Numaralar, Hostun **Network Interface Card (NIC)** ve Switch RJ-45 Portu Üzerindeki Pinleri Temsil Eder. 8 Adet Tel var, 10BASE-T ve 100BASE-T için 2 Çift (Pair) / 4 Tel (Wire) Kullanılır.

Host, Switch'e Veri İletmek için **TX** Olarak Yazabileceğimiz Pin 1 ve 2'yi Kullanacaktır. Host, Pin 1 ve 2 Üzerinden Veri İlettiği için Switch O Pinler Üzerinden Veri İletemez. Switch, **RX** Olarak Yazabileceğimiz 1 ve 2 Pinlerinden Verileri Alması Gerekir. Kısaca; Host NIC, 1 ve 2 Numaralı Pinlerden Verileri İletir ve Switch'deki Port, 1 ve 2 Numaralı Pinlerden Verileri Alır.

Bu Şemada Teller Düz Görünse de, Bir UTP Kablosunda Çiftlerin Birlikte Büküldüğünü Unutmayın.

[![]({{ '/assets/images/tutorials/ccna/day-02/image-11.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhQU3YKGoTMUAef0ZSUJAPx0CobhVziGKBoGBi7DxrjXSMqISuuRh9jlqRcC9OvMlJaoQYGO6MFDqIwAMBBU7CRAJmplmdT3Sdke7m0K-h7BZL7PhFl9kdXa5mDT-V5cL6A8Pipg-8aHV63tIQx8X7L8Dv0ivcx1uvfPoYxm4oBmyALIos4XMAATHGxNQ/s690/resim2.jpg)

Sonraki Çift, 3 ve 6'dır ve 1 ve 2 Çiftinin Tersi İşlem Yapar.

Switch, Veri İletmek için Pin 3 ve 6 Kullanır ve Host 3 ve 6 Pinlerden Veri Alır. Bu, **Full-Duplex** Denilen Şeye İzin Verir.

**Full-Duplex;** Cihazların Aynı Anda Hem Veri Göndermesi, Hem de Veri Alması Anlamına Gelir. Veri İletmek ve Almak için Ayrı Tel Çiftleri Kullandıklarından **Çarpışma (Collision)** Gibi Sorunlar Olmaz.

[![full duplex]({{ '/assets/images/tutorials/ccna/day-02/image-12.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjOiOrB6l4mbIsCEWOxVBXfI0Rfmb1pHKl0KIx61HZtHrMYO-UJPW9un3QQTaCLdVPFHpTxEgwsUf5Sy7lM_dJtsynTMRc1RVb81YrZvexEGyLUE1RoH8O2Aqtj9x9oYNH-HX7BBGjxB8HCFfzSC7Op3FEz91YACOV1psvVgy0_86A7hWZj0ZJcFjwAUw/s693/resim3.jpg)

Resmin Sol Tarafında PC, Router, Wireless Access Point, Firewall Bulunabilir. Sağ Tarafta ise Switch, Hub Bulunabilir.

##### Straight-Through Cable

Kablonun Bir Ucundaki Bir Pin, Diğer Uçtaki Aynı Pine Doğrudan Bağlanır (Örnek: Pin 1 - Pin 1, Pin 2 - Pin 2, ..).

Yukarıdaki Resimde Sağ Taraftaki Switch Yerine Router Koyarsak Ne Olur? Router-Router, Switch-Switch, PC-Router, PC-PC, vb. Durumları Düşünelim.

[![]({{ '/assets/images/tutorials/ccna/day-02/image-13.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEh2PysXePess5XY_YaLjAp9OQX7q3g2Y_568A228tz1oVzKeH0BET5P0EADZ7fDlJqozewB8QcxojUBCV3zk5UB58GZNwRqdBi12DYGqFesmszGiONCi3rE3fuoH2jpgFG-WkWYBMJel3gvdawq__gfY3nkDVx3_99pQLcemqjgzrsk9BL5t4EC_fV9hQ/s683/resim4.jpg)

**Straight-Through Cable** Kullanırsak Sağ Taraftaki Router 1 ve 2 Pinlerinden Veri Alamayacaktır, Bu Nedenle İki Router Arasında İletişim Gerçekleşmez. Aynı Şey İki Switch Arasında da Geçerlidir.

[![]({{ '/assets/images/tutorials/ccna/day-02/image-14.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEg_V60cdd7w5BdzNG2lCHs89ewbvrUqXBYoqcP_0XYKHWG3LPR-5xcqfgHdEBcX9rfQ9SSVZ4p-shSzXfeJKYed6zfu52bdhUza82Sh9ku9XCPeZTuOpATWh_LLYP3JCKV6rC5xnJUv927lEon7nij007UbB4IF0EyaSjljj7eZdzi7byj2a_Hfqo-HQQ/s691/resim5.jpg)

##### Crossover Cable

Kablonun Bir Ucundaki Pin, Diğer Uçtaki Aynı Pine Doğrudan **Bağlanmaz.**

[![çapraz kablo (crossover cable)]({{ '/assets/images/tutorials/ccna/day-02/image-15.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgeGi-YpvcY71AsZeTZRLUiwqCdljcoIryg5ss98HN7bPUmHtqvTL0WENEqaMoymaH9s8L_LvGMKeBhNSzZjDC9zItRWK9yv_NP3Cy0zLfsFRLLcuEae4we5l7GCE2wb1e9HAXTVSUciooV1SoWqctYrL3F27t6N0U2ITQzo7vrCz-hyhh8kxqS5-RbwA/s694/%C3%A7apraz-kablo.jpg)

Bir Taraftaki TX Pinleri, Diğer Taraftaki RX Pinlerine Bağlıdır. Bu Sayede Artık İki Cihaz Birbirine Veri Gönderebilir.

[![çapraz kablo (crossover cable)]({{ '/assets/images/tutorials/ccna/day-02/image-16.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEili6hieG3WrgA1iz6NpWLnwgJ4NGl-Q_F87KR2S6ROWvH3RQkVN_hjGuiUS3GLfIh5sMbOI09KEfLhw_nHIoejGtgSf8wiDUEyUOBrxOyIyO9Qbl__VPBe5AljsIdWEUvFYnrYO01VX69chCIJDl1BC9_2Tdy-R0oMf_aTopXVK0408fWgmhb3KkY6Sg/s720/crossover-cable.jpg)

Cihazların Veri Göndermek ve Almak için Hangi Pinleri Kullandığına Dair Özet Bir Tablo:

[![]({{ '/assets/images/tutorials/ccna/day-02/image-17.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEheoVzUPKLm7o1SwUiMLIaqcygsf-TDsifpsbVqaTCKbDiTInwsoAqTDvfjLM8s1aAtHxJMeeoA2G_g0G3Bq731T6DzZiI-a9M0y8wmeChsUziS70rgsoVchK33HlFYYJ6-L-tpCVPYANgeve94WC9Hu1Yb4r2d2mHJVC8JleaDNfUtmyWS5gs6Fd6ZPg/s582/resim5.jpg)

Günümüzde Çoğu Modern Ağ Cihazı, Straight Through Cable ve Crossover Cable Hakkında Endişelenmenin Ötesine Geçmiştir. Bunun Nedeni Modern Ağ Cihazlarının **Auto MDI-X** Özelliği İçermesidir.

**Auto MDI-X**Nedir?****Cihazların Komşularının Hangi Pinlerden Veri İlettiğini Otomatik Olarak Algılamasına ve Ardından Veri İletmek ve Almak için Hangi Pinleri Kullanacaklarını Ayarlamasına İzin Verir. Daha Sonra Normal Şekilde Veri Alışverişi Yapabilirler.

#### UTP Kablo (1000BASE-T, 10GBASE-T)

1000BASE-T ve 10GBASE-T için 4 Çift (Pair) / 8 Tel (Wire) Kullanılır.

[![]({{ '/assets/images/tutorials/ccna/day-02/image-18.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjgA-KnVPXSqam81kMwq8VAnJajd84S1FzenWThD_6vyTgU1IJ6m7AnTgTuZVvb2CiJte8PPxf7Jf97OInO4a8DupH8uGY_leaHeEnPvSLXQq8CkuVDLaTSNt1zrdBMR7Ckf75yCpc8bLrPCgVkFNPJ-4V16mtZ1EPVZdF8TKkhz0dd3CQE6_-t2Dtuiw/s694/resim6.jpg)

Pin 1 ve 2, Pin 3 ve 6, Pin 4 ve 5, Pin 7 ve 8 Kullanılır.

Her Bir Çift Veri Alma ve Veri Gönderme için Özel Değildir. Her Bir Çift Hem Veri Alıp, Hem Gönderebilir. Bu, Çok Daha Yüksek Hızlarda Çalışabilmelerinin Bir Nedenidir.

### Fiber-Optik Kablo

[![]({{ '/assets/images/tutorials/ccna/day-02/image-19.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhePchXqpyh3pvPQGPjq7z9dEM8XSBLMJfC-vpe8lf4CsFlRjNy1LlE5j9m62FPpacIpUM3hOxZg3zI7CsWkcvMi_1UJXhAcGmf49EaeNBYcTr3whIDEAWVz-MhoS8rrw3uMoYct0nKi3fYBdygBB2om8NqLS6CI02tNxQphzWX4JWClhCN8hgUH0btBA/s531/resim7.jpg)

Üstekki Cihaz Bir Cisco Switch, Alttaki Cihaz ise Cisco Router'dır. Sarı Alan UTP RJ-45 Portlarını Temsil Eder.

#### SFP Transceiver

[![fiber optik kablo sfp]({{ '/assets/images/tutorials/ccna/day-02/image-20.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhUwlInnhh-7_BOZ2fE7LAwp-IitxKuiK1AoDlghMjaU4KK6XsRnL8YNys7d4w54UoPi5FdSNSBqxd1WPpB5N2Ouf9BX-4_HoPUK_uKyGWgO8yMRScZGimyvGRI9f0k9Pol9HHj71YP_RnjUWQiApPiAQg6QIwAsPW76eFTznSaknVCpNj0LP7TbS-cGw/s378/fiber-optik-kablo-sfp.jpg)

**SFP Transceiver,** Router veya Switch'lerin Fiber Portlarına Takılır (Kırmızı Alan).

**SFP**Açılımı: Small Form-Factor Pluggable.

Peki **SFP'lere** Ne Tür Bir Kablo Bağlanır?

[![fiber optik kablo]({{ '/assets/images/tutorials/ccna/day-02/image-21.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEi_08STf8CRdf1iDJU7tPXj_YuUjox3DJXs3J6uyei2w8Ex5Yj9oa2nxaU6unT-A-MJP-ElNzP-BFuHMbLeBgrM7cucE7zVyeUuBrw7ojdPywo1-nlRhL-9NA5-0D2rYoWjt6v2o0kAW639gjnTmTbFqaJsw6gwSxi4kfLi5oieJvMegY8p1R5nsJ_vbw/s425/fiber-optik-kablo.jpg)

Bu Bir **Fiber-Optik Kablodur.**  Bakır Kablo Üzerinden Bir Elektrik Sinyali Yerine, Bu Kablolar Cam Fiberler Üzerinden **Işık sinyali** Gönderir.

Her İki Uçta da İki Konnektör Olduğuna Dikkat Edin. Bunun Nedeni, Veri İletmek için Bir Konnektör ve Veri Almak için Bir Konnektörün Kullanılmasıdır. Bakır Kablolar Veri İletmek ve Almak için Kablo İçinde Ayrı Tel Çiftleri Kullanıyordu. Fiber Optik Kablolar Bunun Yerine Veri Almak ve İletmek için Ayrı Kablolar Kullanır.

[![]({{ '/assets/images/tutorials/ccna/day-02/image-22.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjM-6cQT2JaTaMEF4CuXa0gSurhUfyh1zZ0UFgnrt4rF-_EJnjZMupMUOBdsZEXPzgCiC6l8gUDKMOwb7qOaLgEtPC38Fd8OKBIIyYmewvIG62g7UX9tpRmLHZ9O0n3caz8LoVsMLC9IFESVV4ki59_QnCGihaGh3fI2TXWsboWhe576rBsW9jYOWb6nw/s682/resim8.jpg)

#### Fiber-Optik Kablo Yapısı

[![fiber optik kablo yapısı]({{ '/assets/images/tutorials/ccna/day-02/image-23.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEim3tHovsrOc3V5YyKJZCLEyV3U4txvH3b5roJYebTuU8s_DMIBIxcngKIk4JNSicssSvuGN_XXR0Ys0xPi5PJKo4NJb1QpQExzX5AHgiUbxkbxnv5ZctiwBGd4pigTjMOl_vWq_FJSz4h_E8Ty5gVkjCPxJZD74NHehHOza3yVqu9HaKeWsVujyN259A/s317/fiber-optik-kablo-yapisi.jpg)

1. **Fiberglass Core:** Verileri Bir Cihazdan Diğerine İletmek için Bu Çekirdekten Işık İletilir.
2. **Cladding:** Işığı Yansıtan Kaplama.
3. **Protective Buffer.**
4. **Kablonun Dış Kılıfı.**

#### Fiber-Optik Kablo Türleri

##### Multimode Fiber

[![multimode fiber kablo yapısı]({{ '/assets/images/tutorials/ccna/day-02/image-24.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj9ZhJ2JAiK-2eEl7D5TBCncNKSuQJImZNvWCb0i82wEfJra8ysD1bdz2oHZwBM8j8E2OSpW2p9-X5HjpGwnKdRt5p5APfst-79ynaMtM9TXmvWcfUtIm-G1hzZBAqUltn6RtDWLmF-vs-5Har_XBMyzLTOXZKQqr3WSzNueYAnt0XCrUeEhodPNurvig/s311/multimode-fiber.jpg)

Merkez, **Fiberglass Core** ve Mavi Alan **Cladding'i** Temsil Eder.

- Çekirdek Çapı, Single Mode Fiberden Daha Geniştir.

- Fiberglass Core İçine Çok Açılı Işık Dalgalarının Girmesine İzin Verir.

- UTP'den Daha uzun, Fakat Single Mode Fiberden Daha Kısa Kablolara İzin Verir.

- Single Mode Fiberden Daha Ucuzdur (Daha Ucuz **LED Tabanlı SFP Transceiver** Nedeniyle).

##### Single Mode Fiber

[![singlemode fiber kablo yapısı]({{ '/assets/images/tutorials/ccna/day-02/image-25.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjyTdsspqAS1LDzQyJeJkXm8E1IHCc498pLJHPWqlGlC--gCuitWCn0KvZOmWMBFcjFpLf1HO3WgGuZrbGMkoBZQ4P6MVRB5HVcztJ2JqjAw90739M5kArnnNkCrxABnqECKpzknuIGEAFhDK9cnLQzqWqeTTharNv_tejsEgonn_k16XjjhvMOJwshgA/s303/singlemode-fiber.jpg)

- Çekirdek Çapı Multimode Fiberden Daha Dardır.

- Işık Dalgaları, Fiberglass Core İçine Tek Bir Açıyla Girer.

- UTP ve Multimode Fiberden Daha Uzun Kablolara İzin Verir.

- Multimode Fiberden Daha Pahalı (Daha Pahalı **Lazer Tabanlı SFP Transceiver** Nedeniyle).

#### Fiber-Optik Kablo Standartları

[![fiber optik kablo standartları]({{ '/assets/images/tutorials/ccna/day-02/image-26.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgF5NlbbPRqvREq0Ic18Pm5QtuyXc8KGVQ4aPGMRX3ysNDHmuVW2uXq5yOwnXsKDnj_krbl65rvuKBRKWMmr6Bt8t5_UzeofBicj99WHNkWAqrCZZW3QwRppQHzactqpHdXTusPgn2dH157qDaQPJ-6taXBPh94JcHWTNcKKByz2adpQgVxiJwBmSov1Q/s594/fiber-optik-kablo-standartlari.jpg)

### UTP ve Fiber Optik Kablo Karşılaştırması

[![utp ve fiber optik kablo karşılaştırması]({{ '/assets/images/tutorials/ccna/day-02/image-27.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhhaOWqOopQT4H7Gew2NKqYCVdcJEwgysc-K9X8hpZkvuhzOm9Qishk9cCzbvg8Tl_0g_4xYe7-U_j8yFoA_ljNF1Vitg5JXOVJQ_bJe_jn4PjUluTCeuuee2o-Lcy5EjJHEx2XcYsRl8COMex0No2OFb6ZUWe-zmlcr8DQvtsOBIAXx8FcU8JSF5X6mQ/s701/utp-vs-fiberoptic.jpg)

UTP ve Fiber-Optik Kabloyu Karşılaştıran Bir Tablo. Bilerek İngilizce Olarak Bıraktım, İngilizceye Alışalım :)

**Not:** Straight Through Cable, Crossover Cable ve Rollover Cable (Console Cable) Piyasada **Patch Cable** Olarak da Bilinir.

**Quiz 1**

[![]({{ '/assets/images/tutorials/ccna/day-02/image-28.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjvLCyq8NoWA7iV0CM9hnrVGKzqpqjruGs5aLaSqcPsXxprPPx-IR4WXzbKFhATK3QqVdFyqbaK-KAyfYuZ2eqUpqvwGWifaHSEsGcvduXFr8WngNkFguEOMjQElwN_h4V9NE7KX1TxTMtb0LgXqImg8KS23uPYxwzEKAISgPRUfDNtzaHILn6QDiYwhw/s621/quiz1.jpg)

**Quiz 2**

[![]({{ '/assets/images/tutorials/ccna/day-02/image-29.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhFucQstcfUrCeEt8cv67lSQhn_ekdYttrLO8JNJaQZoQea83M_7FXdm3GCA0_4gifmcOCFPuwvHOFGHGJ3X2BDMsiBHEkf2zfc5nXG9hMi-GfKvSF__bhwJ5ouitjRIrYXoFLItqtNNzgcWr7GlutmmpadY4dCSbaSMH3pq2L_1AOa6Ph6gucbkFNPPQ/s674/quiz2.jpg)

**Quiz 3**

[![]({{ '/assets/images/tutorials/ccna/day-02/image-30.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhemSg5upJT-Hy2lnkTXFw1Sz0C-3VnldfjO0U_oPv3xoV7KDzzAN2sB6i5JDKPof2Df3xNjhd7qQofhGZFfx64qbNfv1pGm18DlwQAOaV-WFPSkuCCnX7HdU6lNb2H5yutJHuVRwWxVWmsZuAUWvnC0S6TpobJnkzgyz1UjQsh8sNhm9SPat5xswtUXQ/s644/quiz3.jpg)

**Quiz 4**

[![]({{ '/assets/images/tutorials/ccna/day-02/image-31.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhFUttuf2zGNS7XdFV8gLz89r7r7ibHcIKw3SnGr6Ltcl537qmEYbmELhkfM0mcgXpD3hgfrb6SXv8PsMuA4f0MAuMr4WRWpCXbY0sMPfXQMRMa4qfOvNjCVtXPXloJtSDmqfyaILAU7KMkM78ttLDe7igG9gnFAATZbagaYwIbjnmwnbgwvOeBh-v40g/s690/quiz4.jpg)

**Quiz 5**

[![]({{ '/assets/images/tutorials/ccna/day-02/image-32.jpg' | relative_url }})](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEh2tdqqj8if3ZiQddxTlWBiIyWsnoRFydxYnNg2j1jjIar2GQ5vrAqMfkWmzNvk8wVk6qSDTG9lvwlQoD6U8K2yOfpdxe7VgDeLS6JsEFm9kylNx4hZ5rVII0SivgDuoVYf2pqHU-wfkNqkZBu3kDxfWnQWt6ROEbqzSTmxbgVKQZVjYbfQWMy39ep3ww/s675/quiz5.jpg)

****

**Cevaplar (Sırası İle):** a, c, b, a, a

[LAB](https://drive.google.com/file/d/1Ezh0JwliXp3GxcDYlXkkhTOTgMfnU8kU/view?usp=drive_link) - [ANKI](https://drive.google.com/file/d/1VTrIC5ScCEKeknvzQWeM-3vwq2zznDPe/view?usp=drive_link)

Okuduğunuz için Teşekkürler.
