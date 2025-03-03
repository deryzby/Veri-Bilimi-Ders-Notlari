# Veri Bilimi Eğitimi Notları

## 1. Ders: Yapay Zeka ve Veri Bilimi (07.10.2024)

### Yapay Zeka ve Veri Bilimi Kavramları
- **Yapay Zeka (AI):** İnsan gibi düşünebilen ve hareket edebilen makineler yaratmayı hedefleyen bir alan.
- **Veri Bilimi:** Verilerden anlamlı bilgiler çıkarmak için kullanılan disiplinler arası bir alan.
- **Makine Öğrenmesi (ML):** Bilgisayarların açıkça programlanmadan verilerden öğrenmesini sağlayan bir yapay zeka alt kümesi.
- **Derin Öğrenme (Deep Learning):** Çok katmanlı yapay sinir ağlarını kullanarak verilerden karmaşık örüntüler çıkaran bir makine öğrenmesi alt kümesi.

### Yapay Zeka Modelleri
- **Parametreler:** Yapay zeka modellerinin davranışını kontrol eden ayarlar.
- **Eğitim:** Veriler kullanılarak modelin parametrelerinin ayarlanması süreci.
- **Amaç:** İnsan zekasına benzer şekilde verileri analiz edebilen, tahminlerde bulunabilen ve kararlar alabilen modeller geliştirmek.

### Aktivasyon Fonksiyonları
- **ReLU (Rectified Linear Unit):** Negatif değerleri sıfırlayan, pozitif değerleri olduğu gibi bırakan bir aktivasyon fonksiyonu.
- **Sigmoid:** Çıktıyı 0 ile 1 arasında bir değere sıkıştıran bir aktivasyon fonksiyonu.
- **Softmax:** Çok sınıflı sınıflandırma problemlerinde çıktıları olasılıklara dönüştüren bir aktivasyon fonksiyonu.

### Veri Analizi
- **Örüntü Bulma:** Verilerdeki gizli örüntüleri ve ilişkileri keşfetme.
- **Anlama:** Verilerin ne anlama geldiğini ve nasıl yorumlanacağını anlama.
- **Tahmin:** Geçmiş verilere dayanarak gelecekteki olayları veya değerleri tahmin etme.

### Araçlar ve Kaynaklar
- **Jupyter Notebook:** Veri analizi ve makine öğrenmesi için popüler bir etkileşimli ortam.
- **VS Code:** Kod yazmak ve hata ayıklamak için güçlü bir kod düzenleyici.
- **Geriye Yayılım (Backpropagation):** Yapay sinir ağlarında hataları geriye doğru yayarak ağırlıkları güncelleme algoritması.
- **Learning Rate:** Modelin öğrenme hızını kontrol eden bir parametre.
- **GitHub:** Kod paylaşımı ve versiyon kontrolü için bir platform.
- **Hugging Face:** Doğal dil işleme modelleri için bir platform.
- **Kaggle:** Veri bilimi yarışmaları ve veri setleri için bir platform.

---

## 2. Ders: Aktivasyon Fonksiyonları ve Hata Fonksiyonları

### Aktivasyon Fonksiyonları
- **ReLU (Rectified Linear Unit):**
  - Girdi değeri 0'dan küçükse 0, 0'dan büyükse girdi değerinin kendisini döndüren bir aktivasyon fonksiyonudur.
  - Yapay sinir ağlarında yaygın olarak kullanılır ve doğrusal olmayanlığı modele dahil etmeye yardımcı olur.
- **Sigmoid:**
  - Girdi değerini 0 ile 1 arasında bir değere dönüştüren bir aktivasyon fonksiyonudur.
  - Formülü: \( S(x) = \frac{1}{1 + e^{-x}} \)
  - Genellikle ikili sınıflandırma problemlerinde kullanılır.

### Hata Fonksiyonları (Loss Functions)
- **Mean Squared Error (MSE):**
  - Modelin tahminleri ile gerçek değerler arasındaki farkın karesinin ortalamasını hesaplayan bir hata fonksiyonudur.
  - Regresyon problemlerinde yaygın olarak kullanılır.
