<h1># Alışveriş Sitesi Projesi</h1>

Bu proje, bir alışveriş sitesinin React formatına dönüştürülmesi ve çeşitli özelliklerin eklenmesi amacını taşımaktadır. Aşağıda projeyle ilgili detaylı bilgilere ulaşabilirsiniz.

<h1>## Hedefler</h1>

<h3>1. HTML Tasarımını React Formatına Dönüştürme:</h3>

- Verilen HTML tasarımını React bileşenleri ve JSX kullanarak dönüştürme işlemi gerçekleştirilecektir.</br>
- Tasarımın yapısı, bileşenlerin hiyerarşisi ve stillemesi React standartlarına uygun olacak şekilde düzenlenecektir.</br>

<h3>2. API'den Verileri Çekme:</h3>

- Gerekli olan verileri almak için bir API entegrasyonu yapılacaktır.</br>
- API, alışveriş sitesi için ürünler, kategoriler, sayfalar, kullanıcı bilgileri vb. gibi verileri sağlayacaktır.</br>
- Axios veya fetch gibi uygun bir kütüphane kullanılarak API istekleri gerçekleştirilecektir.</br>

<h3>3. Login ve Register Ekranları:</h3>
   - Kullanıcıların sisteme giriş yapabilmesi ve yeni hesap oluşturabilmesi için Login ve Register ekranları tasarlanacaktır.</br>
   - Kullanıcılar, formları doldurarak giriş yapabilecek veya yeni hesap oluşturabilecektir.</br>
   - Giriş ve kayıt işlemleri için API'ye gerekli veriler gönderilecek ve gelen yanıtlara göre işlem sonuçları alınacaktır.</br>
   - Kullanıcı bilgileri, giriş yaptıktan sonra tutulacak ve ilgili sayfalarda kullanılacaktır.</br>

<h2>Login Sayfasının Tasarımı:</h2>

HTML ve CSS kullanarak bir login formu oluşturulmuştur.</br>
E-posta adresi ve şifre gibi gerekli giriş alanları bulunmaktadır.</br>
Form göndermek için bir submit düğmesi de mevcuttur.</br>

<h3>onSubmit İşlevi:</h3>

Login sayfasındaki form, onSubmit olayı ile bir işlevle ilişkilendirilmiştir.</br>
Bu işlev, form gönderildiğinde çağrılacak olan asenkron bir işlevdir.</br>
İşlevin içinde, form verileri alınır ve bir JSON nesnesine dönüştürülür.</br>
Daha sonra, api.post fonksiyonu kullanılarak bu JSON verisi API'ye gönderilir.</br>
API'den gelen yanıt, authResponse değişkenine atanır ve konsola yazdırılır.</br>

<h3>API İstekleri:</h3>

API istekleri yapmak için bir api değişkeni kullanılmaktadır. Bu değişken, useApi kancasından elde edilen bir axios instance'ıdır.</br>
api.post fonksiyonu, bir POST isteği yapmak için kullanılır.</br>
İlk parametre olarak isteğin yapılacağı URL ("admin/authentication-token") verilir.</br>
İkinci parametre olarak form verilerini içeren bir JSON nesnesi (formJson) verilir.</br>
api.post fonksiyonu, isteğin tamamlanmasını bekler ve sonucu authResponse değişkenine atar.</br>

<h3>Sonuçları İşleme:</h3>

API isteği tamamlandıktan sonra, authResponse değişkeninde yanıt bilgileri bulunur.</br>
Bu yanıt, başarılı giriş durumunda bir kullanıcı kimlik bilgisi veya hata mesajları içerebilir.</br>
Login sayfasında, gelen yanıta göre işlem sonuçları uygun şekilde işlenir. Örneğin, başarılı giriş durumunda kullanıcı yönlendirilir veya hata mesajı görüntülenir.</br>
Register sayfası için de benzer bir işleyiş geçerlidir. Kullanıcılar register sayfasında gerekli bilgileri doldurduktan sonra form gönderildiğinde, API'ye bir POST isteği yapılır ve kullanıcı bilgileri kaydedilir.</br>

<h3>4. Kategori ve Ürünleri API'den Çekme:</h3>
   - Alışveriş sitesindeki kategoriler ve ürünler API'den çekilerek sayfalarda görüntülenecektir.</br>
   - Kategoriler, menülerde veya filtreleme seçeneklerinde kullanılabilecektir.</br>
   - Ürünler, ilgili kategorilere göre gruplandırılarak listelenecektir.</br>
   - Ürün detaylarına ve ilgili sayfalara yönlendirmeler yapılacaktır.</br>

<h1>## Kurulum</h1>

1. Projeyi klonlayın: `git clone https://github.com/kullanici/alisveris-sitesi.git`</br>
2. Proje dizinine gidin: `cd alisveris-sitesi`</br>
3. Gerekli bağımlılıkları yükleyin: `npm install` veya `yarn install`</br>
4. Projeyi başlatın: `npm start` veya `yarn start`</br>
5. Tarayıcınızda proje adresini açın: `http://localhost:3000`</br>

<h1>## Kullanım</h1>

- Ana sayfada alışveriş sitesinin React formatına dönüştürülmüş hali görüntülenecektir.</br>
- Kategoriler, ürünler, sayfalar vb. veriler API'den çekilerek dinamik olarak görüntülenecektir.</br>
- Login ve Register ekranlarına erişmek için ilgili bağlantılara tıklayabilirsiniz.</br>
- Ürün detaylarına ve il

<a href="https://ecommerce-bootcamp.netlify.app/">Canlı Önizleme</a>
<img src="./public/assets/images/screen.gif" alt="">
