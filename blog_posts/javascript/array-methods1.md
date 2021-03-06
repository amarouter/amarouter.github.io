<center><img  src="./images/jsarraymethod1.png" alt="en çok kullanılan method image" width="500"/>
</center>
<br>

<center>

# JavaScript En Çok Kullanılan Array Method'ları - 1

</center>

Array'ler JavaScript'teki en önemli veri yapılarından biridir. Array'ler sayesinde tek bir array değişkeninde liste şekinde elemanlar tutulabilir. Bununla beraber Array'lerin gerçek gücü method'larında yatmaktadır. Array method'ları Array'lerimize uygulayabileceğimiz JavaScript'in [built-in](## "gömülü") özellikleridir. Her method ya Array'imizde bir değişiklik yapar, ya da Array'imiz üzerinde hesaplamalar yapar.
Array method'ları serimizin birincisinde her [developer'ın](## "geliştiricinin") bilmesi gereken ve Array'ler üzerinde ekleme-çıkarma işlemleri yapan 6 method'dan bahsedeceğiz.

## push Method'u

`push` method'u Array'in sonuna yeni bir eleman eklemek için kullanılır.

```javascript
console.log(meyveler); // [ '🍎', '🍌', '🍉' ]
meyveler.push("🍓");
console.log(meyveler); // [ '🍎', '🍌', '🍉', '🍓' ]
```

## pop Method'u

`pop` method'u Array'in sonundaki elemanı çıkarır ve geriye çıkardığı elemanı döner.

```javascript
console.log(meyveler); // [ '🍎', '🍌', '🍉', '🍓' ]
const sonEleman = meyveler.pop();

console.log(meyveler); // [ '🍎', '🍌', '🍉' ]
console.log(sonEleman); // 🍓
```

## shift Method'u

`shift` method'u Array'in ilk elemanını çıkarır ve geriye çıkardığı elemanı döner. Aslında burada bir kaydırma işlemi yapılmaktadır.

```javascript
console.log(meyveler); // [ '🍎', '🍌', '🍉' ]

const ilkEleman = meyveler.shift();

console.log(meyveler); // [ '🍌', '🍉' ]
console.log(ilkEleman); // 🍎
```

`Dikkat`: Sıralama önemli ise `shift` method'u ile çıkarma yapılır. Sıralama önemli değilse `pop` method'u ile çıkarma yapılır. `pop` method'u `shift` method'undan daha hızlı çalışır.

## slice Method'u

`slice` method'u içine yazılan aralıktaki elemanların kopyasını döndürür. İçine değer girilmediği taktirde tüm elemanların kopyasını döndürecektir.

`slice(index1, index2)`

Arrayde elemanları almaya `index1`(dahil)'den baslayip `index2`(dahil değil)'ye kadar alacaktir.

```javascript
let sayilar = [0, 1, 2, 3, 4, 5, 6, 7];

console.log(sayilar.slice()); // [ 1, 2, 3, 4, 5, 6, 7 ]

console.log(sayilar.slice(1, 4)); // [ 1, 2, 3 ]
```

`Dikkat`: Burada orijinal Arrayde degişim olmayacaktır. Sadece kopyası alınır.

## unshift Method'u

`unshift` method'u Array'in başına yeni eleman ekler ve geriye eleman sayısını döner.

```javascript
meyveler = ["🍎", "🍌", "🍉"];

console.log(meyveler.unshift("🍓")); // 4
console.log(meyveler); // [ '🍓', '🍎', '🍌', '🍉' ]
```

## splice methodu

`splice` method'u kullanarak istediğimiz index'lerde elemanları değiştirebiliriz. `splice` method'u üç parametre alır.

`splice( index, silenecekElemanSayisi , eleman )`

`index`: Array'imizin değişmeye başlayacağı konumu gösterir. Burada elemanları silmeye `index`'ten başlarız. Elemanlar silindikten sonra yeni eklenecek elemanlar da yine bu `index`'ten itibaren eklenir.

`silenecekElemanSayisi`: İkinci girilen adet bilgisi ile kaç adet eleman silineceği bilgisi girilir.

`eleman`: Son olarak yeni eklenecek eleman girilir.

Bunu birer örnek ile anlayalım.

```javascript
let meyveler = ["🍎", "🍌", "🍉"];

meyveler.splice(1, 0, "🍇");

console.log(meyveler); // [ '🍎', '🍇', '🍌', '🍉' ]
```

Burada `silenecekElemanSayisi` olarak 0 yazıldığı için araya eklenmiş olur.

```javascript
console.log(meyveler); // [ '🍎', '🍇', '🍌', '🍉' ]
meyveler.splice(2, 1, "🍍");

console.log(meyveler); // [ '🍎', '🍇', '🍍', '🍉' ]
```

Burada `silenecekElemanSayisi` yerine 1 yazıldığı için `index` ikiden başlayıp sadece bir eleman değiştirilecektir.

`Dikkat`: splice method'u silinen elemanı geri döndürür.

```javascript
const silinen = meyveler.splice(0, 1, "🍒");

console.log(silinen); // [ '🍎' ]
console.log(meyveler); // [ '🍒', '🍇', '🍍', '🍉' ]
```

Eğer yeni eklenecek eleman yazmazsak sadece silme işlemi yapılacaktır.

```javascript
console.log(meyveler); // [ '🍒', '🍇', '🍍', '🍉' ]
meyveler.splice(3, 4);
console.log(meyveler); // [ '🍒', '🍇', '🍍' ]
```

## Bonus

## length Property

`length` aslında bir method değil ama çok sık kullanılan bir [property](## "özellik") olduğu için bonus olarak ekledik. Array'in eleman sayısını tutar.

```javascript
console.log(meyveler); // [ '🍎', '🍌', '🍉', '🍓' ]
console.log(meyveler.length); // 4
```

## Kaynakça

[Mozilla Array Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array?retiredLocale=tr)
