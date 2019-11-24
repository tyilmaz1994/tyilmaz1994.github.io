---
layout: post
title:  "Telegram Rss Servis"
subtitle: "Rss Takibi"
date:   2018-09-06 23:34:01
categories: [projects, documentation]
---
## [Artık Kullanılmıyor] Komutlar yenilendi ve aşağıda yazan çoğu açıklama geçersiz. `@RssServiceBot` ile telegramdan iletişim kurarak nelerin değiştiğini görebilirsiniz. 

Proje kısaca, telegram botu kullanarak telegramın grup yada kanalından RSS güncellemelerini takip etmemizi sağlıyor.

## Kullanım

RSS takibi için ilk olarak, `@RssService` adlı bot ile konuşmamız gerekiyor. Botun sadece bir komutu var.

Komut: `/start`.

Komut kullanıldığında,
![start komutu ekranı](/assets/images/startScreen.jpg)
seçenekleri karşımıza çıkıyor.

`1-Channels` seçeneği, karşımıza 3 seçenek çıkartır.

* **List Channels:** Programda sizin eklediğiniz tüm kanalları gösterir. Herhangi bir kanal seçildiğinde, karşımıza programa eklenen tüm RSS ler listelenir. *Seçilen RSS kanala eklenir.*

* **Remove Channel:** Ekli olan kanalları programın listesinden silmenizi sağlar. Kanalın listede gözükebilmesi için, kanalın üzerinden RSS takibi yapılmaması gerekiyor.

* **Add Channel:** Programın listesine kanal eklemek için, `Add Channel` seçeneği seçilmesi gerekiyor. Seçildiğininde kod üretir. Örnek;{% highlight python%}zJV7FXPiRlhvBbn3sjdebGI0ugDVv8XFHYBvzgfzBqWuevsDDV{% endhighlight %}Bu kodu eklenmek istenen kanala mesaj olarak gönderildiğinde, **eğer bot kodu gönderilen kanalda ekliyse, kanal programın listesine eklenir.** Diğer durumlarda kanal eklenemez.

`2-Groups` seçeneği, karşımıza 3 seçenek çıkartır.

* **List Groups:** Programda sizin eklediğiniz tüm grupları gösterir. Herhangi bir grup seçildiğinde, karşımıza programa eklenen tüm RSS ler listelenir. *Seçilen RSS gruba eklenir.*

* **Remove Group:** Ekli olan grupları programın listesinden silmenizi sağlar. Grubun listede gözükebilmesi için, grubun üzerinden RSS takibi yapılmaması gerekiyor.

* **Add Group:** Programın listesine grup eklemek için, `@RssService` botunu eklemek istediğiniz gruba davet ettiğinizde programa otomatik olarak grup eklenir.

`3-Rss` seçeneği, karşımıza 3 seçenek çıkartır.

* **List Rss:** Programda sizin eklediğiniz tüm RSS leri gösterir. Herhangi bir RSS seçildiğinde, RSS in ekli olduğu tüm grupları ve kanalları listeler. Eğer bir grup yada kanal seçilirse, seçilen kanaldan ilgili RSS takibi bırakılır.

* **Remove Rss:** Ekli olan RSS leri programın listesinden silmenizi sağlar. Sadece takibi yapılmayan RSS leri gösterir. **Silinmek istenen RSS grup yada kanaldan takip ediliyorsa, listede gözükmez (silinemez).**

* **Add Rss:** Programın listesine RSS eklemek için, `Add Rss` seçeneği seçilmesi gerekiyor. Seçildiğinde bizden RSS in bulunduğu URL i ister. URL girildiğinde, kontrolü yapılır. Eğer dosya RSS ise sizden takma bir isim istenir. Girilen URL i temsili olarak programda saklanır ve siz botun menülerinde gezinirken gözükür.

## Yenilikler

* `/bugreport` adında yeni bir komut eklendi. Komut sayesinde bize isteklerinizi, karşılaştığınız bug'ları iletebilirsiniz.(2018-11-18)
