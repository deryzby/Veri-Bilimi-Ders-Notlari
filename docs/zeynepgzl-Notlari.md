***VERİ BİLİMİ NOTLARI***

## Veri Analizi : Elimizdeki veriyi anlamaya çalışılmasıdır.

## Veri Bilimi : Veri analizi ile örüntü bulmak yada eldeki veri ile elde olmayan veriyi tahmin etmek, bulmak.

## Yapa zeka, içinde belirli sayıları barındırır ve bir sonraki sayıyı tahmin eder. Hiçbir yapay zeka sistemi hiçbir şeye yüzde yüz sonuç vermez, hep tahminlerde bulunur.

## Back Propagation : Geriye yayılım. Hatayı ayıklayıp sebebini bulma.

## Learnin Rate : Hatanın ne kadar düzelteceğini belirler. 

## Aktivasyon Fonksiyonu : Yapay sinir ağlarında bir nöronun çıktısını belirleyen matematiksel fonksiyon. Aktivasyon fonksiyonları;
	
        1) Sigmoid : Sürekli gerçek sayıyı (0,1) aralığında dönüştüren matematiksel fonksiyondur. 
S(x)=1/(1+e^(-x) )

	2) tanh (Hyperbolic Tangent) : Giriş değerini (-1,1) aralığında sıkıştıran matematiksel fonksiyondur.
f(x)=(e^x-e^(-x))/(e^x+e^(-x) )

	3) Softmax : Tüm çıktıların toplamı 1 olan matematiksel fonksiyondur.
f(xi)=e^xi/(∑j^(e^xi ) )

	4) ReLU (Rectified Linear Unit) :   
Eğer x > 0 ise, çıktı x olur.
Eğer x ≤ 0 ise, çıktı 0 olur.
f(x)=max⁡(0,x)

## Mean Squared Error (MSE) : Yapılan hataların karesini alıp ortalamasını hesaplamadır.
MSE=(1/n) ∑_(i=1)^n▒(y_i -y_i')^2 
y_i : Gerçek değer
y_i'  : Modelin tahmin ettiği değer
n : Veri sayısı

## Hata Türleri :
	True Pozitif : Modelin doğru bir şekilde pozitif sınıfı tahmin etmesi.
	False Pozitif : Modelin yanlış bir şekilde pozitif sınıfı tahmin etmesi.
	True Negatif : Modelin doğru bir şekilde negatif sınıfı tahmin etmesi.
	False Negatif : Modelin yanlış bir şekilde negatif sınıfı tahmin etmesi.

## Lineer Regresyon : İki değişken arasındaki ilişkiyi incelemek için kullanılan istatistiksel yöntemdir.
y=ax+b
𝑌 : Tahmin edilen değer (bağımlı değişken).
𝑎 : 𝑌 eksenini kestiği nokta, yani 𝑋=0 olduğunda  𝑌 ’nin aldığı değer.
𝑏 : Doğrunun eğimi, yani 𝑋 ’teki bir birimlik değişikliğin  𝑌 ’yi ne kadar değiştirdiğini gösterir.
𝑋 : Bağımsız değişken.
  #BİR MAKİNE ÖĞRENMESİ MODELİ, MATEMATİKSEL FORMÜLDEN VE O FORMÜLDE Kİ PARAMETRELERDEN OLUŞUR.#

	* Logaritmik Artış : İlk başta hızlı bir artış olur, sonra yavaşlar ve bir limite yaklaşır.
y=log⁡(x)

	* Üssel Artış : Başlarda  yavaş başlar, sonra hızla artar.

y=a*b^x  ,( b>1)

	* Parabolik Artış : Başladığı oranla aynı şekilde azalır. Simetrik bir eğri oluşturur.
y=ax^2+bx+c

## Fine Tuning : İnce ayar, sayılarla çok oynamadan kendi durumumuza yaklaştırma.

## İstatistikte Veri Türleri:

	1) Kategorik Veri : Ölçülemeyen, üzerinden sayısal işlem yapılamayan nesnel veri tipidir.
  	* Nominal Veri: Sıralama veya karşılaştırma yapamayız. Örneğin, “Cinsiyet (Kadın, Erkek)”, “Göz rengi (Mavi, Kahverengi, Yeşil)”.
	  * Ordinal Veri: Kategoriler arasında bir sıralama vardır ama aralarındaki fark net değildir. Örneğin, “Eğitim seviyesi (İlkokul - Ortaokul - Lise)”.

	2) Numerik Veri : Ölçülebilen, üzerinde aritmetik işlemler yapılabilen veri tipidir.
	  * Kesikli Veri: Sayılabilir, tam sayı olan verilerdir. Örneğin, “Bir sınıftaki öğrenci sayısı (25 kişi)”.
	  * Sürekli Veri: Ölçümle elde edilir, kesirli ve ondalıklı olabilir. Örneğin, “Boy (166 cm)”, “Ağırlık (61 kg)”.

