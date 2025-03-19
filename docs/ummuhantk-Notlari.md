# Veri Bilimi Ders Notları

## Veri Bilimi Nedir?

### Tanım
Veri bilimi, ham verilerden anlamlı bilgiler ve içgörüler çıkarmak için istatistik, matematiksel modelleme, yapay zeka ve bilgisayar bilimleri tekniklerini kullanan disiplinler arası bir alan.

### Temel Bileşenler
- **İstatistik ve Matematiksel Analiz**
- **Programlama (Python)**
- **Makine Öğrenmesi**
- **Veri Görselleştirme**
- **Büyük Veri Teknolojileri**

### İşlev ve Amaçları
- Karmaşık verileri analiz etme
- Geleceğe yönelik tahminler yapma
- İş kararlarını destekleme
- Örüntü ve ilişkileri keşfetme

---

## Veri Bilimi Problem Aşamaları
1. **Problemi Anlama**: Veri setini ve çözülmesi gereken soruyu net bir şekilde tanımlama
2. **Veri Toplama**: Gerekli verilerin toplanması
3. **Veri Ön İşleme**: Eksik verileri düzeltme, aykırı değerleri temizleme
4. **Veri Analizi**: İstatistiksel inceleme ve görselleştirme
5. **Model Seçimi ve Eğitimi**: Uygun makine öğrenmesi modelini seçme
6. **Değerlendirme**: Modelin performansını ölçme
7. **Dağıtım**: Modeli gerçek dünya problemlerinde kullanma

---

## Veri Türleri
### **Numerik Veri**
Sayısal değerler (yaş, gelir)  
Örnek: `[25, 50000, 1.75]`

### **Kategorik Veri**
Sınıflandırılmış veriler (cinsiyet, renk)  
Örnek: `["erkek", "kadın", "diğer"]`

---

## Veri Anonimleştirme
- Kişisel bilgileri gizleme
- Örnek yöntemler:
  - Veriyi rastgele karıştırma
  - İsimleri kodlama
  - Hassas bilgileri silme

### **Veri Tipleri**
- **Analog Veri**: Sürekli, kesintisiz sinyaller  
  Örnek: Ses dalgaları
- **Dijital Veri**: Ayrık, sayısal değerler  
  Örnek: Bilgisayar verileri
- **Ham Veri (Raw Data)**: İşlenmemiş, ham bilgi

---

## Aktivasyon Fonksiyonları
- **ReLU**: Doğrusal düzeltme, derin öğrenmede yaygın  
  \( f(x) = \max(0, x) \)
- **Sigmoid**: Olasılık hesaplamalarında kullanılır  
  \( f(x) = \frac{1}{1 + e^{-x}} \)
- **Softmax**: Çok sınıflı sınıflandırmada kullanılır

---

## Performans Metrikleri
- **MSE (Mean Squared Error)**: Ortalama kare hata
- **Loss Fonksiyonu**: Modelin tahmin performansını ölçer

---

## Python ve Kütüphaneler
### Python Veri Türleri
- **Primitive**: Temel veri tipleri (`int`, `float`, `bool`, `str`)
- **Non-Primitive**: Karmaşık veri tipleri (`list`, `dict`, `set`, `tuple`)

### Koşul Operatörleri
- `==`: Tam eşitlik kontrolü
- `!=`: Eşit olmama durumu
- `>`, `<`: Sayısal büyüklük karşılaştırmaları
- `and`: Her iki koşulun da doğru olması gerektiği
- `or`: En az bir koşulun doğru olması durumu
- `not`: Koşulun tersini alma

### Python Döngüler
- **For Döngüsü**: Liste, tuple, string gibi yinelenebilir nesneleri dolaşmak
- **While Döngüsü**: Belirli bir koşul doğru olduğu sürece çalışır
- **Range Fonksiyonu**: Sayısal diziler üretme
- **Break ve Continue**: Döngüyü tamamen durdurma ya da sonraki iterasyona geçme
- **Nested Döngüler**: İç içe geçmiş döngüler

