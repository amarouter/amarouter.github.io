## JavaScript [Syntax](## "Yazım Kuralları, Sözdizimi")
JavaScript'te syntax, JavaScript programlarının nasıl oluşturulduğuna dair kurallar kümesidir.

```javascript
// Degiskenler nasil olusturulur:
var x;
let y;

// Degiskenler nasil kullanilir:
x = 5;
y = 6;
let z = x + y;
```

### JavaScript Değerleri
JavaScript ile;

- Sabit Değerler
- Değişken Değerler

olmak üzere iki farklı değer türü yazabiliriz.

### Sabit Değerler 
Herhangi bir değişkende saklamadan yazdığımız değerlerdir.

Sabit değerler için en önemli iki syntax kuralı şunlardır:

1-Sabit değerli [number](## "sayısal") değerler herhangi bir tırnak işareti eklenmeden yazılır.

```javascript
10.50

1001
```

2-Sabit değerli [string](## "metinsel") değerler tek veya çift tırnak arasında yazılır.

```javascript
"Tekir"

'Tekir'
```

### Değişken Değerler
Bir programlama dilinde değişkenleri veri depolamak için kullanırız.

JavaScript dilinde değişken tanımlamak için `var`, `let`, `const` anahtar kelimelerini kullanırız.

Tanımlanan değişkene değer atamak için atama operatörünü`(=)` kullanırız.

Aşağıdaki örnekte `x` bir değişken olarak tanımlanmıştır, daha sonra `x` değişkenine `1907` değer olarak atanmıştır.

```javascript
let x;
x = 1907;
```

### Operatörler
JavaScript'te değerleri hesaplamak için [aritmetik operatörleri](## "+, -, *, /") kullanırız.

```javascript
(5 + 6) * 10  // Sonuc 110 olarak bulunur.
```

### İfadeler
JavaScript'te ifadeleri; değerlerden, değişkenlerden ve operatörlerden yeni değerler üretmek için kullanırız.

Aşağıdaki örnekte iki değerin çarpımı ile yeni bir değer elde edilmiştir:

```javascript
5 * 10  // Sonuc 50 olarak bulunur.
```

İfadelerde `değişken` değerler kullanabiliriz.

```javascript
x * 10
```

İfadelerde [string](## "metinsel") değerler kullanabiliriz.

```javascript
"Tekir" + " " + "Boncuk"
```

### [Keywords](## "Anahtar Kelimeler")
JavaScript'te `anahtar kelimeler`'i, gerçekleştirilecek eylemleri belirtmek için kullanırız.

JavaScript'te `var`, `let` anahtar kelimelerini tarayıcıya yeni değişken oluşturma talimatı vermek için kullanırız.

```javascript
let x, y;
x = 5 + 6;
y = x * 10;
```

```javascript
var x, y;
x = 5 + 6;
y = x * 10;
```

** Yukarıdaki örneklerde görüldüğü gibi `var` veya `let` kullanmak genellikle aynı sonucu verir.

### Yorumlar
Tüm JavaScript kodları tarayıcı tarafından işlenmez.

`Çift eğik çizgi //` sonrasında yazılan kodları veya `/*....*/` arasına yazılan kodları yorum satırı olarak ele alırız.

Yorumlar yok sayılır ve tarayıcı tarafından işlenmez.

```javascript
let x = 5;   // Bu satırdaki komut çalışır.

// x = 6;   Bu satırdaki komut çalışmaz.
```

### Tanımlayıcılar
JavaScript'te değişkenleri, fonksiyonları ve etiketleri isimlendirirken `tanımlayıcı`ları kullanırız.

Tanımlayıcı kuralları çoğu programlama dilleri için aynıdır.

JavaScript'te tanımlayıcının ilk karakteri harf, alt çizgi`(_)`, veya dolar işareti`($)` olmalıdır.

Sonraki karakterler harf, rakam, alt çizgi veya dolar işareti olabilir.

### Büyük/Küçük Harf Duyarlılığı
JavaScript tanımlayıcıları büyük/küçük harfe duyarlıdır.

Aşağıdaki örnekte `kediadi` ve `kediAdi` iki farklı değişkendir:

```javascript
let kediadi, kediAdi;
kediadi = "Tekir";
kediAdi = "Boncuk";
```

### Karakter Seti
JavaScript `Unicode` karakter setini kullanır.

`Unicode`, dünyadaki tüm karakterleri, noktalama işaretlerini ve sembolleri kapsar.


#### Kaynakça

[w3schools JavaScript Syntax](https://www.w3schools.com/js/js_syntax.asp)