## Veri Maskeleme (Data Masking) : Gerçek verinin yerini alacak şekilde, belirli kısımlarını gizleme işlemidir. Maskeleme yapılan veri hâlâ bir şekil alır ama orijinal bilgiyi açığa çıkarmaz.

## Veri Anonimleştirme (Data Anonymization) : Veriyi değiştirip, gerçek kişiye veya kaynağa geri dönülmemesi işlemidir. Maskelemeden farklı olarak, anonimleştirilen veri geri getirilemez yani tamamen kimliksiz hâle gelir.

## Analog Veri : Sürekli değişen ve zamanla akıcı bir şekilde değişebilen verilerdir.
y(t)=Asin(2πft+θ)
A : Genlik (sesin yüksekliği),
𝑓 : Frekans (saniyedeki titreşim sayısı),
𝜭 : Faz açısı.

## Lojistik Regresyon : Bir istatistiksel sınıflandırma. Çıktısı (0,1) arasında bir olasılık değeri verir.  Sigmoid fonksiyonunu kullanarak tahmin yapar:
y=a_1 x_1+a_2 x_2+a_3 x_3+⋯+b

## Superviser Learning : Modelin eğitilmesi için etiketlenmiş veriler kullanılır. Veriye ait her bir örneğin doğru sonucu verilir ve model, doğru tahminler yapabilmek için bu etiketli verilerden öğrenir. Superviser Learning iki ana kategoriye ayrılır:
	1) Sınıflandırma (Classification) : Model, veriyi hangi sınıfa ait olduğunu tahmin eder. Çıktılar kategori (etiket) şeklindedir.
	2) Regresyon : Model, bir sayıyı tahmin eder. Çıktılar sürekli bir değer olur.

## K-Means Algoritması : Veri setindeki benzer nesneleri gruplamak için kullanılan popüler bir algoritmadır. Bu algoritma, veriyi K tane kümeye ayırarak, her bir veri noktasının en yakın kümeye ait olmasını sağlar.

## Regex (Regular Expressions) : Düzenli ifadeler, metin içindeki belirli desenleri tanımlamak ve bunlarla işlem yapmak için kullanılır.

## Caching (Önbellekleme) : Verilerin sıkça erişilen kısmını hızlı bir şekilde erişebilmek için geçici olarak saklama işlemidir. Yani, veriyi ilk kez aldığında, daha sonra tekrar ihtiyaç duyduğunda aynı işlemi tekrar yapmamak için veriyi saklar.

## Batch Processing (Toplu İşlem) : Büyük veri kümesi veya işlemleri küçük gruplar halinde işleme tekniğidir. Bu tür işlemler genellikle zamanlamalı olarak yapılır ve genellikle anlık (real-time) işleme gerek duymaz.

