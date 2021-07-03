## JavaScript Değişkenler
JavaScript dilinde değişkenler veri depolamak için kullanılır.

### Değişken Tanımlama Kuralları
- Değişken ismi sayısal ifade ile başlayamaz.
- Değişken isimleri harf, alt çizgi veya dolar işareti($) ile başlayabilir.
- [Reserved kelimeler](## "JavaScript için ayrılmış kelimeler") değişken adı olarak kullanılamaz.(var,while,if...)
- Birden fazla kelimeden oluşan değişken tanımlarken [best practise](## "genelgeçer kullanım alışkanlığı") olarak [Camel Case](## "Birden çok kelimeden oluşan değişken veya fonksiyon tanımlanırken ilk kelimenin baş harfi küçük ve diğer bütün kelimelerin baş harfi büyük olacak şekilde bitişik tanımlama yapılarak kullanılır.") kullanılır.(arabaRengi)
- Değişken isimleri [büyük/küçük harf duyarlıdır](## "arabaRengi ve ArabaRengi farklı değişkenlerdir").

### Değişken Tanımlama 
JavaScript'te değişken tanımlamanın 3 yolu vardır. Bunlar:
- var
- let
- const 

anahtar sözcükleridir.
Tüm JavaScript değişken isimleri benzersiz olmalıdır.
JavaScript değişken isimleri [identifier](## "tanımlayıcı") olarak adlandırılır.

### Atama Operatörü
JavaScript ile tanımlanan değişkene değer atamak için "eşittir" `(=)` operatörü kullanılır.
```javascript
var a = 10;
```
`a` değişkeninin değeri `10` oldu.

### Değişken Türleri
JavaScript değişkenleri `70` gibi [number](## "sayısal") bir değer alabileceği gibi `kedi` gibi [string](## "metinsel") bir değer de alabilir.
`string` değerler tek tırnak ya da çift tırnak arasına yazılırken `number` değerler tırnak arasına alınmadan yazılır.
`number` değerler tırnak içine alınırsa JavaScript değeri `string` ifade olarak tanımlanacaktır.

### Değişken Oluşturmak
JavaScriptte değişken oluşturma `değişken tanımlama` olarak adlandırılır.
Değişken oluştururken sırayla `var/let/const` anahtar kelimelerinden biri, değişken ismi(tanımlayıcı), değişken operatörü(=) ve atamak istediğimiz değer olmalıdır. Örneğin:
```javascript
var catName = "Tekir";
```

### Tanımsız Değişkenler
Eğer değişken tanımlanırken değişkene değer atanmazsa o değişken [undefined](## "tanımsız") değerini alır.

### Değişkenlere Yeni Değer Atamak
Önceden tanımlanmış bir değişkene yeni değer atanırsa değişken atanan yeni değeri alır.
```javascript
catName = "Boncuk";
```
`catName` değişkeninin değeri artık `Boncuk` oldu.

### JavaScript Değişken Aritmetiği
JavaScript değişkenleri ile işlemler yapmak için aritmetik operatörleri kullanabiliriz.

```javascript
var elmaSayisi = 5;
var armutSayisi = 3;
var meyveSayisi = elmaSayisi + armutSayisi;
alert(meyveSayisi);
```

#### Kaynakça

[w3schools JavaScript Variables](https://www.w3schools.com/js/js_variables.asp)
