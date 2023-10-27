# O|X|O (Go): 2. Kısım

## Giriş

Evet, ilk bölümde XOX oyununun komut satırı sürümünü oluşturduk. Bu bölümde, oyunu bir API aracılığıyla oynamanızı sağlayacak şekilde güncelleyeceğiz!

## Kullanılacak Diller & Kütüphaneler

- Go
  - API arayüzünü oluşturmak için: [Fiber](https://gofiber.io/)

## Yapılacaklar

1. Oyunu başlatmak, yeniden başlatmak, oyun tahtasını görüntülemek ve oyunda bir hamle yapmak için API uçnoktaları (endpoint) yazın.
  1. `/start` uçnoktası oyunu başlatmalı ve tahtanın başlangıç durumunu kullanıcıya iletmeli.
  2. `/restart` uçnoktası oyunu yeniden başlatmalı, aynı şekilde tahtanın başlangıç durumunu kullanıcıya iletmeli.
  3. `/move` parametre olarak bir x ve y değeri almalı, bunlar tahtadaki bir noktanın kordinatını temsil etmeli.
  4. `/board` tahtanın anlık durumunu kullanıcıya iletmeli.

## Öğrenilmesi Gereken Konular & Kavramlar

- Fiber ile uçnokta oluşturma.
- HTTP GET metodu.
- HTTP isteklerine sorgu parametreleri ekleme.

## Projenin Sağlaması Gereken Şartlar

- Bütün uçnoktalar GET metodunu desteklemeli.
- `/move` uçnoktasıyla yapılan isteklerde sıra otomatik olarak birinci ve ikinci oyuncu arasında değişmeli, hamle sırası da kullanıcıya iletilmeli.
- Oyun bittiği takdirde beraberlik veya galibiyet/mağlubiyet durumu kullanıcıya bildirildikten sonra oyun sıfırlanmalı.

## İpuçları

- Farklı uçnoktalar aynı fonksiyonlardan faydalanabilir.

## Kendini Biraz Daha Zorlamak İsteyenler İçin

- Oynanmış oyunların kaydını istediğiniz formatta bir JSON dosyasında saklayın.