## Load Balancing (Yük Dengeleme) : Bir sistemdeki iş yükünün eşit bir şekilde dağıtılmasıdır. Load balancing, istekleri farklı sunuculara yönlendirerek sistemin yükünü dengelemeyi sağlar.

## Accuracy Metrics : Bir modelin ne kadar doğru tahminlerde bulunduğunu değerlendiren ölçütlerdir. Bu metrikler, sınıflandırma ve regresyon problemlerine göre değişiklik gösterir.
	
 1) Sınıflandırma Problemleri için Accuracy Metrics

	 * Doğruluk (Accuracy) : En yaygın kullanılan metriklerden biridir. Modelin doğru tahmin ettiği örneklerin, tüm örnek sayısına oranıdır.
Accuracy=Doğru Tahminler/Toplam Tahminler
	 * Kesinlik (Precision) : Modelin pozitif sınıf tahminleri arasında ne kadarının gerçekten doğru olduğunu gösterir. Özellikle yanlış pozitiflerin önemli olduğu durumlarda kullanılır.
Precision=Doğru Pozitifler (TP)/(Doğru Pozitifler (TP)+Yanlış Pozitifler (FP) )


	 * Hassasiyet (Recall) : Modelin gerçek pozitifleri bulma yeteneğini ölçer. Yanlış negatiflerin önemli olduğu durumlarda kullanılır. Örneğin, kanser teşhisi gibi kritik bir durumda, kaçırılan hastaların (yanlış negatiflerin) sayısının düşük olması istenir.
Recall=Doğru Pozitifler (TP)/(Doğru Pozitifler (TP)+Yanlış Negatifler (FN) )

	 * F1-Score : Kesinlik ve hassasiyet arasındaki dengeyi kuran bir metriktir. Özellikle, kesinlik ve hassasiyet arasında bir seçim yapmak zor olduğunda kullanılır. Bu metrik, iki ölçütü birleştirerek bir ortak denge sağlar.
F1=2*((Kesinlik*Hassasiyet)/((Kesinlik+Hassasiyet) ))

 
	 * ROC-AUC (Receiver Operating Characteristic - Area Under Curve) : Sınıflandırma modelinin sınıflandırma doğruluğunu daha kapsamlı bir şekilde değerlendiren bir metriktir. ROC, doğru pozitif oranı (TPR) ile yanlış pozitif oranı (FPR) arasındaki ilişkiyi gösteren bir grafiktir. AUC, bu eğrinin altında kalan alandır.
	 * Logaritmik Kayıp (Logarithmic Loss - Log Loss) : Modelin tahmin ettiği olasılıkların gerçek olasılıklardan ne kadar uzak olduğunu ölçen bir regresyon ve sınıflandırma metriğidir. Özellikle sınıflandırma problemlerinde ve derin öğrenme gibi modellerde yaygın olarak kullanılır. Log loss, doğruluğun yanı sıra modelin ne kadar güvenilir tahminler yaptığını da değerlendirir.
Log Loss=(-1/n) ∑_(i=1)^n▒〖(y_i  log⁡(p_i )+(1-y_i )log⁡(1-p_i)〗)
	 * Özgüllük (Specificity) : Negatif sınıf tahminlerinin doğruluğunu ölçen bir metriktir. Yani, modelin gerçekten negatif olan örnekleri negatif olarak tanımlama başarısıdır. Bu metrik, genellikle yanlış pozitiflerin (False Positives) azaltılmasında kritik rol oynar.
Specificity  =Doğru Negatifler (TN)/(Doğru Negatifler (TN)+Yanlış Pozitifler (FP) )

	2) Regresyon Problemleri İçin Accuracy Metrics
	 * Mean Absolute Error (MAE) : Tahmin edilen değerlerle gerçek değerler arasındaki mutlak farkların ortalamasıdır. Yani, modelin hata miktarını ölçer.
