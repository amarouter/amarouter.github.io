<center><img  src="./images/jsarraymethod3.png" alt="en çok kullanılan method image" width="600"/>
</center>
<br>

<center>

# JavaScript En Çok Kullanılan Array Method'ları - 3

</center>

## concat Method'u

`concat` method'u bir yada daha fazla Array'i birleştirmeyi sağlar. `concat` immutable bir method'dur. Bu özellik bize mevcut Array'lerimizin değişmediğini ifade eder.

```javascript
let meyveler = ["🍎", "🍌", "🍉"];

let sebzeler = ["🥕", "🥦", "🥒"];

const birlestir = meyveler.concat(sebzeler);

console.log(birlestir); // [ '🍎', '🍌', '🍉', '🥕', '🥦', '🥒' ]

console.log(meyveler); // [ '🍎', '🍌', '🍉' ]
console.log(sebzeler); // [ '🥕', '🥦', '🥒' ]
```

Burada göründüğü gibi üzerinde concat method'unu kullandığımız Array'ler değişmeyecektir.

## join Method'u

`join` method'u Array'in tüm elemanlarını içerisine String olarak verdiğimiz ayırıcı ile birleştirerek tek bir String değerine çevirir.
İçerisine ayırıcı vermeden sadece `.join()` olarak kullanırsak virgül ile tek bir String'e çevrilecektir.

Bunu örnek ile daha iyi anlayabiliriz.

```javascript
console.log(meyveler); // [ '🍎', '🍌', '🍉' ]

const tekString = meyveler.join();

console.log(tekString); // 🍎,🍌,🍉
```

join() method'u parantezler içerisine yazdığımız String değerini kullanarak birleştirme yapar.

```javascript
const tekEleman = meyveler.join("*");

console.log(tekEleman); // 🍎*🍌*🍉
```

`Dikkat` : Belirli bir ayırıcı ile birleşmiş olan String değerlerini tekrardan ayırarak Array'e çevirmek için String'in `split` method'unu kullanırız.

`Dikkat`: Eğer aradığımız eleman Array'in içerisinde yoksa `-1 ` döndürecektir.

```javascript
indexBul = rakamlar.indexOf(7);

console.log(indexBul); // -1
```

## reverse Method'u

`reverse` method'u Array'in tersini alacaktır. `reverse` method'u orijinal Array'i değiştirir.

```javascript
const tersiniAl = rakamlar.reverse();

console.log(tersiniAl); // [ 6, 5, 4, 3, 2, 1 ]
console.log(rakamlar); // [ 6, 5, 4, 3, 2, 1 ]
```

## sort Method'u

`sort` method'u Array'deki elementleri sıralamamızı sağlar. `sort` method'u orijinal Array'i değiştirir.

```javascript
let isimler = ["Recai", "Koray", "İzlimek"];

const sirala = isimler.sort();

console.log(sirala); // [ 'Koray', 'Recai', 'İzlimek' ]
console.log(isimler); // [ 'Koray', 'Recai', 'İzlimek' ]
```

```javascript
const karisikSayilar = [5, 6, 4, 2, 1, 0];

console.log(karisikSayilar.sort()); // [ 0, 1, 2, 4, 5, 6 ]
```

`Dikkat`: Eğer biz tersten sıralamak istiyorsak `reverse` metod'u ile beraber kullanabiliriz.

```javascript
console.log(karisikSayilar.sort().reverse()); // [ 6, 5, 4, 2, 1, 0 ]
```

## some Method'u

`some` method'u girilen koşul array içerisinde en az bir kere varsa `true` yoksa `false` döndürür.

```javascript
let array = [30, 50, 23, 21, 105];

const varMi = array.some((sayi) => {
    return sayi > 32;
});

console.log(varMi); // true
```

## every Method'u

`every` method'u içerisinde belirtilen koşul Array'deki tüm elemanlar tarafından sağlanıyorsa `true`, sağlanmıyorsa `false` döndürür.

```javascript
let array = [30, 50, 23, 21, 105];

// Belirtilen kosul sadece 1 eleman tarafindan saglaniyor,
// oysaki method'un true donebilmesi icin tum elemanlarin
// kosulu sagliyor olmasi gerekir.
const saglanmaz = array.every((sayi) => {
    return sayi > 50;
});

console.log(saglanmaz); // false

const saglanir = array.every((sayi) => {
    return sayi > 20;
});

console.log(saglanir); // true
```


## Kaynakça

[Mozilla Array Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array?retiredLocale=tr)
