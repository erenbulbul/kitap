# OpenGApps Nasıl Kaldırılır

microG kullanmayı, veya telefonunuzu direkt GApps'sız olarak kullanmayı
düşünüyorsanız, hiç bir verinizi silmeden OpenGApps'ı kaldırabilirsiniz.

::: warning DIKKAT
Bu işlem sadece tek bir telefonda denenmiştir, bir sıkıntı olursa bizi sorumlu
tutmayın. İnternetten rastgele bir rehberi takip eden sizsiniz.
:::

## Gereksinimler

- Signature Spoofing patch'i olan bir ROM zaten kurulu olmalı
  - microG gereksinimi. Yok ise [Signature Spoofing Ekleme](../s/signature-spoofing-eklemek.md) sayfasına bakabilirsiniz.
- Şu anki kurulu ROM'un kurulum zipi sizde bulunmalı

## OpenGApps Kaldırmak

1. TWRP'ye giriş yapın
2. `/system`'i bağlayın
3. Advanced **>** File Manager
4. `/system/addon.d` klasörüne girin
5. `<numara>_gapps.sh` dosyasını silin
6. Hiç bir şey silmeden ROM zipini flashlayın
7. Kalan bütün Google uygulamalarını ayarlardan kaldırın

::: warning DIKKAT
ROM flashlayıp sisteme geri girdiğinizde, Google Play Servisleri bir çökme
döngüsünde kalacaktır, Google Play Servislerini ayarlardan silebilirsiniz.
:::