- **Hata Ölçümleme:**
  - Modelin performansını değerlendirmek için kullanılır.
  - Doğru ve yanlış tahminlerin sayısını ölçer (True Positive, False Positive, True Negative, False Negative).
- **Yönlü Hata:**
  - Tahminlerin gerçek değerlerden ne kadar saptığını yönlü olarak (pozitif veya negatif) ölçer.
- **Loss Fonksiyonlarının Amacı:**
  - Modelin hatalarını en aza indirgemek için kullanılır.
  - Modelin eğitimi sırasında, loss fonksiyonunun değeri azaltılmaya çalışılır.

---

## 3. Ders: Veri Tipleri ve Yapıları

### Veri Tipleri
- **Tuple (Demet):** Sıralı ve değiştirilemez veri koleksiyonudur. Örneğin, `(elma, armut, muz)`.
- **Set (Küme):** Sırasız ve tekrarlayan elemanları içermeyen veri koleksiyonudur. Örneğin, `{elma, armut, muz}`.
- **Dictionary (Sözlük):** Anahtar-değer çiftlerinden oluşan veri koleksiyonudur. Örneğin, `{"isim": "Hatice", "yas": 30}`.

### Döngüler ve Koşullar
- **For Döngüsü:** Belirli bir sayıda tekrarlamak için kullanılır. Örneğin, `for i in range(1000): print("Beni Affet!")`.
- **While Döngüsü:** Belirli bir koşul doğru olduğu sürece tekrarlamak için kullanılır. Örneğin, `while i < 1000: print("Beni Affet!")`.
- **Koşullar (if-else):** Bir koşul doğruysa bir kod bloğunu, yanlışsa başka bir kod bloğunu çalıştırır.

---

## 4. Ders: Makine Öğrenmesi Problemleri ve Türleri

### Makine Öğrenmesi Problemleri
- **Regresyon:** Geçmiş verilere dayanarak gelecekteki değerleri tahmin etmeyi amaçlayan bir makine öğrenmesi problemi.
- **Sınıflandırma:** Verileri belirli kategorilere veya sınıflara ayırmayı amaçlayan bir makine öğrenmesi problemi.
- **Kümeleme:** Verileri benzerliklerine göre gruplara ayırmayı amaçlayan bir makine öğrenmesi problemi.

### Gözetimli ve Gözetimsiz Öğrenme
- **Gözetimli Öğrenme (Supervised Learning):** Etiketlenmiş veri kümeleri kullanılarak modelin eğitildiği bir makine öğrenmesi türüdür.
- **Gözetimsiz Öğrenme (Unsupervised Learning):** Etiketlenmemiş veri kümeleri kullanılarak modelin eğitildiği bir makine öğrenmesi türüdür.

---

## 5. Ders: Veri Bulma ve Oluşturma

### Veri Bulma ve Oluşturma
- **Hazır Veri Setleri:** Veri bilimi projelerinde hazır veri setleri kullanmak yaygın olsa da, projeye özgü veriler toplamak ve oluşturmak daha etkili sonuçlar verebilir.
- **Duygu Analizi:** Metin verilerindeki duygu durumunu (olumlu veya olumsuz) anlamak için, metnin başlangıç ve son kısımlarındaki kelimeler incelenebilir.
- **Etiketli Veri:** Makine öğrenmesi modellerini eğitmek için etiketlenmiş veri kullanmak önemlidir.

---

## 6. Ders: Sürekli Öğrenme ve Yapay Zeka Modelleri

### Sürekli Öğrenme
- **Öğrenmenin Önemi:** Veri bilimi alanındaki hızlı gelişmeler nedeniyle, sürekli öğrenme ve yeni bilgileri takip etme önemlidir.
- **Hedef:** Veri biliminin farklı alanlarında uzmanlaşmak ve derinlemesine bilgi sahibi olmak.

