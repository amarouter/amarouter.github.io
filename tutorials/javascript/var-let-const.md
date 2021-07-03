## var, let ve const Farkları

### var
 `var` ile oluşturulan değişkenler function scope özelliği taşımaktadır. 
 Yani fonksiyon içerisinde oluşturulan değişkenlere o fonksiyon içerisinde herhangi bir yerden erişilebilir.
 `var` ile tanımlanan bir değişken tekrar tanımlanabilir ve değerleri güncellenebilir.

### let
`let` ile oluşturulan değişkenler block scope özelliği taşımaktadır.
Yani `let` ile oluşturulan bir değişkene sadece oluşturulduğu yerdeki süslü parantezler içerisinde erişilebilir ve o değişken süslü parantez dışında kullanılamaz.
`let` ile tanımlanan bir değişken tekrar tanımlanamaz ancak değeri güncellenebilir.

### const
`const` ile oluşturulan değişkenler block scope özelliği taşımaktadır.
Yani `const` ile oluşturulan bir değişkene sadece oluşturulduğu yerdeki süslü parantezler içerisinde erişilebilir ve o değişken süslü parantez dışında kullanılamaz.
`const` ile oluşturulan bir değişkene daha sonra farklı bir değer atanamaz.
`const` ile oluşturulan değişkenlere [immutable](## "değişmez") değişkenler denir.

`Daha fazla bilgi ve örnekler için Kaynakça bölümündeki yazılara göz atabilirsiniz.`

#### Kaynakça
[Medium JavaScript JavaScript — var-let-const nedir? Aralarındaki Farklar Nelerdir?](https://medium.com/kodcular/javascriptte-var-let-const-nedir-aralar%C4%B1nda-ki-farklar-nelerdir-3b1f6c9e23cd)

[w3schools JavaScript Variables](https://www.w3schools.com/js/js_variables.asp)

[w3schools JavaScript Let](https://www.w3schools.com/js/js_let.asp)

[w3schools JavaScript Const](https://www.w3schools.com/js/js_const.asp)