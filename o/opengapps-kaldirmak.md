# OpenGApps Nasıl Kaldırılır

microG kullanmayı, veya telefonunuzu direkt GApps'sız olarak kullanmayı
düşünüyorsanız, hiç bir verinizi silmeden OpenGApps'ı kaldırabilirsiniz.

::: warn DIKKAT
Bu işlem sadece tek bir telefonda denenmiştir, bir sıkıntı olursa bizi sorumlu
tutmayın. İnternetten rastgele bir rehberi takip eden sizsiniz.
:::

## Gereksinimler

- Signature Spoofing patch'i olan bir ROM zaten kurulu olmalı
- Şu anki kurulu ROM'un kurulum zipi sizde bulunmalı

## OpenGApps Kaldırma

- TWRP'ye giriş yapın
- /system'i bağlayın
- Advanced > File Manager
- /system/addon.d klasörüne girin
- numara_gapps.sh dosyasını silin
- Hiç bir şey silmeden ROM zipini flashlayın
- Kalan bütün Google uygulamalarını ayarlardan kaldırın

::: warn DIKKAT
ROM flashlayıp sisteme geri girdiğinizde, Google Play Servisleri bir çökme
döngüsünde kalacaktır, Google Play Servislerini ayarlardan silebilirsiniz.
:::