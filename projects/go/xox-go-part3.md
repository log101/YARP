# O|X|O (Go): 3. Kısım

![gif](https://media.giphy.com/media/3og0IEb2EuRQ3xc7kY/giphy.gif)

## Giriş

Kimsenin olmadığı bir yerde atılmış bir API isteği, gerçekten bir yanıt döndürebilir mi? XOX projemizin son bölümünde oyunumuzu tarayıcı üzerinden oynanabilir bir hale getireceğiz.

## Kullanılacak Diller & Kütüphaneler

- HTML
- CSS
- JavaScript
  - Bir önceki kısımda oluşturduğumuz API ile iletişim kurmak için: [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/fetch)

## Yapılacaklar

1. HTML ve CSS kullanarak ekranda 3x3'lük bir tahta gösterin
2. Tahtanın hemen üstünde sıranın kimde olduğunu veya bittiyse oyunun durumunu (galibiyet, yenilgi, beraberlik) gösterin.
3. Tahtanın hücrelerini, tıklandığında API'ye istek gönderecek şekilde güncelleyin:
   1. İsteğin cevabına göre hücreler ve oyunun durumu güncellenmeli.
4. Tahtanın altına oyunu yeniden başlatacak bir buton konulmalı

## Öğrenilmesi Gereken Konular & Kavramlar

- HTML
  - div, p etiketleri (tag)
  - onClick olay işleyicisi (event handler)
- CSS
  - Grid
- DOM
  - Javascript ile DOM elemanlarını güncellemek
- Fetch API
- Eşzamansız fonksiyonlar (asynchronous functions)
  - Async, await

## Projenin Sağlaması Gereken Şartlar

- İlk hamle her zaman "X" olmalı.
- Bütün HTML, CSS ve Javascript kodu tek bir dosyada olmalı.

## İpuçları

- Konu HTML, CSS, Javascript olduğunda ilk başvurmanız gereken kaynak: [MDN](https://developer.mozilla.org/en-US/)
- Başta görüntünün güzelliğine takılmayın, öncelikli olan oyunun çalışması.
- İçerisi boş bir elemanın sınırlarını genişlik ve yükseklik vererek belirleyebilirsiniz.
- Javascript kodlarınızı body etiketinin en altına koymayı unutmayın, yoksa kodunuz sayfa yüklenmeden çalışmaya başlar ve hata alırsınız.

## Kendini Biraz Daha Zorlamak İsteyenler İçin

- Bilgisayara karşı oynama modu ekleyin.
- HTML, CSS ve Javscript kodlarınızı ayrı ayrı dosyalarda tutun.
