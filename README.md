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
Agile bir ortamda bir sprint tamamlandığında bir diğeri başlar. Bu durumda yaklaşan bir sonraki sprint için başlamadan önce hazır olmamız gerekir. Sprint sonuna yakın Grooming (Product Backlog Refinement) toplantısı yapılır. Product Owner önderliğinde Scrum Master ve Development Team katılmalıdır. Asıl amaç, bir sonraki sprint için ortak bir anlayış oluşturmaktır.

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

![Ekran Görüntüsü (350)](https://user-images.githubusercontent.com/42176018/163273351-82772f95-2690-4ff7-b1e2-f63e818c581b.png)


Oluşturulan Scrum Dashboard

![Ekran Görüntüsü (347)](https://user-images.githubusercontent.com/42176018/163272501-1fb23dd8-25d0-4e33-8742-75f9bee98882.png)

#### 9- Daily Stand Up Toplantısı :
Günlük olarak yapılan Scrum toplantısıdır. Development Team her gün 15 dakika ayırarak sprint hedefine ulaşırken yapacakları etkinlikleri senkronize eder ve sonraki 24 saat için bir plan geliştirir. Kaliteli bir ürünün ortaya çıkmasına katkı sağlar. Takım üyeleri arasındaki iş birliğini artırır ve yüksek motivasyon ile çalışnayı sağlar.

Amaç : Kendi kendine organize olan bir takımın sprint esnasındaki akışı daha iyi yönetebilmesidir. 

Product Owner'ın ve Scrum Master'ın bu toplantıya katılması zorunlu değildir.

#### 10- Retrospective Toplantısı :
Scrum takımının takımca yaptığı sprint veya genel iş akışının üzerine kişiler, ilişkiler ve araçlar kapsamında geriye yönelik bir değerlendirme ve iyileştirmedir. Takımın " Nasıl daha iyi yaparız? " sorusuna cevaplar bulduğu bir toplantıdır. Scrum takım üyeleri çalışma şekillerine dair negatif, pozitif olarak değerlendirdikleri tüm konuları açık yüreklilikle konuşurlar. Daha sonra konuşulan maddelere dair kök sebepler bulunmalı, aksiyonlar çıkmalı ve bu aksiyonlar takım tarafından takip edilerek hayata geçirilmelidir.

Retrospective araçları : 
- Mad / Sad / Glad Yöntemi
- Starfish Yöntemi

#### 11- Sprint Raporu Oluşturma :
Sprint’i kapattıktan sonra sistem doğrudan Sprint Report sayfasına götürecektir. Otomatik olarak sistem tarafından oluşturulan sprint raporunda tamamlanan işler ile Backlog'a gönderilen işler gösterilir.

![tamamlanan sprint](https://user-images.githubusercontent.com/42176018/163710305-ba582565-7723-4252-a9f8-88890e1e6e86.png)

![sprint raporu](https://user-images.githubusercontent.com/42176018/163710338-fdf6e61d-e35f-499b-aa9a-e850cf1ad3f4.png)

Velocity Chart, ekibin her sprintte tamamladığı işi gösterir. Böylece ekibin kapasitesini ölçebilir ve ileriye dönük planlama yapabiliriz.

![velocity chart](https://user-images.githubusercontent.com/42176018/163710376-23adfa1b-9aa8-401b-9536-6bbe8a31a8e9.png)

#### 12- Kanban Board Oluşturma :
Kanban bir agile proje yönetim tekniğidir. Kanban, bir süreç içinde hareket ederken işi yönetmek için kullanılan görsel bir sistemdir. 

Hem Scrum hem de Kanban büyük, karmaşık projeleri yönetilebilir parçalara ayırmanıza ve iş akışlarını tüm ekibi döngüde tutacak şekilde görselleştirmenize olanak tanır.

Kanban ve Scrum arasındaki en temel fark Kanban'da sprintlerin olmamasıdır. Bu yüzden sprint planlama toplantısına ihtiyaç yoktur. 

Kanban'da bir projenin yaşam döngüsü tek bir Kanban Panosu kullanılarak yapılır. Kanban panoları görevler ve zamanlama açısından daha esnektir.

Jira aracında oluşturduğum Kanban Panosu 

![Kanban board](https://user-images.githubusercontent.com/42176018/163711007-172c10e2-ada0-45f4-91e4-15e3c5e7b229.png)

#### 13- Parola Sıfırlama İşlevini Doğrulayan Test Senaryosu :
Parola sıfırlama işlevini doğrulamak için yazılmış test adımlarından oluşan basit bir senaryodur. Excel dosyasında yazılmıştır.

![ParolaSıfırlama](https://user-images.githubusercontent.com/42176018/164069121-c71f0d0d-9467-4d39-9d2e-2c54d9974a53.png)

####  14- Jira'da Xray Uygulamasına Giriş :
Xray, test planlamasından tasarım, uygulama ve test raporlamasına kadar bütün test döngüsünü yönetmek için tasarlanmıştır. Test yönetimi uygulamasıdır.

- Xray uygulamasının Jira'ya eklenmesi

![xray kurulumu](https://user-images.githubusercontent.com/42176018/164454004-dd3a2ca5-3b3e-49a0-b3fb-8d4c2331676a.png)

- Test açıklamasının ve test adımlarının yazılması. Test senaryolarının oluşturulması.

![Test senaryosunun oluşturulması](https://user-images.githubusercontent.com/42176018/164454604-3c9d5b74-49b7-480b-aa5e-88edd42de202.png)

- Test ön koşulunun yazılması.

![test ön  koşulu](https://user-images.githubusercontent.com/42176018/164455448-aeb75959-e9a4-48f5-a98d-d3e03128618b.png)

- Bir grup test senaryosunu içeren test setinin oluşturulması.

![test set](https://user-images.githubusercontent.com/42176018/164464330-0dd996a5-59b4-4ce2-9bbb-56316ea37c9d.png)

- 26 Nisan 2022 gününü hedefleyen yayın için test planı oluşturulması. Böylece insanlar sadece bu sürümü açacak, bir planı test edecek ve yapmak istedikleri testlerin ne olduğunu bilecekler. 26 Nisan'da yayınlanmasının önemli olduğu test senaryolarnı belirtme.

![testplan](https://user-images.githubusercontent.com/42176018/164472927-7f6a7ce7-2996-48ff-95cd-429ebdc0d982.png)

