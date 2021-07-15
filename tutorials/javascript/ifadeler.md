## JavaScript Komutları

Bilgisayar programları, bilgisayarlar tarafından işlenmek üzere yazılmış talimatlardan oluşur. Bu talimatlara [komutlar](## "statements") denir.

Bir JavaScript programı, programlama komutlarının bir listesidir.

** HTML'de JavaScript programları web tarayıcısı tarafından yürütülür.

JavaScript komutları şunlardan oluşur:

- [Değerler](## "Values")
- [Operatörler](## "Operators")
- [İfadeler](## "Expressions")
- [Anahtar Kelimeler](## "Keywords")
- [Yorumlar](## "Comments")

Aşağıdaki örnekteki komut tarayıcıya `id="demo"` içeren bir HTML elemanının içinde `"Merhaba Dünya"` yazmasını söyler.

```javascript
document.getElementById("demo").innerHTML = "Merhaba Dünya";
```

Çoğu JavaScript programı birçok JavaScript komutu içermektedir, bu komutlar yazıldıkları sırayla birer birer yürütülmektedir.

** Belirli bir görevi yerine getirmek üzere yazılan JavaScript komutları bütününe [script](## "betik") deriz.

### Noktalı Virgül(;)
JavaScript komutlarını `noktalı virgül(;)` ile sonlandırırız.

Eğer bir komut tek satırda ifade ediliyor ise satırın sonuna `noktalı virgül(;)` koyarız.

```javascript
let a, b, c;  // 3 değişken bildirelim
a = 5;        // 5 değerini a'ya atayalım
b = 6;        // 6 değerini b'ye atayalım
c = a + b;    // a ve b'nin toplamını c'ye atayalım
```

Aynı satırdaki komutlar arasına `noktalı virgül(;)` koyarak komutların birbirinden ayrılmasını sağlayabiliriz. Ancak bu yaygın bir kullanım değildir.

```javascript
a = 5; b = 6; c = a + b;
```

** Noktalı virgül içermeyen JavaScript kodları görebilirsiniz, JavaScript kodlarını `noktalı virgül(;)` ile bitirmek bir [best practice](## "genelgeçer kullanım alışkanlığı")'tir.

### JavaScript White Space(Boşluk)
JavaScript fazladan kullanılan boşlukları yok sayar.

Kodları daha okunabilir hale getirmek için boşluk kullanırız.

Aşağıdaki örnekte satırlar eşdeğerdir:

```javascript
let kedi = "Tekir";
let kedi="Tekir";
```

Operatörlerin ( = + - * / ) etrafına boşluk koymak her zaman tercih edilen bir yöntemdir.

### JavaScript Satır Uzunluğu ve Satır Sonları
Programcılar en iyi okunabilirlik için genellikle `80 karakterden` uzun olan kod satırlarından kaçınırlar.

Bir JavaScript komutu bir satıra sığmıyorsa, onu alt satıra geçirmek için en iyi yer bir operatörden sonradır:

```javascript
document.getElementById("demo").innerHTML =
"Merhaba Dünya!";
```

### JavaScript Kod Blokları
JavaScript komutları bir araya gelerek `kod blokları`'nı oluşturur.

Kod bloklarının amacı, birlikte yürütülecek komutları tanımlamaktır.

Kod blokları `süslü parantez{}` ile kullanılır.

Kod blokları için en güzel örnek `JavaScript fonksiyonlarıdır`.

```javascript
function myFunction() {
  document.getElementById("demo1").innerHTML = "Merhaba Dünya";
  document.getElementById("demo2").innerHTML = "Merhaba JavaScript";
}
```

### JavaScript [Keywords](## "Anahtar Kelimeler")
JavaScript komutları, gerçekleştirilecek JavaScript eylemini tanımlamak için genellikle bir `anahtar kelime` ile başlar.

Bu eğitimde öğreneceğimiz bazı anahtar kelimeler aşağıda listelenmiştir:

| Keyword    | Açıklama                                                     |
|------------|--------------------------------------------------------------|
| `var`      | Bir değişken bildirir                                        |
| `let`      | Bir blok değişkeni bildirir                                  |
| `const`    | Bir blok sabiti bildirir                                     |
| `if`       | Bir koşulda yürütülecek bir komut bloğunu işaretler          |
| `switch`   | Farklı durumlarda yürütülecek bir komut bloğunu işaretler    |
| `for`      | Bir döngüde yürütülecek bir komut bloğunu işaretler          |
| `function` | Bir işlev bildirir                                           |
| `return`   | Bir işlevden çıkar                                           |
| `try`      | Bir komut bloğuna [error handling](## "hata işleme") uygular |

** JavaScript anahtar kelimeleri JavaScript'e ayrılmış kelimelerdir. [Ayrılmış kelimeler](## "reserved words") değişkenler için isim olarak kullanılamaz.


#### Kaynakça

[w3schools JavaScript Statements](https://www.w3schools.com/js/js_statements.asp)