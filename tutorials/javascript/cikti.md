## JavaScript Çıktısı(Ekrana Yazdırma)
JavaScript'te verileri ekrana farklı şekillerde yazdırabiliriz:

- HTML elemanının yazısını değiştirmek için `innerHTML`,
- Uyarı penceresine yazdırmak için `alert()`,
- Tarayıcı konsoluna yazdırmak için `console.log()`,
- `document.open()` tarafından açılan bir belge akışına bir metin dizesi yazmak için `document.write()`.

### innerHTML Kullanımı
JavaScript ile HTML nesnelerini seçmek için `document.getElementById()` method'u kullanılır.
Seçme işleminden sonra `innerHTML` özelliği ile seçilen HTML nesnesinin içeriği değiştirilebilir.

```html
<p id="demo"></p>

<script>
  document.getElementById("demo").innerHTML = 11;
</script>
```

### alert() Kullanımı
JavaScript verilerini uyarı mesajı olarak ekrana yazdırmak için `alert()` method'u kullanılır.

```html
<p>Benim ilk paragrafım.</p>

<script>
  alert("Şifrenizi mi unuttunuz?");
</script>
```

### console.log() Kullanımı
`console.log()` method'u genellikle verileri  ekrana yazdırmak için kullanılır. [Hata ayıklama](## "Koddaki hatayı tespit etme") işlemi için de en sık kullanılan yöntemdir.
Sonucu görüntüleyebilmek için konsol ekranınızın aktif olduğuna emin olun.

### document.write() Kullanımı 
JavaScript komutlarını test etmek amacıyla kullanılır.

```html
<p>Benim ilk paragrafım.</p>

<script>
  document.write(11);
</script>
```

`document.write()` method'u bir HTMl belgesi yüklendikten sonra kullanılırsa mevcut tüm HTML elamanları silinir.

```html
<p>Benim ilk paragrafım.</p>

<button type="button" onclick="document.write(11)">Dene</button>
```

#### Kaynakça
[w3schools JavaScript Output](https://www.w3schools.com/js/js_output.asp)
