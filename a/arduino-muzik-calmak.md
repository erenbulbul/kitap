# Arduino Buzzer İle Nasıl Müzik Çalınır

## Gerekli Malzemeler

* Arduino
* Buzzer
* Kablo
* 1 Adet Direnç (220 Ohm)
* Kırmızı LED

## Kurulum

1. Bir adet LED'in ayakları 12 numaralı Arduino pinlerine bağlanır
2. LED'in diğer ucu 220 Ohm'luk direnç ile toprak hattına bağlanır.
3. Toprak hattı GND pinine bağlanır.
4. Buzzerın bir kolu 220 Ohm direnç ile GND'ye bir kolu 9 numaralı Arduino pinine bağlanır.
5. Çalınacak melodinin notaları, 24 adet olmak üzere koddaki ``melodi[]`` kısmına yazılır.
6. Genel tempo ve her notanın süresi ayarlanır.

## Kod

```c
#define dok  1000// (kalın do)
#define re   1120
#define mi   1260
#define fa   1335
#define sol  1500
#define la   1680
#define si   1890
#define doi  2000// (ince do)


int melodi[] ={mi,sol,doi,mi,sol,doi,mi,sol,doi,mi,sol,doi,mi,sol,si,mi,sol,si,mi,sol,si,mi,sol,si,mi,sol,si};
int notasuresi[] = {3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3};
int tempo = 1000;
 
void loop() 
{

   for (int Nota = 0; Nota <24; Nota++)
    {int sure = tempo/notasuresi[Nota];
     tone(9, melodi[Nota],sure);
     tone(12, melodi[Nota],sure);
     delay(sure*1.2);
    }
 }
```

