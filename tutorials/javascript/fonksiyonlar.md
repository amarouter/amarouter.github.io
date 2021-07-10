## JavaScript Fonksiyonlar
JavaScript'te fonksiyonlar, belirli bir görevi gerçekleştirmek için tasarlanmış kod bloklarıdır.

JavaScript ile yazılmış bir fonksiyonu çağırdığımızda fonksiyon çalışır ve işlem yapar.

```javascript
function carp(sayi1, sayi2) {
  return sayi1 * sayi2;   // fonksiyon sayi1 ve sayi2'nin çarpımını döndürür.
}
```

### Fonksiyon [Sözdizimi](## "Syntax")
Sözdizimi, bir dilin ifade ediliş biçimidir. JavaScript sözdizimlerini doğru kullanmazsak kendimizi bilgisayara ifade edemeyiz. Bilgisayar da [bizi anlamadığını söyler](## "uygulama hata verir.").
- JavaScript'te fonksiyonu; `function` anahtar kelimesi, `fonksiyon adı` ve parantez `()` ile oluştururuz.

- Fonksiyon adlarında; harf, rakam, alt çizgi`(_)`, dolar işareti`($)` kullanabiliriz.(değişken tanımlama kuralları ile aynı)

- Fonksiyona girdi olarak kullandığımız değişkenleri `parametre`, fonksiyon çağrılırken gönderdiğimiz değerleri ise `argüman` olarak adlandırırız.

- Fonksiyon parametrelerini fonksiyon içerisinde `yerel değişken` gibi kullanırız.

- Fonksiyon parametrelerini parantez içerisinde virgülle ayırarak kullanabiliriz.
(parametre1, parametre2,...)

- Fonksiyon kodlarını süslü parantez`{}` içine yazarız.

```javascript
function fonksiyonAdi(parameter1, parameter2, parameter3) {
  // fonksiyon kodlari
}
```

### Fonksiyon Çağırma
JavaScript ile yazılmış fonksiyon kodlarını çalıştırmak için fonksiyon çağırma işlemini yaparız.

JavaScript'te fonksiyon çalıştırmanın yolları aşağıda sıralanmıştır:

- Bir olay meydana geldiğinde(örneğin, kullanıcı bir butona tıkladığında)
- Fonksiyon çağrılma işlemi yapıldığında 
- Otomatik olarak(fonksiyon içinde fonksiyon çağırma gibi)

** JavaScript büyük-küçük harf farkına duyarlıdır, bu yüzden fonksiyon adları tanımlarken ve fonksiyon çağrılırken harflerin büyük, küçük oluşuna dikkat etmemiz gerekir.

### Fonksiyon Değer Döndürme
Fonksiyonlar `return` anahtar kelimesi ile değer döndürür.

JavaScript'te bir fonksiyon çalışırken `return` anahtar kelimesine geldiğinde `return` işlemini yaptıktan sonra fonksiyonun işi biter. Uygulama çalışmaya fonksiyonun çağrıldığı yerden devam eder ve varsa kalan kodları işler.

```javascript
let x = carp(4, 3);   // Fonksiyon cagrilir, donen deger x'e atanir.

function carp(a, b) {
  return a * b;    // Fonksiyon a ve b'nin carpimini doner.
}
```

### Neden Fonksiyon
Fonksiyonlar bir işlevi yerine getiren kod bloklarıdır. 
Eğer bir projede birden fazla yerde çalışmasını istediğimiz kodlar varsa fonksiyonları kullanırız. Aynı kodu bir kez yazarak birden fazla yerde kullanabildiğimiz için kod tekrarının önüne geçmiş oluruz.

### Fonksiyon Nesnelerini Değişkene Atama ve Atanan Değişken Üzerinden Çağrılması

Aşağıdaki örnekte farklı değerleri parametre olarak alan ve hesaplama yapan `besCikar` fonksiyonu tanımlanmıştır.

```javascript
function besCikar(cikarilacakSayi) {
  return cikarilacakSayi - 5;
}

let besCikarmaIslemi = besCikar; 

let sonuc = besCikarmaIslemi(13);  // Fonksiyon burada cagrilir ve sonuc'un degeri 8 olur.
```


#### Kaynakça

[w3schools JavaScript Functions](https://www.w3schools.com/js/js_functions.asp)