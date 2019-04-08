# F@tih Wi-Fi'ında Bilgisayar Ile Engelleri Aşmak

(Sadece bir okulda denenmiştir)

## Gerekenler
- 80 portunda (webde) bir şey çalıştırmayan bir sunucu (Vultr veya DigitalOcean önerilir)
- Bir bilgisayar (telefonlarda şu anlık bir yol bulamadım)
- SOCKS5 proxyleri kullanabilen bir tarayıcı
- Bir domain (bedava bile olabilir)

## Sunucu Ayarları

1. [Buradan](https://github.com/jpillora/chisel/releases) Chisel programını indiriyorsunuz.
2. Komut satırından, `chisel server -p 80 --socks5` diye çalıştırıyorsunuz
3. Domaininizi sunucunuza bağlıyorsunuz

## Bilgisayar Ayarları

1. Üstteki linkten Chisel programını indiriyorsunuz
2. `chisel client http://sizin.domaininiz socks` diye çalıştırıyorsunuz
3. Tarayıcınızı `127.0.0.1:1080` adresli SOCKS5 proxy'ini kullanmaya ayarlıyorsunuz.

Bu yöntem ile bilgisayarınız ile f@tih ağları içerisinde engelsiz bir şekilde
internet kullanabilirsiniz! (Sadece tarayıcı üzerinden, başka programlar çalışmaz)
