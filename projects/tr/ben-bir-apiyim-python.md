# Proje: Ben Bir API'yim (Python)

## Giriş

![wolverine](https://media.giphy.com/media/2nwTda1ewYssE/giphy.gif)

**"Gregor Samsa bir sabah bunaltıcı düşlerden uyandığında, kendini yatağında dev bir *API*'ye dönüşmüş olarak buldu..."**. İtiraf edelim hikaye tam olarak böyle başlamıyor ama API'ler bir programcı için hayati öneme sahip, burası kesin. API'leri kullanmayı [daha önceki projemizde](https://gist.github.com/log101/cae289704aec54fa054c05b26833a86b) zaten öğrenmiştik. Bu projede bir adım daha ileri gidip kendimiz bir API yazacağız.

Projedeki hedefimiz eskiden PokéAPI'ye istek atarak ulaştığımız verilere şimdi kendi yazdığımız API vasıtasıyla ulaşmak.

## Kullanılacak Diller & Kütüphaneler

- Python
  - Kullanıcıların isteklerini yanıtlayabilmek için: [Flask](https://flask.palletsprojects.com/en/2.3.x/)

## Yapılacaklar

1. Kullanıcıların `GET` isteği atabileceği bir endpoint yaz.
   - Bu endpoint `GET` parametresi olarak gelen pokémonun ismini kullanarak PokéAPI'ye istek atmalı.
2. PokéAPI'ye atılan istekten dönen nesneyi kullanıcıya dön.
3. Bir önceki projede yazdığımız uygulama ile API'ne istek at.

## Öğrenilmesi Gereken Konular & Kavramlar

- HTTP protokolü ve metodları, özellikle `GET` ve `POST` metodları.
- REST API'ler
- Endpoint
- Decorators (Python)
- Sınıflar / Classes (Python)

## Projenin Sağlaması Gereken Şartlar

- Yazacağınız API `localhost:3000` adresinde çalışmalı.
- Endpoint'in adresine siz karar verebilirsiniz, anlamlı bir isim vermeye çalışın, örneğin: `/pokemon`.
- Endpoint'e herhangi bir parametre belirtmeden istek atıldığında sunucunuz [400 Bad Request](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400) hatası dönmeli.
- Parametre olarak belirtilen pokémon bulunamazsa sunucunuz [404 Not Found](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/404) hatası dönmeli.
- Parametre olarak belirtilen pokemon bulunduğu takdirde PokéAPI'nin size döndüğü cevabı olduğu gibi kullanıcıya sunabilirsiniz.

## İpuçları

- Her daim aklınızda bulunması gereken anahtar kavramlar:
  - Bir HTTP isteği iki özne arasında gekçekleşir: **İstemci(client)** ve **sunucu(server)**
  - İstemci sunucuya bir **istek(request)** gönderir ve sunucu buna karşılık olarak bir **yanıt(response)** döner.
- Flask dokümantasyonunu detaylı bir şekilde okuyun, muhtemelen ihtiyacınız olan bir çok fonksiyon çoktan yazılmıştır, mesela: [`abort()`](https://flask.palletsprojects.com/en/2.3.x/api/#flask.abort)
- *Parametre* ile *Payload* arasındaki fark nedir?

## Kendini Biraz Daha Zorlamak İsteyenler İçin

- Gelen isteği HTML ile görselleştirerek kullanıcıya sun ve API'ye tarayıcından eriş.
- API'yi [Postman](https://www.postman.com/) ile test et.
- API'yi [cURL](https://curl.se/) ile test et.
