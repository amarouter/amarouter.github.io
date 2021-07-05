## JavaScript Operatörleri
Diğer dillerde olduğu gibi JavaScript'te de çeşitli operatörler vardır. Bu operatörler ile değişkenlere değerler atayabiliriz, atanan değerleri karşılaştırabiliriz, aritmetik işlemleri gerçekleştirebiliriz.

- Atama operatörü `(=)` değişkene değer atamak için kullanılır.

```javascript
let x = 5;         // x degiskenine 5 degeri atanir
let y = 2;         // y degiskenine 2 degeri atanir
let z = x + y;     // z degiskenine 7 degeri atanir (5+2)
```

- Toplama operatörü `(+)` sayıları toplamak için kullanılır.

```javascript
let x = 5;
let y = 2;
let z = x + y;  // z degiskeninin degeri 7 olur
```
- Çarpma operatörü `(*)` sayıları çarpmak için kullanılır.

```javascript
let x = 5;
let y = 2;
let z = x * y;  // z degiskeninin degeri 10 olur
```
### JavaScript Aritmetik Operatörler
Aritmetik operatörler sayılar üzerinde matematiksel işlemler yapmak için kullanılır.

- Toplama : `(+)`

- Çıkarma : `(-)`

- Çarpma : `(*)`

- Bölme : `(/)`

- Arttırma : `(++)`

- Azaltma : `(--)`

- Mod Alma : `(%)`

Aritmetik operatörleri `JavaScript Aritmetik Operatörler` bölümünde detaylı olarak açıkladık.

### JavaScript Atama Operatörleri
Atama operatörleri JavaScript değişkenlerine değer atamak için kullanılır.

| Operatör              | Örnek | Sonuç |
|-----------------------|-------|-------|
| Atama : `(=)`         | x=y   | x=y   |
| Topla ve Ata : `(+=)` | x+=y  | x+y   |
| Çıkar ve Ata : `(-=)` | x-=y  |  x-y  |
| Çarp ve Ata : `(*=)`  | x*=y  | x*y   |
| Böl ve Ata : `(/=)`   | x/=y  | x/y   |
| Kalanı Ata : `(%=)`   | x%=y  | x%y   |

Atama operatörlerini `JavaScript Atama Operatörleri` bölümünde detaylı olarak açıkladık.

### JavaScript string Operatörleri
- Toplama operatörü `+` [number](## "sayısal") değerlerde toplama işlemi yapmak için kullanılırken [string](## "metinsel") değerlerde birleştirme işlemi için kullanılır.

```javascript
let ad = "Turgut";
let soyad = "Uyar";
let adSoyad = text1 + " " + text2;
```
`adSoyad` ın sonucu şöyle olacaktır:
```javascript
 Turgut Uyar
 ```

- Topla ve ata operatörü `+=` değişkenin değerini yeni bir değer ile birleştirir.

```javascript
let mesaj = "Ne güzel ";
mesaj += "bir gün";
```
mesaj in sonucu şöyle olacaktır:

```javascript
Ne güzel bir gün
```

### string'leri(Metin) ve Sayıları Toplama
İki [number](## "sayısal") değeri topladığımızda sonuç yine bir [number](## "sayısal") değerdir. Ancak bir [number](## "sayısal") değer ve bir [string](## "metinsel") değer toplandığında sonuç bir [string](## "metinsel") değerdir.

```javascript
let x = 5 + 5;  // x in degeri 10 olur
let y = "5" + 5;  // y nin degeri "55" olur
let z = "Merhaba" + 5;  // z nin degeri "Merhaba5" olur
```

### JavaScript Karşılaştırma Operatörleri
Karşılaştırma operatörlerini, değişkenler veya değerler arasındaki eşitliği veya farkı saptamak için kullanırız.

Bu operatörler iki değerin karşılaştırmasını yapar ve [true](## "doğru") veya [false](## "yanlış") değerini döndürür.

Karşılaştırma operatörlerini değerleri karşılaştırmak ve sonuca göre işlem yapmak için koşullu ifadelerde kullanırız.

- x ve y eşit mi?
```javascript
x == y
```
- x ve y değerleri ve değer türleri eşit mi?
```javascript
x === y
```
- x ve y değerleri eşit değil mi?
```javascript
x != y
```
- x ve y değerleri veya değer türleri eşit mi?
```javascript
x !== y
```
- x değeri y değerinden büyük mü?
```javascript
x > y
```
- x değeri y değerinden küçük mü?
```javascript
x < y
```
- x değeri y değerinden büyük veya eşit mi?
```javascript
x >= y
```
- x değeri y değerinden küçük veya eşit mi?
```javascript
x <= y
```
- [ternary operator](## "kısaltılmış koşul operatörü")
```javascript
?
```

### JavaScript Mantıksal Operatörler
JavaScript'te birden fazla koşul ifadesini aynı anda değerlendirmek için JavaScript mantıksal operatörlerini kullanırız. 

3 tane JavaScript mantıksal operatör türü vardır:

- ve ( `&&` )
- veya ( `||` )
- değil ( `!` )

### JavaScript Tip Operatörleri
2 tane JavaScript tip operatörü vardır:

- `typeof` değişken tipini öğrenmek için kullanırız.
- `instanceof` değişken tipini karşılaştırmak için kullanırız.

Tip operatörleri ile ilgili daha fazla bilgi için `Tip Dönüşümleri` bölümümüze bakabilirsiniz.

### JavaScript Ternary Operator
Ternary Operator  adından da anlaşılacağı üzere 3 adet parametre alan tek JavaScript operatörüdür. 

Sıklıkla `if` karşılaştırmalarında kullanılır.

Satır sayısı kullanımını azaltır.

Daha fazla bilgi için [buraya](https://muratdogan.medium.com/javascript-hap-yaz%C4%B1s%C4%B1-ternary-operator-2788782189fb) göz atabilirsiniz.

#### Kaynakça
[w3schools JavaScript Operators](https://www.w3schools.com/js/js_operators.asp)

