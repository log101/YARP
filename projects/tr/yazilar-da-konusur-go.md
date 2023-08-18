# Proje: Yazılar da Konuşur (Go)

## Giriş

![woman-clapping-her-hands](https://media.giphy.com/media/KCdq1IyxkmgRKj2D23/giphy.gif)

Ctrl + Windows Tuşu + Enter ve karşınızda... Neredeyse hiç kimsenin kullanmadığı bir Windows özelliği! TTS ismi verilen "Text-to-Speech" yazılı bir metnin bilgisayar tarafından seslendirilmesi anlamına geliyor. Günümüzde daha çok Tiktok/YT videolarının arkasında duymaya alıştığımız bu teknolojinin faydaları saymakla bitmez, o yüzden saymamaya karar verdik.

Bu projede hedefimiz VoiceRSS' in [Text to Speech API'sini](https://www.voicerss.org/api/) kullanarak bir metin dosyasını seslendirmek.

## Yapılacaklar

- VoiceRSS'in [örnek uygulamasına](https://www.voicerss.org/api/demo.aspx) bir göz atın.
- API'ye seslendirmek istediğiniz metni içeren bir istek atın.
- Gelen ses dosyasını bilgisayarınıza kaydedin.
- Bir API oluşturun ve GET isteği atıldığında kullanıcıya sabit bir ses dosyası dönen bir endpoint yazın.

## Kullanılacak Diller & Kütüphaneler

- Kullanıcıların isteklerini yanıtlayabilmek için: [Fiber](https://gofiber.io/)
- Ses verisini okuyabilmek için: [io](https://pkg.go.dev/io)
- Ses verisini bilgisayarınıza kaydedebilmek için: [os](https://pkg.go.dev/os)
- VoiceRSS'e istek atabilmek için: [net/http](https://pkg.go.dev/net/http)

## Öğrenilmesi Gereken Konular & Kavramlar

- REST API'ler
- HTTP protokolü, özellikle `GET` ve `POST` metodları
- JSON veri türü
- RIFF Formatı

## Dikkat Edilmesi Gerekenler

- API'yi kullanabilmek için önce ücretsiz bir hesap oluşturup API şifresi almalısınız. Bu şifreyi attığınız istekle beraber sunucuya iletmelisiniz. Aksi halde API size yanıt vermeyecektir.
- Herhangi bir programlama dilinde bilgisayarınızda dosya indirme, okuma, yazma gibi işlemler yapmak için yerleşik (built-in) kütüphaneler kullanıyoruz. GO dilinde bu `os` ve `io` kütüphaneleri oluyor. Bu işlemlerin nasıl yapılacağını bilmeniz bu projeyi tamamlayabilmeniz için önemli.
- Kullanıcıya döneceğimiz dosyanın formatı RIFF (Resource Interchange File Format) ve içerik tipi "audio/wav". Endpoint fonksiyonunda bunu belirtmeniz tarayıcının gelen dosyası doğru bir şekilde anlamlandırmasını sağlayacaktır.

## Projenin Sağlaması Gereken Şartlar

- Yazacağınınz API `localhost:3000` adresinde çalışmalı.
- Endpoint'in adresine siz karar verebilirsiniz, örneğin: `/ismail-abi`.
- Endpoint'e herhangi bir parametre belirtmeden istek atıldığında sunucunuz 'hoop' gibi sabit bir metnin seslendirmesini dönmeli.

## Kendini Biraz Daha Zorlamak İsteyenler İçin

- Seslendirilecek metni `GET` parametresi olarak kullanıcıdan alın.
