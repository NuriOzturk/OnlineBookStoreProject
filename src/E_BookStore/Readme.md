# Book Listesine Ekleme-Çıkarma İşlemleri:
### Bu projemizde bizden, online book satışı yapan bir mağazanın ürün listesine ekleme çıkarma yapabilen bir modül tasarlanması istenmiştir. 

Projenin Örnek Ağaç Yapısı Aşağıdaki Gibi Olabilir :
```markdown
src
├───bookStore
│       Book.java
│       OnlineBookStore.java
│       Readme.md
│       Proje7.Shape.Proje7.School.Runner.java
```

1. Java programlama dilinde, kullanıcıya book eklemesi, book silmesi ve mevcut kitapları listelemesi için bir uygulama geliştirmeniz istenmektedir. Bu uygulama içerisinde aşağıdaki kavramları kullanmanız beklenmektedir:
--- 
- Bir `Book` sınıfı oluşturun. Bu sınıf, book adı, yazar adı, yayın yılı ve price gibi özellikleri (`fields`) içermelidir. Book numarası (id'si) otomatik ve sıralı bir şekilde yegane (unique) olarak (`static`) atanmalıdır.
---
- Bir `OnlineBookStore` sınıfı oluşturun. Bu sınıf, kitapları bir dizi (array) içerisinde tutmalıdır. Kullanıcıdan alınan girdilere göre book ekleme, book silme ve kitapları listeleyebilme metotları içermelidir. Book silme fonksiyonu, silinecek kitabın listede olup olmadığını kontrol etmelidir. Silinecek book listede yoksa, "_**Belirtilen numarada bir book bulunamadı.**_" gibi bir mesajı konsolda göstermelidir. 
- Bu sınıfın aşağıdaki gibi field ve methodları olmalıdır:

```java
class OnlineBookStore {
    private ArrayList<Book> kitapListesi = new ArrayList<>();
    private Scanner scanner = new Scanner(System.in);

    public void kitapEkle() {...}

    public void kitapSil() {...}

    public void kitapListele() {...}
}
```
---
- Bir menü oluşturun. Menü, kullanıcıya aşağıdaki gibi seçenekleri sunmalıdır:
```
  ============ Online Book Mağazası ============
    1. Book Ekle
    2. Numarasıyla Book Sil
    3. Tüm Kitapları Listele
    4. Çıkış
```
- Kullanıcı bir seçenek belirlediğinde, ilgili işlemi gerçekleştirmek için uygun methodları çağırın.
- Programın sürekli çalışmasını sağlayın, yani kullanıcı çıkış seçeneğini seçene kadar program çalışmaya devam etmelidir.
- Müşteri farklı bir seçenek seçtiğinde "_Geçersiz bir seçim yaptınız. Lütfen tekrar deneyin._" mesajı almalıdır.
2. Bu görevi yerine getiren bir Java programı yazınız.