MAE=(1/n) ∑_(i=1)^n▒〖∣y_gerçek-y_tahmin∣〗
	 * Mean Squared Error (MSE) : Tahmin hatalarının karesinin ortalamasıdır. Bu metrik, büyük hataları daha fazla cezalandırır çünkü hata karesi büyüdükçe hata değeri artar.
MSE=(1/n) ∑_(i=1)^n▒(y_gerçek-y_tahmin )^2 
	 * Root Mean Squared Error (RMSE) : MSE’nin kareköküdür. Bu metrik, modelin hata büyüklüğünü doğal biriminde gösterir.
√((1/n) ∑_(i=1)^n▒() y_gerçek-y_tahmin)^2

>>Accuracy’nin Doğru Çalışmama Nedenleri:<<
	 * Dengesiz veri seti
	 * Hedef olmayan metrikler kullanılması
	 * Veri kalitesi veya hatalı veri hazırlama
 	 * Overfitting (Aşırı Uyum) veya Underfitting (Eksik Uyum)
	 * Yanlış model seçimi veya aşırı karmaşık modeller
	 * Özellik mühendisliği eksiklikleri

## Veri Seti : Verilerin düzenli bir şekilde toplandığı ve işlendiği bu yapılar, genellikle bir modelin öğrenme sürecini destekler veya analiz yapılabilmesi için temel sağlar.
	 1) Model Eğitimi ve Testi : Veri setleri, makine öğrenmesi ve yapay zeka modellerinin eğitim ve test süreçlerinde kullanılır. Modellerin doğru şekilde çalışabilmesi için, önce eğitilmesi gerekir. Bu süreçte kullanılan veri seti modelin öğrenme sürecinde ne kadar başarılı olduğunu belirler.
	 2) Veri Analizi ve Keşif : Veri setleri, çeşitli istatistiksel analizler yapmak, veri desenlerini keşfetmek ve veri hakkında derinlemesine bilgi edinmek için kullanılır. Bu analizler, model geliştirmeden önce verinin nasıl yapıda olduğunu anlamaya yardımcı olur.
	 3) Karar Destek Sistemleri : Veri setleri, iş süreçlerini iyileştirmek ve daha iyi kararlar almak için kullanılır. Verilerden elde edilen içgörüler, yöneticilere, karar alıcılara ve işletmelere stratejik kararlar konusunda rehberlik eder.
	 4) Otomatik Sistemlerin Eğitilmesi : Veri setleri, özellikle denetimli öğrenme yöntemleriyle otonom sistemler ve yapay zeka uygulamalarını eğitmek için kullanılır. Bu sistemler, insan müdahalesine gerek kalmadan bir problemi çözmek için eğitilebilir.
	 5) Anlamlı Tahminler Yapılması : Veri setleri, geçmiş verilerden elde edilen desenlere dayanarak gelecekteki olayları tahmin etmek için kullanılır. Bu, özellikle finans, sağlık, perakende ve lojistik gibi alanlarda önemlidir.
	 6) Modelin Performansını Değerlendirmek : Veri setleri, modelin doğruluğunu ve genelleme yeteneğini değerlendirmek için kritik öneme sahiptir. Test veri setleri kullanılarak modelin performansı ölçülür ve modelin ne kadar doğru tahminler yaptığına bakılır.
	 7) Hedefe Yönelik Veri Toplama : Veri setleri, belirli bir hedefe yönelik özel verilerin toplanması için kullanılır. Bu tür veri toplama, iş stratejileri, araştırmalar veya sosyal projeler gibi konularda kullanılabilir.
	 8) Eğitim ve Öğrenme : Veri setleri, özellikle öğrenme ve eğitim alanında önemli bir yere sahiptir. Eğitimciler, araştırmacılar ve öğrenciler, veri setleri kullanarak gerçek dünya problemleri üzerinde çalışabilir ve farklı veri bilim tekniklerini öğrenebilir.
	 9) Model Geliştirme : Veri setleri, model geliştirme sürecinin temel yapı taşlarıdır. Makine öğrenmesi ve derin öğrenme gibi alanlarda, modelin başarılı bir şekilde çalışabilmesi için çok sayıda etiketlenmiş veri gerekir. Bu veriler, modelin doğru sonuçlar verebilmesi için sürekli olarak test edilmeli ve geliştirilmelidir.

