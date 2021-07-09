## JavaScript Veri Tipleri
JavaScript ile değişken oluştururken farklı veri tipleri kullanabiliriz.

JavaScript değişkenlerinde [number](##"sayı"), [string](## "metin"), [object](## "nesne") veri tiplerini barındırabilir.

```javascript
let uzunluk = 16;                          // Number
let soyad = "Kilikya";                     // String
let calisan = {ad:"İsa", soyad:"Kilikya"};       // Object
```

### Veri Tipleri Kavramı
Programlamada veri tipleri önemli bir kavramdır.

Değişkenler üzerinde işlem yapabilmek için veri tipleri hakkında bilgi sahibi olmamız önemlidir.

Veri tipleri olmadan bilgisayarlar aşağıdaki ifadenin ne olduğunu güvenli bir şekilde çözemez.

```javascript
let x = 16 + "kedi";
```

Yukarıdaki işlemin sonucunda 16 değeri ile "kedi" değeri toplanacak mı, yoksa hata mı oluşacak?

JavaScript yukarıdaki örneği aşağıdaki gibi yorumlayacak:

```javascript
let x = "16" + "kedi";
```

- Bir [number](##"sayı") değer ve bir [string](## "metin") değer toplanırken Javascript `number` veri tipini `string` veri tipine dönüştürür.
- JavaScript işlemleri `soldan sağa` doğru yapar, farklı değerler farklı sonuçlar verebilir.

`number` değeri `string` değerin soluna yazdığımızda;

```javascript
let x = 16 + 4 + "kedi";
```

Sonuç:

```javascript
20kedi
```

`number` değeri `string` değerin sağına yazdığımızda;

```javascript
let x = "kedi" + 16 + 4;
```

Sonuç:

```javascript
kedi164
```

İlk örnekte JavaScript "kedi" değerine kadar değişkenleri [number](##"sayı") veri tipi olarak ele alır.

İkinci örnekte ise ilk değer [string](## "metin") veri tipinde olduğu için sonradan gelen değerler de `string` veri tipinde ele alınır.

### JavaScript Veri Tipleri Dinamiktir
JavaScript veri tipleri dinamiktir. Bir değişkeni aynı kod içinde farklı veri tipleri için kullanabiliriz.

Dinamik ve statik programlama dilleriyle ilgili daha fazla bilgi için [buraya](https://www.kadir.xyz/yazi/65/statik-ve-dinamik-programlama-dillerinin-farklari) göz atabilirsiniz.

```javascript
let x;           // x değişkeninin veri tipi undefined
x = 7;           // x değişkeninin veri tipi number
x = "kedi";      // x değişkeninin veri tipi string
```

### [Primitive](## "Temel") Veri Tipleri
JavaScript [Primitive](## "Temel") veri tipleri yalnızca bir değer içeren veri tipleridir. Bunlar:
- string
- number
- boolean
- undefined
- [bigint](## "Diğer veri tiplerine oranla az kullanılır.")
- [symbol](## "Diğer veri tiplerine oranla az kullanılır.")
- [null](## "Özel bir primitive veri tipidir. Özel kullanım alanları vardır.")

### [Structural](## "Yapısal") Veri Tipleri
JavaScript structural veri tipleri 2 tanedir. Bunlar:
- [object](## "nesne")
- [function](## "fonksiyon")

### Değişken Tipini Öğrenme
JavaScript değişkeninin tipini öğrenmek için `typeof` operatörünü kullanırız.

```javascript
typeof("")            // string
typeof("Tekir")       // string
typeof(1907)          // number
typeof(19.07)         // number
```

## Primitive Veri Tipleri

### string Veri Tipi
JavaScript [string](## "metin")'leri `"kedi"` örneğinde olduğu gibi harflerden oluşur.

`string` veri tipleri çift `("")` veya tek `('')` tırnak arasına yazılır.

```javascript
let kediAdi1 = "Tekir";   // Cift tırnak kullanimi
let kediAdi2 = 'Boncuk';   // Tek tırnak kullanimi
```

`string` veri tipinde `string`'i çevreleyen tırnak dışında `string` içerisinde de tırnak kullanmak istersek farklı bir tırnak işareti kullanmamız gerekir.

```javascript
let metin1 = "Kedimin adı 'Tekir'";    // Cift tirnak içerisinde tek tirnak
let metin2 = 'Kedimin adı "Tekir"';    // Tek tirnak içerisinde cift tirnak
```

### number Veri Tipi
- JavaScript [number](##"sayı") veri tipinde sayıları ondalıklı ve ondalıksız sayılar olarak yazabiliriz.

```javascript
let x1 = 1907;     // Ondalıksız sayı
let x2 = 19.07;    // Ondalıklı sayı
```
- Çok büyük ve çok küçük sayılar [bilimsel](## "üstel") gösterimle yazılabilir.
(Yaygın kullanılan bir özellik değildir.)

```javascript
let y = 123e5;      // 12300000
let z = 123e-5;     // 0.00123
```

### [boolean](## "mantıksal") Veri Tipi
[boolean](## "mantıksal") veri tipleri yalnızca iki değere sahip olabilir:
- [true](## "doğru")
- [false](## "yanlış")

`boolean` veri tipleri genellikle koşullu durumlarda kullanılır.

```javascript
let elmaSayisi = 5;
let armutSayisi = 5;
let ayvaSayisi = 6;
(elmaSayisi === armutSayisi)       // true
(elmaSayisi === ayvaSayisi)       // false
```

### [undefined](## "tanımsız") Veri Tipi
JavaScript'te değer atanmayan değişkenler [undefined](## "tanımsız") olarak tanımlanır.

```javascript
let kedi;                // değişken değeri ve veri tipi undefined
let kedi = undefined;    // değişken değeri ve veri tipi undefined
```

### Boş Değerli string
Boş değerli string [undefined](## "tanımsız") veri tipinden farklıdır. Boş değerli string bir veri tipine ve bir değere sahiptir.

```javascript
let kedi = "";   // değişken değeri "", veri tipi string
```

### [null](## "boş") Veri Tipi
JavaScript [null](## "boş") veri tipi içeriği boş olan veri tipidir.

JavaScript'te önceden tanımlanmış değişkene [null](## "boş") değeri atayarak içeriğini boşaltabiliriz.

```javascript
let kediAdi = "Tekir";
kediAdi = null;   // kediAdi degiskeninin degeri artik null
```

### [null](## "boş") ve [undefined](## "tanımsız") Veri Tipi Farkları
- Bir değişkene olmayan bir değer atamak için [null](## "boş") veri tipini, bir değişken [bildirildiğinde](## "yeni bir değişken oluşturulduğunda") ancak bir değer atanmadığında [undefined](## "tanımsız") veri tipini kullanırız.

- Değişken [null](## "boş") olarak atandığında, değer [null](## "boş") olur, değişken [undefined](## "tanımsız") olarak atandığında, değer [undefined](## "tanımsız") olur.

- Değişken [null](## "boş") olarak atandığında, veri tipi sorgusunun sonucu [object](## "nesne") olur, değişken [undefined](## "tanımsız") olarak atandığında, veri tipi sorgusunun sonucu [undefined](## "tanımsız") olur.

## Structural Veri Tipleri

### [object](## "nesne") Veri Tipi
JavaScript [object](## "nesne") veri tipi [key:value](## "anahtar:değer") çifti elemanlardan oluşur, süslü parantezle`{}` tanımlanır ve her eleman virgülle ayrılarak yazılır.

Örneğin;

```javascript
const kedi = {ad:"Tekir", yas:2, gozRengi:"yeşil"};
```

### [array](## "dizi") Veri Tipi
JavaScript [array](## "dizi") veri tipi birden fazla elemandan oluşan veri topluluğudur.

** `array` veri tipi aslında `object` veri tipinin alt tipidir. Bu konuya `Nesne Tabanlı Programlama` bölümünde değineceğiz. 

JavaScript `array`'leri köşeli parantezlerle yazılır.

`array` elemanları virgülle ayrılır.

```javascript
const kediler = ["Tekir", "Boncuk", "Pamuk"];
```

`array` tipinde bir değişkenin elemanlarına ulaşmak istediğimizde elemanların bulunduğu [index](## "sıra") kullanılır. `array`'lerde ilk elemanın `index`'i `0` ile başlar; yani yukardaki örnekte ilk elemana `kediler[0]`, ikinci elemana `kediler[1]` ile ulaşırız.

### [function](## "fonksiyon") Veri Tipi
`function` veri tipini `JavaScript Fonksiyonlar` bölümünde detaylı olarak açıkladık.


#### Kaynakça

[w3schools JavaScript Data Types](https://www.w3schools.com/js/js_datatypes.asp)

[JavaScript'te null ve undefined Arasındaki Fark](https://tr.strephonsays.com/null-and-vs-undefined-in-javascript-7311#:~:text=Veriler%20de%C4%9Fi%C5%9Fkenler%20halinde%20saklan%C4%B1r.,ancak%20bir%20de%C4%9Fer%20atanmad%C4%B1%C4%9F%C4%B1nda)

[JavaScript data types and data structures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#primitive_values)





