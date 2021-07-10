## JavaScript [Object'ler](## "Nesneler")

### Gerçek Hayat Nesneleri, Özellikleri ve Method'ları
Nesneler her [Object Oriented Programming](## "Nesne Tabanlı Programlama") dillerinde yer alır. Nesneler JavaScript'e özgü değildir.

JavaScript'teki nesneler gerçek hayattaki nesnelerle karşılaştırılabilir. Nesneler kavramı gerçek hayattaki somut nesnelerle daha iyi anlaşılabilir.

Şimdi JavaScript nesnelerini gerçek hayattan örnekler vererek açıklayalım.

Gerçek hayatta, araba bir `nesne`dir. Bir arabanın ağırlık, renk gibi `özellikleri` ve motoru çalıştır, gaz ver, motoru durdur gibi `method'ları` vardır.

| Özellikler            | Method'lar             |
|-----------------------|------------------------|
| araba.marka = Fiat    | araba.motoruCalistir() |
| araba.model = 500     | araba.gazVer()         |
| araba.agirlik = 850kg | araba.frenle()         |
| araba.renk = beyaz    | araba.motoruDurdur()   |

Tüm arabalar benzer özelliklere sahiptir, ancak `özellik değerleri` arabadan arabaya farklılık gösterir.

Tüm arabalar benzer method'lara sahiptir, ancak method'lar farklı zamanlarda gerçekleşir.

### Nesneler
JavaScript değişkenlerini veri değerlerini depolamak için kullanırız.

Aşağıdaki örnekte araba isimli değişkene tek bir değer olan `Fiat` atanmıştır:

```javascript
let araba = "Fiat";
```

Nesneler de değişkendir, ancak nesnelere birden fazla değer atayabiliriz.

Aşağıdaki örnekte araba isimli değişkene birden fazla değer atanmıştır:

```javascript
const car = {marka:"Fiat", model:"500", renk:"siyah"};
```

** Nesneleri `const` anahtar kelimesi ile kullanmak daha çok tercih edilen bir yöntemdir.

### Nesne [Property'leri](## "Özellikleri")
JavaScript'te nesneleri [key:value](## "anahtar:değer") olarak tanımlarız.

```javascript
const kedi = {kediAdi:"Tekir", yas:2, gozRengi:"yesil"};
```

JavaScript nesnelerindeki key:value çiftine [property](## "özellik") deriz.

| Özellik  | Özellik Değeri |
|----------|----------------|
| kediAdi  | Tekir          |
| yas      | 2              |
| gozRengi | yesil          |

### Nesne Özelliklerine Erişim
JavaScript nesne özelliklerine iki şekilde erişebiliriz.

- `nesneAdi.ozellikAdi`

Örneğin;

```javascript
kisi.soyAdi;
```

veya

- `nesneAdi["ozellikAdi"]`

Örneğin;

```javascript
kisi["soyAdi"];
```
şeklinde erişebiliriz.

### Nesne Method'ları
Nesnelerin method'ları vardır ve bu method'lar nesneler üzerinde gerçekleştirdiğimiz eylemlerdir.

JavaScript nesneleri özellik ve method'ları saklayan veri türüdür.

JavaScript nesne method'larını nesne özelliklerinde `function` olarak saklarız.

| Özellik        | Özellik Değeri |
|----------------|----------------|
| isim           | İsa            |
| soyisim        | Kilikya        |
| yas            | 26             |
| getIsimSoyisim | function() {return this.isim+""+this.soyisim;}|

### Nesne Method'larına Erişim
JavaScript'te nesne method'larına aşağıdaki gibi erişebiliriz.
- `nesneAdi.methodAdi()`

Örneğin;

```javascript
isimSoyisim = kisi.getIsimSoyisim();
```

JavaScript'te nesne method'larına erişirken parantez`()` eklemezsek fonksiyon tanımını döndürür.

```javascript
isimSoyisim = kisi.getIsimSoyisim;
```

#### Kaynakça
[w3schools JavaScript Objects](https://www.w3schools.com/js/js_objects.asp)