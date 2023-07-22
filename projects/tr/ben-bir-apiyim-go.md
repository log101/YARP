
# Proje: Ben Bir API'yim (Go)

## Giriş

![minions](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_images/tenor_1.gif)

**"Gregor Samsa bir sabah bunaltıcı düşlerden uyandığında, kendini yatağında dev bir *API*'ye dönüşmüş olarak buldu..."**. İtiraf edelim hikaye tam olarak böyle başlamıyor ama API'ler bir programcı için hayati öneme sahip, burası kesin. API'leri kullanmayı [daha önceki projemizde](https://gist.github.com/log101/cae289704aec54fa054c05b26833a86b) zaten öğrenmiştik. Bu projede bir adım daha atıp kendimiz bir API yazacağız.

Projedeki hedefimiz eskiden PokéAPI'ye atarak ulaştığımız verilere kendi yazdığımız API vasıtasıyla ulaşmak.

## Kullanılacak Diller & Kütüphaneler

- Golang
  - Kullanıcıların isteklerini yanıtlayabilmek için: [Fiber](https://gofiber.io/)

## Yapılacaklar

1. Kullanıcıların `GET` isteği atabileceği bir endpoint yaz.
   - Bu endpoint `GET` parametresi olarak gelen pokémonun ismini kullanarak PokéAPI'ye istek atmalı.
2. PokéAPI'ye atılan istekten dönen nesneyi kullanıcıya dön.
3. Küçük bir konsol uygulamasıyla API'ni test et.

## Öğrenilmesi Gereken Konular & Kavramlar

- HTTP protokolü ve metodları, özellikle `GET` ve `POST` metodları.
- REST API'ler
- Endpoint
- Struct, Interface, Methods (Golang)

## Projenin Sağlaması Gereken Şartlar

- Yazacağınınz API `localhost:3000` adresinde çalışmalı.
- Endpoint'in adresine siz karar verebilirsiniz, örneğin: `/pokemon`.
- Endpoint'e herhangi bir parametre belirtmeden istek atıldığında sunucunuz [400 Bad Request](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400) hatası dönmeli.
- Parametre olarak belirtilen pokémon bulunamazsa sunucunuz [404 Not Found](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/404) hatası dönmeli.
- Parametre olarak belirtilen pokémon bulunduğu takdirde PokéAPI'nin size döndüğü isteği olduğu gibi(JSON formatında) kullanıcıya sunabilirsiniz.

## İpuçları

- Her daim aklınızda bulunması gereken anahtar kavramlar:
  - Bir HTTP isteği iki özne arasında gekçekleşir: **İstemci(client)** ve **sunucu(server)**
  - İstemci sunucuya bir **istek(request)** gönderir ve sunucu buna karşılık olarak bir **yanıt(response)** döner.
- Fiber dokümantasyonunu detaylı bir şekilde okuyun, muhtemelen ihtiyacınız olan bir çok fonksiyon çoktan yazılmıştır, mesela: ["Status()"](https://docs.gofiber.io/api/ctx#status)
- *Parametre* ile *Payload* arasındaki fark nedir?

## Kendini Biraz Daha Zorlamak İsteyenler İçin

- Gelen isteği HTML ile görselleştirerek kullanıcıya sun ve API'ye tarayıcından eriş.
- API'yi [Postman](https://www.postman.com/) ile test et.
- API'yi [cURL](https://curl.se/) ile test et.
