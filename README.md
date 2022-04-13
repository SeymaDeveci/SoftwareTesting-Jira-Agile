# SoftwareTesting-Jira-Agile
 Agile ve Traditional Software Development Lifecycle'da gereksinimleri toplamayı ve Jira, Bugzilla araçlarının kullanımı öğrenmeyi içerir.

## Kredi Kartı Online Bankacılık Uygulaması
Üzerinde çalıştığım proje kredi kartı online bankacılık uygulaması üzerinde bir çalışma gerçekleştirdim. Bu projede ihtiyacım olan özellikler :
- Develop Login Module (Oturum Açma Modülü)
- Credit Card Dashboard (Kredi Kartı Kontrol Paneli)
- Profile (Profil)

### Amaç 
- Özelliklerde neyin kullanılacağına karar vermek,
- Nasıl geliştirileceğine ve geliştirilecek stratejinin ne olduğuna karar vermek,
- Özellikleri uygulamak için Agile ekibini etkin bir şekilde kullanmak,
- Projede Jira aracını kullanmak ve projeyi yönetmek.

### Projede Boyunca Yapılanlar

#### Jira'da Epic Oluşturma : 
Epic, daha küçük kullanıcı hikayelerine veya görevlerine bölünebilen büyük bir çalışma grubudur.

Birkaç sprint boyunca veya uzun bir süre boyunca tamamlanması gereken büyük bir çalışma grubu için ***epic*** oluşturuldu. ***Epic ismi*** ve ***özet bilgisi*** girildi. Backlog (Biriktirme Listesinde) epic oluşturuldu. (Backlog > Epics > Create epic)

#### Kullanıcı Hikayesi Oluşturma :
User story bir kullanıcının bir yazılımı, bir ürünü ya da hizmeti kullanırken yapmayı hedeflediği şeyi açıklamaya yarayan senaryolardır. User story kısa, bir cümle uzunluğunda olmalıdır. "As a person......, I want to ......., so that......" kısımlarını içermelidir. 

Örnek: Ben kredi kartı bankacılık uygulamasının bir müşterisi olarak kullanıcı adı ve şifre ile giriş yapmak istiyorum. Böylece güvenle portala giriş yaparak para gönderebilirim.

#### Component (Bileşen) Oluşturma :
Bileşenler, projenizdeki sorunları segmentlere ayırmanın yanı sıra sürecinizi düzene koymanıza yardımcı olacak benzersiz özelliklere sahip özel alanlardır. Sorunları UI, API, Hardware vb. gibi daha küçük alt bölümlere ayırmak için kullanılabilir. 

Bu projede belirli bir ekibe özel hikayeleri atamak için componenet öğesi olan ***Team 1*** oluşturuldu. Kullanıcı hikayelerinin Takım 1'e ait olduğunu belirtmek için geçerli olan kullanıcı hikayesinde component olarak Team 1 öğesi seçildi.

![component create](https://user-images.githubusercontent.com/42176018/163253283-c40f1664-f9f4-4459-b047-63044b7fc5e5.png)

![component ekleme](https://user-images.githubusercontent.com/42176018/163253319-7e1edf1f-f306-4ce3-95ba-9f15729e43ba.png)

#### Release (Sürüm, Yayın İzni) Oluşturma :
Özelliklerin müşterilerinize nasıl sunulacağını planlamak veya proje için tamamlanmış işleri düzenlemenin bir yolu olarak kullanılabilirler. Belirlenen tarihte hangi kullanıcı hikayeleri ve işleri yayınlayacağımız belirlenmiş olur. O tarihte yayınlanacak işleri görmek için geçerli sürüme bakılır.

Login modülü için bir release oluşturuldu. Hedef yayın tarihi olarak 26 Nisan belirlendi.

![releases](https://user-images.githubusercontent.com/42176018/163256780-8f139485-7ed2-4c5a-aca0-b2835dc91a8a.png)

![Ekran Görüntüsü (342)_LI](https://user-images.githubusercontent.com/42176018/163257489-a88f6aac-d82f-4643-9264-762152842a84.jpg)