## Veri biliminde, benzerlik ölçümleri ve kümelenme algoritmaları gibi çeşitli makine öğrenmesi tekniklerinde kullanılan mesafe ölçütleri:
	 1) Minkowski Mesafesi : Genel bir mesafe ölçüsü olarak kabul edilir ve bir parametreye bağlı olarak Manhattan ve Öklid mesafelerine dönüşebilir.
	 2) Manhattan Mesafesi : İki nokta arasındaki dikey ve yatay mesafelerin toplamını ifade eder. Geometrik olarak, bu mesafe, bir şehirdeki bloklar arasında yürüyerek gidilen mesafeye benzer.
	 3) Öklid Mesafesi : İki veri noktası arasındaki doğrudan doğrusal mesafeyi ölçer. Bu, en yaygın kullanılan mesafe ölçüsüdür ve geometriyi temsil eder.

## Max Polling : Bir özellik haritasındaki her bölgeden en yüksek değeri seçerek, boyutları küçültür ve önemli özellikleri vurgular. Bu işlem, modelin daha verimli çalışmasını sağlar ve öğrenme sürecini hızlandırır. Görüntü işleme, sınıflandırma ve derin öğrenme uygulamalarında yaygın olarak kullanılır.

## Epoch Sayısı : Modelin eğitim verisi üzerinde kaç kez geçeceğini belirler. Yeterli epoch sayısı, modelin öğrenmesi için önemlidir, ancak fazla epoch sayısı overfitting'e yol açabilir. 
NOT : Makine öğrenmesinde modeli eğitirken Loss değeri belli bir değere düşünce eğitmeyi bırakmalıyız. Loss değeri belli bir noktaya düştüğünde, modelin aşırı öğrenme (overfitting) riski artar.

## Reinforcement Learning from Human Feedback (RLHF) : Modelin insan geri bildirimi kullanarak takviyeli öğrenme sürecini geliştirdiği bir tekniktir. İnsanlar, modelin eylemlerini değerlendirir ve geri bildirim verir. Böylece model daha hızlı, doğru ve güvenli bir şekilde öğrenir. Bu yöntem özellikle etik, güvenlik ve verimlilik konularında önemli avantajlar sağlar.

///////////////////////////////////////////////////////////////////////////////////

***HTML***

## HTML (HyperText Markup Language), web sayfalarını oluşturmak için kullanılan işaretleme dilidir. Web sitelerinin iskeletini oluşturur ve tarayıcıların sayfaları nasıl görüntüleyeceğini belirler. HTML bir programlama dili değildir, mantık ve koşullar içermez, sadece içeriği ve yapıyı belirler. 

## HTML Sayfası Temel Bölümleri :
	* <!DOCTYPE html> : HTML5 olduğunu belirtir.
	* <html> : Tüm HTML kodlarını kapsar.
	* <head> : Sayfanın başlık, stil ve meta bilgilerini içerir.
	* <title> : Tarayıcının sekmesinde görünen başlık.
	* <body> : Sayfanın görünen içeriği.

## HTML Temel Etiketleri :
	* <h1> - <h6> : Başlık etiketleri (h1 en büyük, h6 en küçük)
	* <p> : Paragraf oluşturur
	* <a href="URL"> : Link oluşturur
	* <img src="resim.jpg"> : Resim ekler
	* <ul> <li> : Sırasız liste oluşturur
	* <ol> <li> : Sıralı liste oluşturur
	* <table> : Tablo oluşturur
	* <form> : Form elemanlarını içerir
	* <div> : Blok elemanları gruplandırır
	* <span> : Inline (satır içi) metinleri gruplandırır

