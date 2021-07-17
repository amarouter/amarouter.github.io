## JavaScript Yorumlar
Yazılan JavaScript kodlarını açıklamak ve kod okunurluğunu arttırmak için JavaScript yorumlarını kullanırız.

JavaScript yorumlarını, [alternatif kodun](## "Geliştirme esnasında kodun bir kısmını değiştirmeden önce yeni versiyonu da yazılabilir, böylece sonradan iki versiyon arasında seçim yapılabilir.") test sırasında çalışmasını önlemek için de kullanabiliriz.

### Tekli Yorum Satırı
Tekli yorum satırları için `iki eğik çizgi //` kullanırız.

`İki eğik çizgi //` sonrasında yazılan kodlar yorum satırı olarak yorumlanacak ve JavaScript tarafından çalıştırılmayacaktır.

Aşağıdaki örneklerde her JavaScript kodu öncesinde kodun ne yapacağı hakkında bilgi yorum satırı olarak verilmiştir:

```javascript
// Basligi degistirir.
document.getElementById("myHeader").innerHTML = "Benim İlk Başlığım";

// Paragrafi degistirir.
document.getElementById("myParagraph").innerHTML = "Benim ilk paragrafım.";
```

Aşağıdaki örnekte ise kod sonrasında kodun ne yapacağı hakkında bilgi yorum satırı olarak verilmiştir:

```javascript
let x = 5;      // x degiskenine 5 degeri atandi.
let y = x + 2;  // y degerine x+2 degeri atandi.
```

### Çoklu Yorum Satırı
Çoklu yorum satırları `/*` ile başlar ve `*/` ile biter.

JavaScript `/*` ve `*/` arasında yazılanları çalıştırmayacaktır.

```javascript
/*
Asagidaki kod id'si "myHeader" olan basligi
ve id'si "myParagraph" olan paragrafi degistirir.
*/
document.getElementById("myHeader").innerHTML = "Benim İlk Başlığım";
document.getElementById("myParagraph").innerHTML = "Benim ilk paragrafım.";
```

** Tekli yorum satırlarının kullanımı daha yaygındır.

### Kodları Devre Dışı Bırakmak İçin Yorum Satırı Kullanma
JavaScript ile kod yazarken çalışmasını istemediğimiz kodları devre dışı bırakmak için yorum satırlarını kullanabiliriz.

Tek satırlık kodu devre dışı bırakmak:

```javascript
//document.getElementById("myHeader").innerHTML = "Benim İlk Başlığım";
document.getElementById("myParagraph").innerHTML = "Benim ilk paragrafım.";
```

Çok satırlı kodu devre dışı bırakmak:

```javascript
/*
document.getElementById("myHeader").innerHTML = "Benim İlk Başlığım";
document.getElementById("myParagraph").innerHTML = "Benim ilk paragrafım.";
*/
```

#### Kaynakça

[w3schools JavaScript Comments](https://www.w3schools.com/js/js_comments.asp)