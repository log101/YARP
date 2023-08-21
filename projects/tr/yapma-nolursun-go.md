# Yapma N'olursun! (1. Kısım) (Go)

![gif](https://media.giphy.com/media/3o7WIE14z2d66BJWJa/giphy.gif)

## Giriş

"İnsan, nisyan ile malüldür" demişler, istesek de istemesek de unutmak doğamızda var. Neyse ki bunun farkında olan insanoğlu uzun zaman önce yazıyı icad etmiş, unutmaması gerekenleri de bir kenara kaydetmiş.
Biz de bu projede bir _yapılacaklar listesi_ API'si oluşturacağız ve unutmamamız gerekenleri bir PostgreSQL veritabanında saklayacağız.

## Kullanılacak Diller & Kütüphaneler

- Go
  - Kullanıcıların isteklerini yanıtlayabilmek için: [Fiber](https://gofiber.io/)
  - Veritabanı işlemleri için: [GORM](https://gorm.io/)
- PostgreSQL

## Yapılacaklar

- Yapılacak listesinde ekleme, silme, güncelleme ve listeleme işlemlerini yapabileceği API uçnoktaları (endpoint) yazın.
  - `/todos` - Tüm yapılacakları listeler
  - `/todos/:id` - Belirli bir yapılacağı gösterir
  - `/todos` (POST) - Yeni bir yapılacak ekler
  - `/todos/:id` (PUT) - Bir yapılacağı günceller
  - `/todos/:id` (DELETE) - Bir yapılacağı siler

## Öğrenilmesi Gereken Konular & Kavramlar

- HTTP metodları: `GET`, `POST`, `PUT`, `DELETE`.
- Object Relational Mapping (ORM).
- SQL ve veritabanı işlemleri.

## Projenin Sağlaması Gereken Şartlar

- API `8080` portunda çalışmalı.
- Uçnoktalara uygun olmayan bir istek atıldığında sunucunuz [400 Bad Request](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400) hatası dönmeli.
- Talep edilen yapılacak bulunamadığı takdirde sunucunuz [404 Not Found](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/404) hatası dönmeli.

## İpuçları

- Öncelikle sisteminizde PostgreSQL veritabanının kurulu ve çalışır durumda olduğundan emin olun. Komut satırından bağlanıp örnek bir veritabanı oluşturmayı deneyebilirsiniz.
- Veritabanı işlemleri için Go'nun popüler bir kütüphanesi olan [GORM](https://gorm.io/docs/connecting_to_the_database.html)'u kullanabilirsiniz. Bu kütüphane veritabanı bağlantısından ve nesnelerini saklanabilir hale getirmekten sorumlu olacak.
- Bir yapılacak nesnesinin nitelikleri nelerdir? Mesela başlık eklemeli mi yoksa sadece bir string tutmak yeter mi?

## Kendini Biraz Daha Zorlamak İsteyenler İçin

- Görevlerin ne zaman eklendiğini de kullanıcıya dönün.
- Görevleri tamamlanmış veya tamamlanmamış olarak işaretlenebilir hale getirin.

2. Kısımda projemiz için bir önyüz geliştireceğiz, takipte kalın.
