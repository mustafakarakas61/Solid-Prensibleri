# SOLID Prensibleri - ÖZET

|Prensib | Özet |
|---|---|
|**1.** `Single Responsibility Principle` (Tek Sorumluluk Prensibi)|Bir sınıf sadece bir işten sorumlu olmalıdır.|
|**2.** `Open/Closed Principle` (Açık/Kapalı Prensibi)|Bir sınıf genişletilmeye açık ama değiştirmeye kapalı olmalıdır.|
|**3.** `Liskov Substitution Principle` (Liskov Yerine Geçme Prensibi)|Bir alt sınıf, üst sınıfın yerini alabilmeli ve programın doğru çalışmasını sağlamalıdır.|
|**4.** `Interface Segregation Principle` (Arayüz Ayrımı Prensibi)|Bir arayüz, yalnızca o arayüzü kullananlara özel yöntemler içermelidir.|
|**5.** `Dependency Inversion Principle` (Bağımlılıkların Ters Çevrilmesi Prensibi)|Sınıflar, somut sınıflara değil, soyutlamalara bağımlı olmalıdır.|

### Örnekler

#### **1.** `Single Responsibility Principle`
```java
class User {
    private String name;
    private String email;

    // Getters and Setters
}

class EmailService {
    public void sendEmail(String email, String message) {
        System.out.println("Email sent to " + email + " with message: " + message);
    }
}
```

**Yanlış:** User sınıfının hem kullanıcı hem de e-posta işlemlerini yapması.
**Doğru:** İşlemleri farklı sınıflara ayırmak.

# TODO: README will be update...
