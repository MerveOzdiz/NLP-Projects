# 🎭 Restoran Yorumları Duygu Analizi (NLP Projesi)

## 📌 Proje Hakkında
Bu proje, **Doğal Dil İşleme (Natural Language Processing - NLP)** teknikleri kullanılarak geliştirilmiştir. Amaç, restoran müşterilerinin yaptığı İngilizce yorumları analiz ederek, bu yorumların **Olumlu (Pozitif)** mu yoksa **Olumsuz (Negatif)** mu olduğunu tahmin eden bir yapay zeka modeli oluşturmaktır.

Makine öğrenmesi algoritmalarından **Naive Bayes** kullanılarak metin sınıflandırması yapılmıştır.

## 🚀 Kullanılan Teknolojiler
* **Python 3.x**
* **Pandas & NumPy:** Veri işleme ve manipülasyonu.
* **NLTK (Natural Language Toolkit):** Metin ön işleme (Stemming, Stopwords temizliği).
* **Scikit-Learn:** Makine öğrenmesi modeli (Naive Bayes) ve Vektörleştirme (CountVectorizer).
* **Matplotlib & Seaborn:** Sonuçların görselleştirilmesi (Confusion Matrix).

## ⚙️ Nasıl Çalışır? (Adım Adım)
Proje şu aşamalardan oluşmaktadır:

1.  **Veri Temizliği (Preprocessing):**
    * Noktalama işaretleri ve sayılar Regex ile temizlendi.
    * Tüm harfler küçük harfe (lowercase) çevrildi.
    * **Stemming (Kök Bulma):** Kelimelerin köklerine inildi (örn: "loved" -> "love").
    * **Stopwords:** Anlam taşımayan bağlaçlar (the, is, and vb.) çıkarıldı.

2.  **Öznitelik Çıkarımı (Feature Extraction):**
    * **Bag of Words (BoW)** modeli kullanılarak metin verileri sayısal vektörlere dönüştürüldü.
    * En sık kullanılan 1500 kelime seçilerek bir matris oluşturuldu.

3.  **Modelleme:**
    * Veri seti %80 Eğitim, %20 Test olarak ayrıldı.
    * **Gaussian Naive Bayes** algoritması ile model eğitildi.

## 📊 Sonuçlar
Model, test verisi üzerinde başarılı bir şekilde sınıflandırma yapmıştır. Karmaşıklık Matrisi (Confusion Matrix) ile modelin doğru ve yanlış tahminleri analiz edilmiştir.

