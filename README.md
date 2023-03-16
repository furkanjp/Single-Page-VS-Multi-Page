<h1>Single Page Application Ve Multi-Page Application Nedir?</h1>


<h2>Multi-Page Application (MPA) Nedir?</h2>

Çok Sayfalı Uygulama, üzerlerindeki veriler her değiştiğinde tamamen yenilenen çok sayıda sayfadan oluşan bir web uygulamasıdır. Sunucuya herhangi bir veri değişikliği veya veri aktarımı, tarayıcıda görüntülenen yeni bir sayfaya yol açar.


<h3>MPA Nasıl Çalışır?</h3>

Mpa yani klasik web siteleri , istemci (client), sunucudan (server) ulaşmak istediği sayfayı talep eder, sunucu da bu sayfayı istemci ile paylaşır. Bu işlem her sayfa için tekrar tekrar gerçekleştirilir. Mesela bir siteye girdiğinizde önce ana sayfa sunucudan istenir, sonra kullanıcı diğer bir sayfaya geçtiğinde, mesela iletişim sayfası diyelim, istemci tekrar bu sayfayı sunucudan ister. Klasik web siteleri bu şekilde çalışmaktadır.

![mps](https://user-images.githubusercontent.com/68124208/225749711-c9720803-795a-4b98-b53c-bbe3d99faa8b.jpg)

<h3>MPA'ların Dezavantajları Nelerdir?</h3>
<h5>Uzun Yükleme Süreleri </h5>
Her sayfa yükleme ve yeniden yükleme için sunucuya sürekli istek gönderdiği için, artan kullanıcı talepleri, yükleme hızını ve gezinmeyi yavaşlatır.
<h5>Farklı Platformlara Taşınabilirliği</h5>
Mobil uygulama geliştirme çok daha fazla zaman alacaktır. Çoğu durumda, sıfırdan Backend kısmı yazmanız gerekir.
<h5>Bakım ve güncellemeler</h5>
Çok sayfalı web sitelerine teknik destek sağlamak zor olabilir. Bu konu güvenlik konuları için de geçerlidir.
<h3>MPA'ların Avantajları Nelerdir?</h3>
<h5>SEO Optimizasyon Kolaylığı</h5>
Uygulamanın birden fazla sayfası vardır ve bunların her biri, Google'dan ücretsiz organik trafik almak için belirli bir istek grubu için optimize edilebilir.
<h5>Ölçekleme Kolaylığı</h5>
Bu mimari türü, her ürün veya hizmet için istediğiniz kadar yeni sayfa oluşturmanıza ve bunlarda herhangi bir değişiklik yapmanıza olanak tanır.
<hr/>
<h2>Single Page Application (SPA) Nedir?</h2>

Single Page Application, sunucudan yeni sayfaların tamamını yüklemek yerine geçerli sayfayı dinamik olarak yeniden yazarak kullanıcıyla etkileşime giren bir web uygulaması veya web sitesidir.
<h3>Single Page Application Nasıl Çalışır?</h3>
Klasik web sayflarının aksine istemci sunucuya sadece uygulama ilk açıldığı anda bir kere gider ve ne var ne yok bütün site içeriğini alır.Kullanıcın istediği kısımlar dinamik olarak yenilir.

![spa](https://user-images.githubusercontent.com/68124208/225750899-0a9ac75b-e988-4816-8188-97645a75a527.jpg)
<h3>Single Page Application Avantajları nelerdir?</h3>
<h5>Hız</h5>
Single page web uygulamalarında bütün sayfa sürekli yenilenmez, bu sayede büyük bir hız farkı görülür. Çoğu kaynak(html/css/js) birkez sunucudan gelir ve değişen şey veri olur. Sayfa yüklenme hızı bu sayede çok hızlı olur.
<h5>Kullanıcı deneyimi</h5>
SPA kullanımı size çok daha iyi bir kullanıcı deneyimi yaşatır. Sayfalar arası geçişi çok daha kolaylıkla yapabilir, sayfaların ortak kullandığı alanlar sürekli değişmediğinden ihtiyacınız olanı daha kolay ve hızlı bulursunuz.
<h5>Caching(Önbellek)</h5>
Single page uygulamalar local veriyi çok daha etkili şekilde kullanabilir. Bir kez sunucuya istek attıktan sonra gelen veriyi kullanıcının interneti yavaş olsa ya da gitse bile kullanabilir. İnternet bağlantınız geldiğinde websitesi sunucu ile tekrar senkronize olur.
<h5>Debugging</h5>
SPA ile debugging işlemi çok daha kolaylaşır. Chrome gibi modern tarayıcıların toolları sayesinde network monitoring, elementlerin takibi, verinin takibi gibi işlemleri daha kolay yaparsınız. Chrome üzerinde AngularJS, React, VueJS gibi frameworklerin gelişmiş toolları ile geliştirme hızınızı arttırabilirsiniz.

<h3>Single Page Application Dezavantajları Nelerdir?</h3>
<h5>SEO</h5>
SPA, arama motoru optimizasyonunda biraz zayıf kalıyor. URL eski dinamik sayfalardaki gibi tam anlamıyla değişmiyor, routing işlemi JavaScript tarafından yapılıyor. Bu yüzden arama motorları için aslında tek bir sayfa gibi gözüküyor. Google bu sorunu çözmek için çeşitli değişiklikler yaptığını duyurdu. Frameworklerde kendi içlerinde bu sorunları aşmak için çözümler geliştiriyorlar.
<h5>Tarayıcı Geçmişi</h5>
Web tarayıcınızda geri butonuna bastığınızda web uygulamanız içinde bir önceki duruma gidemezsiniz. Sizi bir önceki sayfaya yönlendirir. Uygulamamız “single page” olduğu için de bir önceki siteye gidersiniz.
<h5>Güvenlik</h5>
Uygulamanın sunucu tarafından istemci tarafına daha çok yük bindirmesi beraberinde güvenlik problemlerini de getiriyor. İstemci tarafında XSS kullanarak istemci taraflı scriptleri çalıştırmak kolaylaşıyor. Aynı şekilde kullanıcının izni olmadan belli yetkileri almakta kolaylaşıyor. Ancak React, Angular gibi popüler frameworkleri geliştiren firmalarda bu durumun farkında olacaktır ki geliştirdikleri frameworkleri bu yönde güncelliyorlar. Uygulamanın güvenliğinde geliştiricinin yani sizin de öneminiz artıyor.
<h5>Memory leaks(bellek sızıntısı)</h5>

Single Page Application için önemli sorunlardan birisi de memory leaks. Uygulamanızda çok fazla obje sürekli yüklenir ve sayfadan gider. Ancak siz gitti olarak görsenizde doğru şekilde geliştirmediyseniz aslında bellekten silinmemiş olabilir. Bu sebeple çöp nesnelerin aldığı bellek alanı işletim sistemine geri verilememiş olur. Bu da belleğin şişmesini sağlar. Bu durum da kullanıcı arayüzünün yavaşlamasına ve batarya kullanımının artmasına sebebiyet verebilir. Özellikle mobil kullanıcılar için problem olabilir.

