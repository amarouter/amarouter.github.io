### JavaScript Aritmetik Operatörler
Aritmetik operatörler sayılar üzerinde aritmetik işlemler (toplama, çıkarma, çarpma, bölme...) yapmak için kullanılır.

- Toplama : `(+)`

- Çıkarma : `(-)`

- Çarpma : `(*)`

- Bölme : `(/)`

- Arttırma : `(++)`

- Azaltma : `(--)`

- Mod Alma : `(%)`

Aritmetik operatörler iki sayı üzerinde işlem yapar.

Sayılar `sabit` değerli olabilir.

```javascript
let toplam = 100 + 50;
```

Sayılar `değişken` değerli olabilir.

```javascript
let sayi1 = 10;
let sayi2 = 7;
let toplam = sayi1 + sayi2;
```

Sayılar `sabit veya değişken` değerli olabilir.

```javascript
let sayi1 = 10;
let toplam = (100 + 50) + sayi1;
```

### Operatörler ve Operand'lar
Sayılar aritmetik operatörlerde `operand` veya `işlenen` olarak adlandırılır.

İşlem ise `operatör` olarak adlandırılır.

- Toplama operatörünü `(+)` sayıları toplamak için kullanıyoruz.

```javascript
let x = 5;
let y = 2;
let z = x + y;
```
- Çıkarma operatörünü `(-)` sayıları çıkarmak için kullanıyoruz.

```javascript
let x = 5;
let y = 2;
let z = x - y;
```
- Çarpma operatörünü `(*)` sayıları çarpmak için kullanıyoruz.

```javascript
let x = 5;
let y = 2;
let z = x * y;
```
- Bölme operatörünü `(/)` sayıları bölmek için kullanıyoruz.

```javascript
let x = 5;
let y = 2;
let z = x / y;  // z'nin degeri 2.5 olur.
```
- Mod alma operatörünü `(%)` bölümden kalanı bulmak için kullanıyoruz.

```javascript
let x = 5;
let y = 2;
let z = x % y;  // z'nin degeri 1 olur.
```
- Arttırma operatörünü `(++)` sayıyı bir arttırmak için kullanıyoruz.

```javascript
let x = 5;
x++;
let z = x;  // z'nin degeri 6 olur.
```
- Azaltma operatörünü `(--)` sayıyı bir azaltmak için kullanıyoruz.

```javascript
let x = 5;
x--;
let z = x;  // z'nin degeri 4 olur.
```

### Operatör Önceliği
Operatör önceliği, aritmetik operatörlerde işlem sırasını belirler.

Aşağıdaki örneği inceleyelim.

```javascript
let sonuc = 100 + 50 * 3;
```

- Matematikte olduğu gibi önce çarpma işlemi ardından toplama işlemi yapılır.

- Çarpma ve bölme işlemlerinin toplama ve çıkarma işlemlerine göre işlem önceliği vardır.

- Parantez "`()`" kullanarak işlem önceliğini değiştirebiliriz.

Aşağıdaki örneği inceleyelim.

```javascript
let sonuc = (100 + 50) * 3;  // Once parantez icindeki islem yapilir, bu yuzden sonuc 450 olur.
```
- Aynı işlem önceliğine sahip operatörlerde işlemler soldan sağa doğru yapılır.

```javascript
let sonuc = 100 + 50 - 3;  // sonuc 147 olur.
```

#### Kaynakça

[w3schools JavaScript Arithmetic](https://www.w3schools.com/js/js_arithmetic.asp)
