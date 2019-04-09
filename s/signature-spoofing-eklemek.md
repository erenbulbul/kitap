# Signature Spoofing Olmayan Bir Android ROM'una Signature Spoofing Eklemek

microG kullanmak istiyorsanız, ROM'unuzun Signature Spoofing desteklemesi
gerekmektedir. Eğer ROM'unuz Signature Spoofing desteklemiyor ise bilgisayarsız
bir şekilde destek ekleyebilirsiniz.

## Xposed İle

[FakeGApps](http://repo.xposed.info/module/com.thermatk.android.xf.fakegapps)
modülünü indirerek Xposed ile Signature Spoofing ekleyebilirsiniz

## Patch Zipi İle

::: warning DIKKAT
Android 9 kullanıyorsanız, services.jar'ı elle deodexlemelisiniz.
Onun için [bu rehberi kullanabilirsiniz](https://github.com/Nanolx/NanoDroid/blob/master/doc/DeodexServices.md)
:::

1. [Bu linkten](https://androidfilehost.com/?w=files&flid=198483) `NanoDroid-patcher` zipini indirin.
2. Recovery kullanarak o zipi flashlayın.
3. Zip, Signature Spoofing desteğini ekleyecektir.