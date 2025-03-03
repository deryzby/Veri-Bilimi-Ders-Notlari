# VERİ BİLİMİ DERS NOTLARI

07/10/2024

Yapay zeka: soruyu tamamlamak ve bir sonraki parçayı tamamlamak, tahmin etmekle görevlidir.

Nasılsın? (soruluyor). daha sonra ne sorulabilir?

belirli sayılarla belirli işlemeler yaparken başka sayılar bulan sistemdir. ChatGPT bu öürntü ile çalışıyor. Örüntü yoksa bu şey yapay zeka olamaz.

Gelecek analiz edilmez tahmin edilir.

Analiz: Ayırmak, parçalamak. Detay. Tüm yönleri ile görebilmektir.

Sentez: Birleştirmek.

Veri Analizi: Elimizdeki olayın detayını anlamaya çalışıyoruz.

örnek: %30’luk geçme oranı ile bitmiş. Örüntüyü anladıktan sonra kat sayıları buluyoruz. Dışardan veri setinde olmayan bir öğrenci eklendiğinde eldeki veriye bakıp elde olmayan bilgiyi Ön Görmeye VERİ BİLİMİ denir.

Veri Bilimi henüz olmayan bir olayı tahmin etmektir.

Geriye yayılım back propagation. Hatayı alıp kim ne kadar hatalı ona bakıyoruz. learning rate ne kadar düzenlenebilir.

10/10/2024

Sider Fusion: sürekli bir gerçek sayıyı dönüştüren matematik fonksiyonudur.

yapay sinir ağlarından karmaşık problemleri öğrenmek için yaygın olarak kullanılır.

Euler's Number (2.718281828459045)sayıları düzene sokmaya çalışıyor.

Softmax 4 sayının toplamı 1 olmalı.

DERİN öğrenme

Sigmoid

tahn

relu ve türevleri

Loss fonksiyonları

MSE (mean squared error)

Gerçek değerlerden tahmin ettiğimiz değerleri çıkartmak.

Yönlü Hata

5 saatte gidecekken 7

5 saatte gidecekken 3 saatte gidiyorsa +2. -2 toplam hata sıfırdır.

Doğrusal (Lİneer) regresyon

y= ax+b

a: eğim

b: bayes

veriye bakıp en yakınsak ölçüyü bulmak

b olmazsa doğru sıfırdan geçer.

14/10/2024

Doğrusal (Lİneer) regresyon

sayıya karşılık sayı gelir.

İki boyutlu bir uzaydır.

Numerik ve kategorik veri türleri lineer regresyonda kullanılır.

Lineer regresyonda veriler sonsuza gidebilmeli eğer veriler sonsuza gitmezse logaritmik regresyondur.

17/10/2024

## List (koleksiyonlar)/array/dizi:

alınacaklar= [“elma”,”armut”,”muz”]

küme(set): {elma,armut,muz} tekrar etmez hepsi birer kere kullanılır. Elemanların sırası olmaz. Elemanlar hep aynı sırada olmak zorunda değildir.

Sözlükler : alınacaklar_sözlüğü {elma:3, armut:3,elma:1} Elmanın son değeri ne ise odur.

# DÖNGÜLER

değişkeni tanımlamadan önce tipim-ni belirlememiz gerekiyor.

< karşılaştırma operatörü

Not: Matematiksel formül ve sayılar yapay zekayı ifade eder.

21/10/2024

Matematiksel formül ve sayılar yapay zeka modelini oluşturur.

a ve b yi vermelidir.

y=a+bx (lineer reg.)

ilk eğitimde rastgele veriler atanır.

Fine tuning yeni verilere göre modeli tekrar eğitmektir. Sayılarla çok oynamadan kendi durumumuza yaklaşmaktır.

Lojistik regresyon modeli

İki veri faktörü arasındaki ilişkileri bulmak için matematikten yararlanan bir veri analizi tekniğidir.

Veri Koleksiyonu: Birden çok veri setini bir arada tutmaktır. Kütüphane, list, set vb.

## İlkel Veri Tipleri:

boolen, string, float, stringer

Koşul Operatörleri

== eşitlik operatörü eşit midir i sorgular

if i %2  == aritmetik operatör (mod bölündüğünde kalan sayı)

!= eşit değildir operatörü

tüm koşul operatörlerinin sonucu true false olur Boolendir.

if bir durum kontroldür.

Emin olmadığımız durumları sorma durum kontrolüdür.

24/10/2024

Makine öğrenmesi/ Problem çeşitleri

regresyon problemi

Geçmiş dataya bakıp tarihsel süreçlerle ilgili tahminde bulunmak (numara tahmini)

