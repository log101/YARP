# Proje: Benim Adım Snorlax (Go)

## Giriş

![snorlax](https://media.giphy.com/media/LT6BnfiyOWsqQ/giphy.gif)

Pokémon çizgi filmini duymayan yoktur. Bu projede amacımız yazacağımız bir program, bir konsol uygulaması vasıtasıyla, favori pokémonumuzun detaylarını PokéAPI sunucusundan çekmek. Bu proje bize konsol uygulaması yazmayı ve uzak bir sunucu ile (teknik olarak bir API ile) iletişim kurmayı öğretecek.

## Kullanılacak Diller & Kütüphaneler

- Go
  - PokéAPI'ye istek atabilmek için [`net/http`](https://pkg.go.dev/net/http) kütüphanesi
  - Bize dönecek JSON dosyasını kullanabilmek için [`json`](https://pkg.go.dev/encoding/json) kütüphanesi

## Yapılacaklar

1. Bir pokémon seç, örneğin "Snorlax".
2. Seçtiğin pokémonun ismi ile PokeAPI sunucusuna istek at, mesela snorlax'ı seçtiysen: [https://pokeapi.co/api/v2/pokemon/snorlax](https://pokeapi.co/api/v2/pokemon/snorlax)
3. Gelen JSON dosyasını bir Go nesnesine(struct) çevir.
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
