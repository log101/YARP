# Ping, PONG (Python)

![gif](https://media.giphy.com/media/rpbYdRj0y1iRLdcRtE/giphy.gif)

## Giriş

Küçük harfler ve büyük harfler. Aynı yüzyüze sohbette olduğu gibi, aşağı yukarı [50 senelik](https://en.wikipedia.org/wiki/Online_chat) bir mazisi olan çevrimiçi sohbetin de kendine has bir kültürü vardır. Mesela kelimeleri BÜYÜK harfle yazmak, "bağırmak" anlamına gelir. "Merhaba" ile "MERHABA" arasındaki fark gibi. Biz de bu projede BAĞIRAN BİR API YAZACAĞIZ!

## Kullanılacak Diller & Kütüphaneler

- Python
  - Kullanıcıların isteklerini yanıtlayabilmek için: [Flask](https://flask.palletsprojects.com/en/2.3.x/)

## Yapılacaklar

- Kullanıcıların `GET` isteği atacakları bir endpoint yazın. Endpoint'in ismine kendiniz karar verebilirsiniz: `/buyuk` gibi.
  - Bu endpoint URL parametresi olarak gönderilen herhangi bir metni büyük harfli olarak kullanıcıya dönmeli ve parametrenin anahtarının ismi `text` olmalı.

## Öğrenilmesi Gereken Konular & Kavramlar

- HTTP protokolü ve metodları, özellikle `GET` metodu.
- JSON veri yapısı.

## Projenin Sağlaması Gereken Şartlar

- API `7070` portunda çalışmalı.
- Endpoint'e herhangi bir parametre belirtmeden istek atıldığında sunucunuz [400 Bad Request](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400) hatası dönmeli.

## İpuçları

- Parametre derken neyi kastediyoruz? Mesela şu URL'deki URL parametreleri hangileri söyleyebilir misin?
  - `https://www.google.com/search?q=alidesidero`

## Kendini Biraz Daha Zorlamak İsteyenler İçin

- Harfleri büyütülmüş metni kullanıcıya bir JSON nesnesi olarak sunun. Mesela "log101" metni gelirse cevaben `{ "message": "LOG101" }` nesnesini döndürmelisiniz.
