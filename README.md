# Restful-API-ve-Backend-Gelistirme
Herkese merhabalar ben Emir, Back-end geliştiriciyim. Bu repo'da sizlere backend geliştirme hakkında bahsedeceğim ve backend'e ilgisi olup merak edenler için faydalı kaynak olacaktır. 

Konular;
1. Back-end (Arka Uç) Ve Front-end (Ön Uç) Nedir?
2. Back-end geliştirme dilleri & frameworkleri
3. Veritabanı Nedir?
4. Front-end'den Back-end'e nasıl isteklerimizi iletiriz? (API Nedir)
5. Node.js Nedir?
6. HTTP Methodları Nelerdir?
7. Restful API Nedir, Nasıl Yazılır, Express.js nedir?

## 1. Back-end Nedir?
Back-end ve türkçesiyle arka uç. Web siteleri örnek alarak gidecek olursak web sitelerimizin görünen kısmını HTML, CSS gibi işaretleme dilleri veya üst düzey işlerde React.js gibi Node.js çalışma ortamında çalışan kütüphaneler kullanırız. Bunlar front-end geliştirme araçlarıdır. Örneğin web siteme bir buton eklemek için bunu HTML elementi <button>Giriş Yap</button> şeklinde eklemem gerekir ve css yoluyla bu butonu kendi isteğime göre stillendirebilirim. Buna front-end denir. Ancak bir üye giriş sistemini düşünücek olursak üyeleri sakladığımız veritabanıyla iletişim kurmamız ve üyeyi kontrol ettirmemiz gerekir işte tam bu sırada sunucu tarafında çalışan bir programlama dili veya frameworküne ihtiyacımız vardır. Sunucu taraflı çalışan bir teknolojide veritabanı ile iletişim kurabiliriz.

## 2. Back-end geliştirme dilleri & frameworkleri
- Node.js (JavaScript)
- Django (Python)
- Flask (Python)
- PHP
- Spring Boot (Java)
ve daha fazla...

## 3. Veritabanı Nedir?
Örneğin web sitemizde bir üyelik sistemi olduğunu düşünelim ve üye giriş - kayıt gibi sistemler var. Üye giriş sisteminde üyenin girdiği bilgileri doğrulamam için üye kayıt olduğunda üye bilgilerini bir yerde saklamamız gerekir. Bunun için çeşitli ve herkesin isteğine göre olan veritabanları mevcut. İhtiyacınıza uygun olanı bulup kullanabilirsiniz
- MySQL
- MongoDB
- PostgreSQL
- SQLite
- Microsoft SQL Server
- Redux

## 4. Front-end'den Back-end'e nasıl isteklerimizi iletiriz? (API Nedir)
Bunun için API dediğimiz yani Application Programming Interface veya türkçesiyle Uygulama Geliştirme Arayüzü geliştiririz. API'yi şu şekilde görebiliriz. Restorana müşteri geldiğini düşünelim bu müşteri front-end olur, müşterinin isteğini almak için masaya gelen garson API olur, yemeği yapan aşçılar ise back-end olur. Bu şekilde herkesin anlayabileceği şekilde anlatabiliriz. API front-end'den back-end'e veri iletmek, veri sildirmek, veri almak gibi bir çok sebep ile kullanılabilir.

## 5. Node.js Nedir?
Node.js günümüzde çokça kullanılan, JavaScript programlama dilinde geliştirilen, sunucu tarafında çalışan bir çalışma ortamıdır. Node.js'i cihazımıza kurduğumuzda yanında npm (node package manager = node paket yöneticisi) yazılımı ile beraber gelir. npm sayesinde uzun kod yazmaktan kurtuluruz ve istediğimiz kütüphaneleri node.js çalışma ortamımıza yükleyebiliriz. Örneğin MySQL veritabanına bağlanmak istiyorsak **"mysql2"** gibi bir kütüphane kullanabiliriz. Bu kütüphane başkaları tarafından geliştirilmiş ve MySQL işlemleri yaptırmamız için uzun koddan bizi kurtaran bir kütüphanedir.

## 6. HTTP Methodları Nelerdir?

**__1-) GET:__** Bu metod sunucudan veri almak için kullanılır. GET ve POST metodları en sık kullanılan metodlar olup sunucudaki kaynaklara erişmek için kullanılırlar.
**2-)POST:** Bu metod ile sunucuya veri yazdırabilirsiniz. Bu metodla istek parametreleri hem URL içinde hem de mesaj gövdesinde gönderilebilir. Sadece mesaj gövdesinin kullanımı yukarıda sayılan riskleri engelleyecektir. Tarayıcılar geri butonuna basıldığında POST isteğinin mesaj gövdesinde yer alan parametreleri tekrar göndermek isteyip istemedimizi sorarlar. Bunun temel nedeni bir işlemi yanlışlıkla birden fazla yapmayı engellemektir. Bu özellik ve de güvenlik gerekçeleriyle bir işlem gerçekleştirileceğinde POST metodunun kullanılması önerilir.
**3-)PUT:** Bu metod ile servis sağlayıcı üzerindeki bir kaynağı güncelleyebilirsiniz. Hangi kaynağı güncelleyecekseniz o kaynağın id’sini göndermek zorunludur.
**4-)HEAD:** GET metoduyla benzer işleve sahiptir ancak geri dönen yanıtta mesaj gövdesi bulunmaz (yani başlıklar ve içerikleri GET metoduyla aynıdır). Bu nedenle GET mesajı gönderilmeden önce bir kaynağın var olup olmadığını kontrol etmek için kullanılabilir.
**5-)DELETE:** Bu metod ile sunucudaki herhangi bir veriyi silebilirsiniz.
**6-)CONNECT:** Bir proxy sunucu üzerinden başka bir sunucuya bağlanmak ve proxy sunucuyu bir tünel gibi kullanmak için kullanılır.
**7-)OPTIONS:** Bu metod belli bir kaynak için kullanılabilecek HTTP metodlarını sunucudan sorgulamak için kullanılır.
**8-)TRACE:** Teşhis amaçlı kullanılan bir metoddur. Sunucu bu metodla gelen istek mesajının içeriğini aynen yanıt gövdesinde geri göndermelidir. Bu yöntemle sunucu ile istemci arasında bir vekil sunucu varsa bu sunucunun ve yaptığı değişikliklerin tespiti mümkün olabilir.
**9-)PATCH:** Bu metod bir kaynağa istediğiniz küçük çaplı değişimi yapmanızı sağlar.
**10-)SEARCH:** Bir dizinin altındaki kaynakları sorgulamak için kullanılır.