Cevap numeriktir.

sınıflandırma problemi

Sınıflama verileridir. cevap numerik değil kategoriktir.

Müşteri kredi almaya uyumlu mu?, Hasta ya da değil, Nüfus artıyor artmıyor,dil modelleri vb.

Supervised learning denetimli öğrenmedir. Bizim yaptığımız da budur.

modeli eğitmel istediğimiz datada öğrenmek istediğimiz bilgiler vardır.

kümeleme problemi

birliktelik kurallı öğrenmedir.

Her zaman öğrenmek istediğimiz bilgiye sahip olmayabilir.

Unsupervised learning denetimsiz öğrenmedir.

K-means Algoritması

Çevremizdeki kişilerin ortalaması şeklinde düşünülebilir.

Veri random şekilde belli sayıda gruba ayrılır. Gruplandırma yapıldıktan sonra veri yorumlanır.

Kümedeki eleman sayısı aynı olmak zorunda değildir. Ancak sınıflandırmada aynı olmak zorundadır.

Kümelerin modeli ve merkezi verilirse model eğitilmiştir, kullanılabilir.

Formüller internetten bulunabilir ancak merkezler veriden elde edildiği için bizim vermemiz gerekir.

04/11/2024

Veri Çekme

http en yaygın protokoldür.

talep ettikçe veri gelir.

get metotu tüm sayfaları veriyor

post istediğimizi veriyor.

07/11/2024

Veri bilimi hangisini öğreneyim ne gerekli, nasıl öğreneyim.

11/11/2024

Data türü

random

yanlış

elimizde data olmamasından daha kötüdür.

sentetik

gerçek hayata benzer örnekler üretmektir.

gerçek

insan tarafından üretilen datadır. en kalitelisidir.

# K-NN

en yakın 5 komşunuzdan ibaretsinizdir.

verilen özelliklerden hagi 5’i sana benziyorsa seni de bulabiliriz.

Makine öğrenmesi yoktur. Formül+ parametre olmalı.

14/11/2024

Learning rate 100 de 1 kendini düzeltiyor( makine öğrenmesinde).

support vector machine (svm)

dağınık veriler verilir. Datayı en iyi ayıran doğruları bulup aradakini gösterir..

wx-b (formül)

overfitting dataya çizgiyi o kadar güzel yerleştiriki datayı en iyi şekilde temsil eder.

underfitting datayı tam temsil edemez.

not: Bir yapay zeka modelinde büyük verilerde  %100 çözüm veriyorsa terslik olabilir.

18/11/2024

Yapay Sinir Ağları (ANN)

bir şeye ne kadar çok açıdan bakarsanız o kadar bilgi olur ve iyi anlayıp yorumlayabiliriz.

veri tüm boyutlardan görülmeli

ancak büyük verilerde: teorik imkansızlık, işlem maliyeti ve zaman gibi sorunlar olabilir

Birden fazla fonksiyon yazılır.

yazılan çoklu lineer fonksiyonlar iç içe şekilde ve birbirine bağlıdır.

her bir fonksiyona nöron denir

bir sinir hücresi aktive olabilmesi için belirli aralıkta değer almalıdır. Buna aktivasyon fonksiyonu denir.

aktivasyon fonksiyonu fonksiyonların girdi ve çıktısını düzenliyor.

21/11/2024

Hiyerarşik kümeleme

her noktanın birbirine olan uzaklığı hesaplanır

25/11/2024

matrix kullanımın temel nedeni işlem paralelleştirmedir. Aynı işlemi daha da hızlandırıp güzelleştiriyoruz.

çalıştığımız problemle ilgili giriş katmanına biz karar vermiyoruz.

çıkış katmanında kaç tane nöron olduğuna da biz karar vermiyoruz.

katman eklerken bir amaç olmalı. Her bir katman bir önceki katmanı değerlendiriyor.

türev alma

f(x)=x2

sigmoid fonksiyonu

28/11/2024

back propagation

Rastgele oluşturulan bu katsayıları, eldeki problemin çözümüne uygun hale getiren ve değişmesini sağlayan metota da backpropagation adı verilir.

tensorflow, , pytorch yazdığımız kodları çalıştırıyor.

pyhton asıl çalışan dil değil,dili yönetmemizi istiyor.

modeli çalıştırdıktan sonra kaydetmemiz gerekiyor.

çünkü her seferinde eğitip soru sormak zor.

Modeli kaydetmek formül ve parametreleri yüklemek demektir.

05/12/2024

Streamlit, gardio

son kullanıcıya direkt olarak ulaşabilmektir.