### Popüler Python Kütüphaneleri
#### **Pandas**
- Veri analizi ve işleme
- CSV, Excel gibi formatları okuma
- Veriyi temizleme ve düzenleme

#### **NumPy**
- Çok boyutlu diziler
- Matematiksel ve bilimsel hesaplamalar

#### **Matplotlib**
- Grafik ve çizelge oluşturma
- Çizgi, çubuk, dağılım grafikleri

#### **PyTorch**
- Derin öğrenme ve yapay sinir ağları
- GPU üzerinde hızlı hesaplama

---

## Makine Öğrenmesi Türleri ve Modelleri

### **Gözetimli Öğrenme**
- Etiketli verilerle eğitim
- Örnek: Spam e-posta tespiti, hastalık teşhisi

### **Gözetimsiz Öğrenme**
- Etiketsiz verilerle çalışma
- Örnek: Müşteri segmentasyonu, anomali tespiti


## Makine Öğrenmesi Modelleri

### Doğrusal Regresyon (Linear Regression)
**Kullanım Alanı:** Sürekli değerlerin tahmini (örneğin, ev fiyatı tahmini).

**Açıklama:** Bağımlı değişken (hedef) ile bağımsız değişkenler (özellikler) arasında doğrusal bir ilişki kurar.

---

### Lojistik Regresyon (Logistic Regression)
**Kullanım Alanı:** İkili sınıflandırma problemleri (örneğin, spam tespiti).

**Açıklama:** Olasılık temelli bir modeldir ve sonuçları 0 ile 1 arasında tahmin eder.

---

### Karar Ağaçları (Decision Trees)
**Kullanım Alanı:** Hem sınıflandırma hem de regresyon problemleri.

**Açıklama:** Veriyi dallara ayırarak karar kuralları oluşturur.

---

### Rastgele Orman (Random Forest)
**Kullanım Alanı:** Sınıflandırma ve regresyon.

**Açıklama:** Birden fazla karar ağacının birleşiminden oluşur. Overfitting (aşırı öğrenme) riskini azaltır.

---

### Destek Vektör Makineleri (Support Vector Machines - SVM)
**Kullanım Alanı:** Sınıflandırma ve regresyon.

**Açıklama:** Veriyi en iyi şekilde ayıran bir hiper düzlem bulmaya çalışır.

---

### K-En Yakın Komşu (K-Nearest Neighbors - KNN)
**Kullanım Alanı:** Sınıflandırma ve regresyon.

**Açıklama:** Bir veri noktasının sınıfını, en yakın komşularının sınıflarına göre belirler.

---

### K-Means Kümeleme (K-Means Clustering)
**Kullanım Alanı:** Kümeleme problemleri.

**Açıklama:** Veriyi önceden belirlenen sayıda kümeye ayırır.

---

### Yapay Sinir Ağları (Artificial Neural Networks - ANN)
**Kullanım Alanı:** Karmaşık problemler (örneğin, görüntü tanıma, doğal dil işleme).

**Açıklama:** İnsan beynindeki sinir hücrelerini taklit eder. Derin öğrenme (Deep Learning) modellerinin temelidir.

---

### Gradient Boosting Modelleri (XGBoost, LightGBM, CatBoost)
**Kullanım Alanı:** Sınıflandırma ve regresyon.

**Açıklama:** Zayıf modelleri birleştirerek güçlü bir model oluşturur.


---

## Destekleyici Teknolojiler
- **Regex**: Metin desenlerini tanımlama
- **Beautiful Soup**: Web içerik çıkarma
- **Back Propagation**: Sinir ağı eğitim algoritması

---

## Veri Bilimi Platform ve Araçları
- **Hugging Face**: Makine öğrenimi kullanarak uygulamalar geliştirmek için hesaplama araçları sağlayan bir platform
- **Kaggle**: Veri bilimi yarışmaları ve veri setleri
- **Streamlit**: Hızlı prototipleme ve makine öğrenmesi uygulamaları
- **Firebase**: Gerçek zamanlı veri senkronizasyonu