### Yapay Zeka Modelleri
- **Perplexity:** Yapay zeka tarafından üretilen metinlerin kalitesini ölçen bir metrik.
- **Bard:** Google tarafından geliştirilen büyük bir dil modeli.
- **Claude:** Anthropic tarafından geliştirilen bir yapay zeka sohbet robotu.
- **Gemini:** Google tarafından geliştirilen bir multimodal yapay zeka modeli.

---

## 7. Ders: Veri Oluşturma ve Kalitesi

### Veri Oluşturma
- **Random Data:** Gerçek dünya verilerine benzer özellikler taşıyan, sentetik olarak üretilmiş verilerdir.
- **Sentetik Data:** Belirli bir amaca yönelik olarak, anlamlı ilişkiler içerecek şekilde üretilmiş verilerdir.

### Veri Kalitesi
- **Data Kalitesi:** Kaliteli veriler, güvenilir ve doğru sonuçlar elde etmek için önemlidir.
- **Model Kalitesi:** Kullanılan modelin kalitesi de veri kalitesini etkiler.

---

## 8. Ders: Yapay Sinir Ağları

### Yapay Sinir Ağları (YSA)
- **Giriş:** Yapay sinir ağları, insan beyninin bilgi işleme yapısını taklit eden bir hesaplama modelidir.
- **Temel Yapı:** YSA'lar genellikle girdi katmanı, gizli katmanlar ve çıktı katmanından oluşur.
- **Çalışma Prensibi:** İleri besleme (forward propagation) ve geri yayılım (backpropagation) ile çalışır.

---

## 9. Ders: Backpropagation ve TensorFlow

### Backpropagation
- **Backpropagation:** Sinir ağlarında öğrenme için kullanılan bir algoritmadır. Modelin tahmini ile gerçek değer arasındaki farkı hesaplar ve bu hatayı kullanarak modelin parametrelerini günceller.

### TensorFlow
- **TensorFlow:** Google tarafından geliştirilen açık kaynaklı bir derin öğrenme kütüphanesidir.
- **Model Kaydetme ve Yükleme:** Eğitilen bir modeli kaydetmek ve daha sonra tekrar kullanmak için kullanılır.

---

## 10. Ders: CNN (Evrişimli Sinir Ağları)

### CNN (Evrişimli Sinir Ağları)
- **Görüntü Ölçekleme:** Görüntülerin boyutunu küçültmek veya büyütmek için kullanılır.
- **Min. Pooling:** En küçük değerleri seçerek görüntünün boyutunu küçültür.
- **Büyütme:** Görüntüyü büyütmek için kopyala-yapıştır yöntemi kullanılabilir.

---

## 11. Ders: Proje İncelemeleri ve Kayıp Fonksiyonu

### Proje İncelemeleri
- **İnsan Kaynakları ve Müşteri Analizi:** Çalışan verileri ve müşteri verileri üzerinde analizler yapılabilir.
- **Kayıp Fonksiyonu (Loss Function):** Modelin tahminlerinin gerçek değerlerden ne kadar uzak olduğunu ölçer.

---

## 12. Ders: Derin Öğrenme ve Arayüz Oluşturma

### Derin Öğrenme
- **Derin Öğrenme:** Makine öğrenmesinin bir alt alanıdır ve yapay sinir ağlarını kullanarak verilerden karmaşık örüntüleri öğrenir.

### Arayüz Oluşturma
- **Streamlit:** Veri bilimi projeleri için etkileşimli web arayüzleri oluşturmak için kullanılır.
- **Gradio:** Makine öğrenimi modelleri için hızlı ve kolay bir şekilde arayüzler oluşturmak için kullanılır.

---

## 13. Ders: Firebase ve TensorFlow.js

### Firebase
- **Firebase:** Google tarafından geliştirilen bir mobil ve web uygulaması geliştirme platformudur.
- **Firebase ile Web Sitesi Oluşturma:** Firebase konsolunda proje oluşturma ve dağıtım işlemleri.

### TensorFlow.js
- **TensorFlow.js:** JavaScript ile makine öğrenmesi modelleri oluşturmak ve eğitmek için kullanılan bir kütüphanedir.
