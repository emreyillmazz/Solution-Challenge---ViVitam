<img src="https://user-images.githubusercontent.com/80172202/110236231-b5881f00-7f45-11eb-9a94-dc4cdef39f2f.png" height="200" width="200">

# Solution-Challenge-ViVitam 
### Smart Greenhouse Systems
Ülkemizde ve dünyada, artan nüfusun yeterince beslenebilmesi ve iyi bir gelir düzeyine ulaşabilmesi üretimin artırılmasına bağlıdır. Bu da sanayileşmeyle birlikte tarım sektöründeki gelişmelerle mümkündür. Günümüzde, toprak, hava, su kirliliği ve bunların giderek tükenmesi, tarımın da gerilemesine neden olmakta, buna bağlı olarak sağlıksız ve kalitesiz üretim artmaktadır. Ayrıca dünya pazarlarının besin maddelerine olan talebi üretimimizin de dış pazarlara yönelmesini zorunlu kılmaktadır. Bu yüzden tarımsal üretimin artırılması ve geliştirilmesi için birtakım önlemler alınması gerekir. Bu önlemlerden birisi de ülkemiz iklim koşullarında, kaliteli ve sürekli üretimi mümkün kıldığı için, besin ve enerji yönetiminin bir arada yapılabildiği sera işletmeciliğidir. Seralar, bitkisel üretimin endüstriyel olarak yapıldığı, gelişmiş işletmecilik kurallarının uygulandığı fabrikalardır. Modern sera tarım, biyosistem, makina,otomasyon, elektrik-elektronik ve bilgisayar mühendisliği gibi farklı disiplinlerdeki teknolojilerin bir arada kullanıldığı endüstriyel bir uygulamadır. 
### Projenin Çıkış Noktası
Tarım ve teknolojinin entegre olamaması sebebiyle tarımda üretim verimliliğinin yetersizliği projemizin çıkış noktasıdır. Seralarda yetişen ürünün sağlıklı olabilmesi optimum iklim koşullarının sağlanması ve korunması, iklim koşullarının sürekli izlenmesi ve gerektiğinde müdahale edilmesi ile sağlanmaktadır. Bu durum otomatik kontrol sistemleri sayesinde bitkinin üretim aşamasındaki kontrolü ile gerçekleştirilmektedir. Seraların verimliliğini arttırmak adına geliştirilen bu otomasyonda sıcaklık, nem, yağmur, ışık miktarı, karbondioksit miktarı, depo seviyesi gibi parametreler kontrol edilmektedir. Mükemmel bir otomasyon sistemi bu etkenleri iyi algılayabilmeli, değerlendirebilmeli ve doğru bir sonuç çıkarabilecek yapıya sahip olmalıdır. Araştırma sonuçlarına göre, 2016 yılında AB’de çalışan başına tarımsal üretimin Türkiye’deki üretimden 38 kat fazla olduğu görülmektedir. (Türkiye Tarım Kredi Kooperatifleri)
<p align="center">
<img src="https://user-images.githubusercontent.com/80172202/110217996-4b7d6480-7ec8-11eb-9034-a4568a9988a7.png" > </p>

### Çözüm
Projemizin başlangıç aşamasında, seraların bir cihaz veya bilgisayar yardımı ile uzaktan;

 >**Sıcaklık Kontrolü**
 
 >**Sulama Kontrolü**
 
 >**Havalandırma Kontrolü**
 
 >**Nem Kontrolü**
   
 >**Kamera ile Canlı Sera İzlemesi** yapılarak, zaman, enerji, iş gücü tasarrufu sağlamak ve üretim verimliliğini arttırmak hedeflenmektedir.


## ViVitam App
Akıllı serada bulunan sensörlerin Firebase bağlantısı yapılır. Sensörden okunan veriler Firebase’e aktarılır. Flutter üzerinden yazılacak masaüstü uygulaması Firebase üzerinden bu değerleri gösterir. Aynı zamanda uygulama arayüzü üzerinden değiştirilen değerler Firebase tarafından sensörlere iletilir. Böylelikle sera yönetimi anlık ve hızlı olarak gerçekleştirilebilir. 

- Masaüstü uygulaması ilk açıldığında bağlantı kurulmasını bekler. Birden çok serayı aynı anda denetleme özelliği bulunur. Demo versiyon olarak sadece sıcaklık kontrolü üzerine durulmuştur.

<p align="center">
 <img src="https://user-images.githubusercontent.com/80172202/110218756-75388a80-7ecc-11eb-8d8a-e3ffa182ac3b.png" height="360" width="460"> </p>

- Sera 1 (Sera adı daha sonra kişileştirilebilir) ile bağlantı gerçekleşir ve sensör verileri anında alınır. Multi-threading sayesinde tüm sera işlemleri birbirine beklemeden kendi içinde gerçekleşir
<p align="center">
<img src="https://user-images.githubusercontent.com/80172202/110218786-a1540b80-7ecc-11eb-922d-bbf28ba75750.png" height="360" width="460"> </p>

- Akıllı serayı kapatırsanız o an çalışan tüm ısıtıcılar sensörler kapatılır. Böylelikle sera hava sıcaklığına göre çalışır. Tekrardan sera açılabilir.
<p align="center">
<img src="https://user-images.githubusercontent.com/80172202/110218841-ea0bc480-7ecc-11eb-9e5b-11847b2043a7.png" height="360" width="460"> </p>

- Seranın sıcaklık değerini değiştirmek için mor ile gösterilen sıcaklık çevirici fare ile döndürülür. Sağ tarafında bulunan değer hedeflenen sıcaklıktır. Sera sıcaklığı bu hedeflenen sıcaklığa yakınsayacak şekilde çalışır.
<p align="center">
<img src="https://user-images.githubusercontent.com/80172202/110218986-a2d20380-7ecd-11eb-9e5c-b5463e18e438.png" height="360" width="460"> </p>

## Projenin Geleceği

##### Kısa Vadeli Hedefler:
- Mobil arayüzün eklenmesi
- Farklı sensörlerin seralara yerleştirilmesi ve uzaktan stabil kontrollerinin sağlanması

##### Uzun Vadeli Hedefler:
- Gelişmiş görüntü işleme sistemleri ile seralarda yetişen ekinlerin olgunluk seviyesi ve kalite durumu tespiti
<p align="center">
<img src="https://user-images.githubusercontent.com/80172202/110220114-a9b04480-7ed4-11eb-9d74-5ea1c27b4621.png"> </p>












