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

#### 1- Jira'da Epic Oluşturma : 
Epic, daha küçük kullanıcı hikayelerine veya görevlerine bölünebilen büyük bir çalışma grubudur.

Birkaç sprint boyunca veya uzun bir süre boyunca tamamlanması gereken büyük bir çalışma grubu için ***epic*** oluşturuldu. ***Epic ismi*** ve ***özet bilgisi*** girildi. Backlog (Biriktirme Listesinde) epic oluşturuldu. (Backlog > Epics > Create epic)

#### 2- Kullanıcı Hikayesi Oluşturma :
User story bir kullanıcının bir yazılımı, bir ürünü ya da hizmeti kullanırken yapmayı hedeflediği şeyi açıklamaya yarayan senaryolardır. User story kısa, bir cümle uzunluğunda olmalıdır. "As a person......, I want to ......., so that......" kısımlarını içermelidir. 

Örnek: Ben kredi kartı bankacılık uygulamasının bir müşterisi olarak kullanıcı adı ve şifre ile giriş yapmak istiyorum. Böylece güvenle portala giriş yaparak para gönderebilirim.

#### 3- Component (Bileşen) Oluşturma :
Bileşenler, projenizdeki sorunları segmentlere ayırmanın yanı sıra sürecinizi düzene koymanıza yardımcı olacak benzersiz özelliklere sahip özel alanlardır. Sorunları UI, API, Hardware vb. gibi daha küçük alt bölümlere ayırmak için kullanılabilir. 

Bu projede belirli bir ekibe özel hikayeleri atamak için componenet öğesi olan ***Team 1*** oluşturuldu. Kullanıcı hikayelerinin Takım 1'e ait olduğunu belirtmek için geçerli olan kullanıcı hikayesinde component olarak Team 1 öğesi seçildi.

![component create](https://user-images.githubusercontent.com/42176018/163253283-c40f1664-f9f4-4459-b047-63044b7fc5e5.png)

![component ekleme](https://user-images.githubusercontent.com/42176018/163253319-7e1edf1f-f306-4ce3-95ba-9f15729e43ba.png)

#### 4- Release (Sürüm, Yayın İzni) Oluşturma :
Özelliklerin müşterilerinize nasıl sunulacağını planlamak veya proje için tamamlanmış işleri düzenlemenin bir yolu olarak kullanılabilirler. Belirlenen tarihte hangi kullanıcı hikayeleri ve işleri yayınlayacağımız belirlenmiş olur. O tarihte yayınlanacak işleri görmek için geçerli sürüme bakılır.

Login modülü için bir release oluşturuldu. Hedef yayın tarihi olarak 26 Nisan belirlendi.

![releases](https://user-images.githubusercontent.com/42176018/163256780-8f139485-7ed2-4c5a-aca0-b2835dc91a8a.png)

![Ekran Görüntüsü (342)_LI](https://user-images.githubusercontent.com/42176018/163257489-a88f6aac-d82f-4643-9264-762152842a84.jpg)

#### 5- Kullanıcı Hikayelerinin Açıklama Kısmına Kabul Kriterlerini Ekleme :
Geçerli olan user story için açıklama kısmına (description) kısa bir tanım bilgisi ve kabul kriterleri (acceptance criteria) girildi.

Kabul kriterleri, bir kullanıcı hikayesini ***tamamlandı*** olarak işaretlemek için karşılanması gereken bir dizi önceden tanımlanmış gereksinimlerdir. Ürün sahibi belirli kullanıcı hikayesi kabul kriterlerini doğruladığında ve geliştirilen özellik bunu geçtiğinde, kullanıcı hikayesinin geliştirilmesi bir başarı olarak kabul edilir. Yani kullanıcı hikayesi kabul testinin temelini oluşturur.

Kabul kriterleri geliştirme ekibi ve ürün sahibi tarafından ortaklaşa geliştirilebilir. Kriterlerde teknik detaylara inilebilir.

![kullanıcı kabul kriterleri yazma](https://user-images.githubusercontent.com/42176018/163264524-a63d09a8-0a90-44f8-9ba0-22dd90607d5f.png)

#### 6- Grooming Toplantılarında Kullanıcı Hikayelerini Puanlama :
Agile modelinde her user story için fibonacci serisindeki sayılar gibi 1,2,3,5,8,13 gibi puanlar verilir. Bu puanlar yapılacak işin büyüklüğü, karmaşıklığı, içerdiği riskleri ve belirsizlikleri baz alınarak yapılır. En çok söylenen puan kabul görür ve Story Points kısmına yazılır.

Örnek projede geçerli user story için 3 puanının verildiğini varsaydım.

![Ekran Görüntüsü (345)_LI](https://user-images.githubusercontent.com/42176018/163267475-17911cfc-b921-4bed-bdf4-f90722b26696.jpg)

#### 7- Subtask (Alt Görev) Oluşturma :
Bir sorun için, sorunu daha küçük parçalara bölmek veya bir sorunun çeşitli yönlerinin farklı kişilere atanmasına izin vermek için bir ***subtask*** oluşturulabilir. Bu projede geliştirme, manuel test ve otomasyon test için alt görevler oluşturuldu. Bu görevlere ekipten birer kişi atandı.

![subtask oluştur](https://user-images.githubusercontent.com/42176018/163269189-9ea4ed58-c909-4d4f-aa72-aa2e5d74ee89.png)

#### 8- Sprint Ekleme :
***Sprint***, belirli bir zaman diliminde bitirmeyi hedeflediğimiz iş öğelerinin toplamıdır. Sprintler, sürekli geliştirme döngüsünün zaman kutu setidir. Scrum içerisindeki tüm aktiviteler sprint içerisinde gerçekleşir. 

Sprint planlaması ekip ile birlikte sprint başlamadan önce yapılmalıdır. Sprinte başlamadan önce gereksinimler detaylandırılmalı ve kullanıcı hikayeleri puanlanmalıdır. Sprint öncesi ortak bir anlayış oluşturulmalıdır. Bunun için Product Backlog Refinement (Grooming) toplantıları gerçekleştirilir.

Genellikle 10 günde bir bir sprint oluşturulur. Sprint için puan tahminlemesi yapılır. Ekibin hızı ve çabası baz alınarak puanlama yapılır. Oluşturulan sprinte önceliğe göre sıralanan kullanıcı hikayelerinden henüz gelişmemiş olanlar eklenir. Sprint için belirlenen puana dikkat edilerek kullanıcı hikayeleri eklenir.

Projede her sprint için 12 puanını belirlediğimizi düşündüm. Kullanıcı hikayelerini 12 puanı geçmeyecek şekilde eklemeye ve sprinti oluşturmaya çalıştım.

![Ekran Görüntüsü (347)](https://user-images.githubusercontent.com/42176018/163272501-1fb23dd8-25d0-4e33-8742-75f9bee98882.png)
