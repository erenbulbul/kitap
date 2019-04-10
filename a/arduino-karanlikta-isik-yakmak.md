# Arduino ile karanlık olduğunda otomatik ışık yakmak

## Gerekli Malzemeler

* Arduino
* 1 Adet Işık Direnci (LDR)
* 1 Adet Işık (LED)
* Kablo
* 1 Adet Direnç (10 K)

## Yapılışı

1. LDR'nin bir bacağını (bundan sonra LDR1 olarak yazacağım) 5V'a bağlayın.
2. LDR'nin diğer bacağını (bundan sonra LDR2 olarak yazacağım) Arduino'nun A0 pinine bağlayın.
3. 10 K Direncin bir bacağını LDR2'ye, diğer bacağını ise Arduino'nun GND (eksi) pinine bağlayın.
4. LED'in negatif bacağını Arduino'nun GND (eksi) pinine bağlayın.
5. LED'in pozitif bacağını Arduino'nun 13 (Dijital) pinine bağlayın.

## Kod

```c
const int LDR = A0;
int deger;

void setup() {
  pinMode(13, OUTPUT);
  Serial.begin(9600);
}

void loop() {

  deger = analogRead(LDR);
  Serial.println(deger);
  delay(400);

  if(deger<200){
    digitalWrite(13, HIGH);
  }else{
    digitalWrite(13, LOW);
  }

}
```
