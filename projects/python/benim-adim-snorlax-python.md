# Proje: Benim Adım Snorlax (Python)

## Giriş

Pokémon çizgi filmini duymayan yoktur. Bu projede amacımız yazacağımız bir program, bir konsol uygulaması vasıtasıyla, favori pokémonumuzun detaylarını PokéAPI sunucusundan çekmek. Bu proje bize konsol uygulaması yazmayı ve uzak bir sunucu ile (teknik olarak bir API ile) iletişim kurmayı öğretecek.

## Kullanılacak Diller & Kütüphaneler

- Python
  - İstek atmak için [Requests Kütüphanesi](https://docs.python-requests.org/en/latest/)
  - Bize dönecek JSON dosyasını kullanabilmek için [JSON Kütüphanesi](https://docs.python.org/3/library/json.html)

## Yapılacaklar

1. Bir pokémon seç, örneğin "Snorlax".
2. Seçtiğin pokémonun ismi ile PokeAPI sunucusuna istek at, mesela snorlax'ı seçtiysen: [https://pokeapi.co/api/v2/pokemon/snorlax](https://pokeapi.co/api/v2/pokemon/snorlax)
3. Gelen JSON dosyasını bir Python nesnesine çevir.
4. Gelen JSON nesnesinden pokemonun id'sini, adını, kilosunu ve boyunu konsol ekranına yazdır.

## Dikkat Edilmesi Gerekenler

- Atacağınız isteğe gelecek cevabın *türünü* [PokéAPI'nin dokümantasyonundan öğrenebilirsiniz.](https://pokeapi.co/docs/v2#pokemon)

## Öğrenilmesi Gereken Konular & Kavramlar

- Değişkenler
- String veri türü
- Konsola yazı yazdırma
- JSON nesne türü
- HTTP protokolü ve metodları, özellikle `GET` ve `POST` metodları.
- REST API'ler

## Kendini Biraz Daha Zorlamak İsteyenler İçin

- Pokemonun ismini kullanıcıdan al.
- Pokemonun küçük resmini bir dosyaya kaydet. (İpucu: `sprites`)
