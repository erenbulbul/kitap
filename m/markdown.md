# Markdown Nasıl Kullanılır

İşsizliğin Kitabı dahil bir çok yere yazabilmek için,
[Markdown](https://help.github.com/en/articles/basic-writing-and-formatting-syntax) kullanmanız gerekmektedir

Markdown, amacı formatlanmadan da okunması olan bir yazı formatlama dilidir,
bu nedenle, kullanımı çok kolaydır.

## Alt Satıra İnmek

Bir satırdan sonra direkt olarak alt satıra geçmeye çalışırsanız
iki satır birleşecektir.  
Bunu engellemek için, önceki satırın sonuna iki boşluk koyabilirsiniz.

```md
Bir satırdan sonra direkt olarak alt satıra geçmeye çalışırsanız
iki satır birleşecektir.__
Bunu engellemek için, önceki satırın sonuna iki boşluk koyabilirsiniz.
```

(Alt çizgiler boşlukları ifade etmektedir.)

## Başlıklar

Başlıklar, 1'den 6'ya kadar `#` işareti koyularak belirtilir.

```md
## Başlıklar

Başlıklar, 1'den 6'ya kadar `#` işareti koyularak belirtilir.
```

## Yazı Stilleri

Yazılar, **kalın**, _eğik_, ~~çizgili~~ veya **_~~hepsi~~_** olabilir.

```md
Yazılar, **kalın**, _eğik_, ~~çizgili~~ veya **_~~hepsi~~_** olabilir.
```

## Alıntılama

> Alıntılar, yazının başına `>` işaretini koyarak yapılabilir

```md
> Alıntılar, yazının başına `>` işaretini koyarak yapılabilir
```

## Kod

Eğer ekleyeceğiniz kod `satır içinde` olacak ise, \`\` arasına koymanız yetmektedir.

Eğer birden fazla satır koyacaksanız, \`\`\`&lt;dil> blokları arasına almanız gerekmektedir.

```md
Eğer ekleyeceğiniz kod `satır içinde` olacak ise, `` arasına koymanız yetmektedir.

Eğer birden fazla satır koyacaksanız, ```<dil> blokları arasına almanız gerekmektedir.

```python
print("Merhaba, dünya!")```
```

## Linkler

Link eklemek için, Link ismini `[]`, linkin kendisini `()` arasına almanız
yetmektedir.

```md
Bu yazı, [İşsizliğin Kitabı](https://issizler.club)'ndan bir alıntıdır.
```

## Listeler

Ekleyebileceğiniz iki tane liste türü vardır.

1. Numaralı listeler
2. Numarasız listeler

### Numaralı Listeler

Numaralı liste eklemek için, numaradan sonra bir nokta koyarak
istediğinizi yazabilirsiniz.

```md
Ekleyebileceğiniz iki tane liste türü vardır.

1. Numaralı listeler
2. Numarasız listeler
```

### Numarasız Listeler

Numarasız liste eklemek için, bir çizgi koyup, devamına istediğinizi yazabilrsiniz.

```md
Ekleyebileceğiniz iki tane liste türü vardır.

- Numaralı listeler
- Numarasız listeler
```

### Liste İçi Listeler

Bir listenin içine başka bir liste koymak isterseniz, ikinci listeden önce
biraz boşluk bırakın.

```md
1. Başlıklar
2. Listeler
  - Numaralı Listeler
    - Nasıl Yapılır
    - Avantajları
  - Numarasız Listeler
    - Buraları örnek olarak dolduruyorum
    - Falan filan
  - Liste İçi Listeler
    - Bir Liste Daha
```

### Resim Eklemek

Resim eklemek, Link eklemek ile aynıdır. Sadece link'i eklemeden önce bir ünlem
koymanız gerekmektedir.

::: tip NOT
İşsizliğin Kitabı'na yazıyor iseniz, resimlerinizi `media/` klasörü altına,
önceki sayfalar nasıl yapıyorsa o şekilde koymanız tavsiye edilmektedir.
:::

```md
![Kedi Resmi](../media/m/markdown/kedi.png)  
[Resim Kaynağı](https://unsplash.com/photos/IbPxGLgJiMI)
```

![Kedi Resmi](../media/m/markdown/kedi.png)  
[Resim Kaynağı](https://unsplash.com/photos/IbPxGLgJiMI)

## Not Ve Uyarı Eklemek

::: warning UYARI
Bunlar, İşsizliğin Kitabı ve benzer **Vuepress** sayfalarına özeldir.  
Başka yerlerde kullanamazsınız.
:::

```md
::: warning UYARI
Bunlar, İşsizliğin Kitabı ve benzer **Vuepress** sayfalarına özeldir.  
Başka yerlerde kullanamazsınız.
:::
```

`warning` (sarı, uyarı) yerine, `tip` (yeşil, not) veya `danger` (kırmızı, önemli) kullanabilirsiniz.

## Emoji

Emoji :ok_hand: kullanabilmek için, emoji ismini `:` arasına almanız gerekmektedir.  
Tam emoji listesini [buradan](https://github.com/markdown-it/markdown-it-emoji/blob/master/lib/data/full.json) bulabilirsiniz.

```md
Emoji :ok_hand: kullanabilmek için, emoji ismini `:` arasına almanız gerekmektedir.  
```

## Tablolar

| İsim          | Alma Nedeni      | Fiyat |
| ------------- | ---------------- | ----- |
| Çay Bardağı   | Kahve içmek için | 20 ₺  |
| Kahve Bardağı | Çay içmek için   | 21 ₺  |

```md
| İsim          | Alma Nedeni      | Fiyat |
| ------------- | ---------------- | ----- |
| Çay Bardağı   | Kahve içmek için | 20 ₺  |
| Kahve Bardağı | Çay içmek için   | 21 ₺  |
```