///////////////////////////////////////////////////////////////////////////////////

***PYTHON***

## Koşul Operatörleri (Comparison Operators) :.

 1) Karşılaştırma Operatörleri : Bu operatörler, iki değeri karşılaştırarak bir doğru (True) veya yanlış (False) sonucu döndürür. 
	  * Eşitlik (==): İki değerin eşit olup olmadığını kontrol eder.
	  * Eşit Değil (!=): İki değerin eşit olup olmadığını kontrol eder. Eğer eşit değilse True döner.
	  * Büyüktür (>): İlk değerin ikinciden büyük olup olmadığını kontrol eder.
	  * Büyük Eşittir (>=): İlk değerin ikinciden büyük veya eşit olup olmadığını kontrol eder.
	  * Küçüktür (<): İlk değerin ikinciden küçük olup olmadığını kontrol eder.
	  * Küçük Eşittir (<=): İlk değerin ikinciden küçük veya eşit olup olmadığını kontrol eder.
	
 2) Mantıksal Operatörler (Logical Operators) : Bu operatörler, birden fazla koşulun birleştirilmesi veya doğruluğunun belirlenmesi için kullanılır. Genellikle True veya False sonuçlarını döndüren daha karmaşık koşul ifadelerinde kullanılır.
	  * Ve (AND - and): Tüm koşulların doğru olması gerektiğini kontrol eder. Eğer bütün koşullar doğruysa, sonuç True olur.
	  * Veya (OR - or): Koşullardan en az birinin doğru olması yeterlidir. Eğer bir koşul doğruysa, sonuç True olur.
	  * Değil (NOT - not): Bir koşulun tersini alır. Eğer koşul True ise, False; False ise, True döner.
 
 3) Koşul İfadeleri (if - elif - else) : Belirli koşullara göre kodu çalıştırmak için kullanılır.

## Temel Veri Türleri (Data Types): Bu veri türleri, değişkenlerin içerebileceği farklı türde verileri ifade eder.
	  * int (İnteger) : Tam sayıları tutar
	  * float : Ondalıklı sayıları tutar.
	  * str (String) : Yazıları/metinleri saklar.
	  * bool (Boolean) : Doğru veya yanlış (True/False) değerini saklar.

## Değişkenler (Variables) : Verileri sakladığımız kutular gibidir. Harf, rakam ve “_” içerebilir. Rakamla başlayamaz. Büyük/küçük harf duyarlıdır.

## Döngüler (Loops) : Belirli kodları tekrar tekrar çalıştırmamızı sağlar.
	  * for Döngüsü : Bir koleksiyon veya liste üzerinde sırayla gezinir.
	  * while Döngüsü : Koşul True olduğu sürece çalışır.

## Listeler (Lists) : Birden fazla veriyi tek bir değişkende tutmak için kullanılır.

## String (Metin) İşlemleri : Python’da " " veya ' ' içinde yazılır.

## Fonksiyonlar (Functions) : Kod tekrarını önleyen ve kodu daha düzenli hale getiren yapılardır. def ile fonksiyon tanımlanır ve çağırılır.

## Hata Yönetimi (Try - Except) : Kod çalışırken hata alınırsa, programın çökmesini önlemek için try-except bloğunu kullanabilir.

## Kütüphaneleri İçe Aktarma :
	  * import pandas as pd : Pandas, veri analizi ve veri manipülasyonu için kullanılan güçlü bir kütüphane. csv dosyalarını okumak, verileri temizlemek ve işlemler yapmak için kullanılıyor. Pandas'ı pd olarak kullanmamızı sağlıyor.  pd.read_csv("file.csv") gibi.
	  * import numpy as np : NumPy, matematiksel hesaplamalar ve diziler (array'ler) üzerinde işlem yapmak için kullanılan bir kütüphane. Büyük veri kümeleriyle çalışırken oldukça hızlı ve etkili. NumPy'yi np olarak kısaltarak kullanmamızı sağlıyor.
	  * from fuzzywuzzy import process : FuzzyWuzzy, metinler arasındaki benzerlikleri hesaplayan bir kütüphane. Kullanıcı yanlış veya eksik yazsa bile en yakın film ismini bulabilmek için bunu kullanıyoruz. FuzzyWuzzy kütüphanesinden process modülünü içe aktarıyor. Bu modül, bir kelimeyi verilen bir listeyle karşılaştırıp en yakın eşleşenleri bulmaya yarıyor.
	  * import requests : Bu kütüphane, internete bağlanarak veri çekmemizi sağlar. API'ye istek göndermemizi sağlıyor. 
	  * from PIL import Image : PIL (Pillow), Python için bir görüntü işleme kütüphanesidir. API’den gelen görselleri alıp Streamlit üzerinde görüntüleyebilmemizi sağlıyor.
	  * import streamlit as st : Streamlit, veri bilimi ve makine öğrenmesi projelerini interaktif bir web uygulaması olarak göstermek için kullanılan bir kütüphane. st.title(), st.text_input(), st.image() gibi fonksiyonlarla bir arayüz oluşturmayı sağlıyor.
	  * from sklearn.feature_extraction.text import TfidfVectorizer : TF-IDF (Term Frequency-Inverse Document Frequency) metinler arasındaki benzerliği hesaplamak için kullanılıyor. Filmlerin özetlerini (overview) vektörleştirmek için kullanıyoruz. Filmlerin özetlerini sayısal verilere çeviriyor ki matematiksel olarak benzerlikleri hesaplayabilelim.
	  * sklearn (Scikit-Learn) : Makine öğrenmesi için kullanılan bir kütüphane.
	  * from sklearn.metrics.pairwise import sigmoid_kernel : Bu fonksiyon, iki metin arasındaki benzerliği hesaplamak için kullanılıyor. 

## Veri Setlerini Birleştirme ve Temizleme :
	  * merge() : Veri setlerini birleştirme.
	  * drop() : gereksiz sütunları veri setinden çıkarma.

## Streamlit Arayüzü :
	  * st.title() : Sayfanın başlığını ayarlıyoruz.
	  * st.sidebar.header() ve st.sidebar.text_input() : Kullanıcıdan başlığı almak için Streamlit'in sidebar kısmında bir metin kutusu oluşturuyoruz.

## Sayfa Tasarımı (Streamlit İle) :
	  * st.set_page_config : Sayfanın başlığını, simgesini ve genişliğini ayarlıyoruz.
	  * page_title="Zeynep Güzel" : Sekmede gözükecek başlık.
	  * page_icon="🌸" : Sayfanın küçük simgesi (favicon).
	  * layout="wide" : Sayfa geniş modda açılacak.

## Başlık ve Veri Kümesini Yükleme : 
	  * st.title("Zeynep Güzel") : Sayfaya büyük bir başlık ekler.
	  * @st.cache_data : Verileri bir kere yükleyip önbelleğe alır, böylece her seferinde CSV dosyasını yeniden okumaz, hız kazandırır.
	  * pd.read_csv("zeynep.csv") : zeynep.csv adlı dosyayı okur ve data değişkenine kaydeder.

## Kullanıcıdan Girdi Alma :
	  * st.number_input() : Kullanıcıdan sayısal giriş almak için kullanılır.
	  * pd.DataFrame() : Girilen değerleri bir DataFrame içine koyuyoruz, çünkü model tahmin yaparken DataFrame formatında veri bekler.

## Model Tahmini ve Sonuç Gösterme : 
	  * model.predict(input_df) : Kullanıcının girdiği değerlere göre tahmin yapar. 

## Sonuçları Gösterme ve Resim Ekleme :
	  * Image.open() : Modelin tahmin ettiği resmi yükler.
	  * st.image() : Resmi ekranda gösterir.


