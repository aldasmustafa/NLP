# NLP Ödev 1: Metin Tabanlı Veri Setleri ile Yapay Zekâ Modelleri Geliştirme

## 1. Proje Amacı
Bu projede, seçilen metin tabanlı bir veri seti üzerinde doğal dil işleme (NLP) teknikleriyle ön işleme, vektörleştirme ve benzerlik analizi adımları uygulanmıştır. Amaç, metinlerin makine öğrenmesi modelleriyle sayısal olarak temsil edilmesi ve benzerliklerinin ölçülmesidir.

## 2. Kullanılan Veri Seti
- **Kaynak:** [Kaggle - Bank Transaction Data](https://www.kaggle.com/datasets/apoorvwatsky/bank-transaction-data)  
- **Boyut:** 6 MB

## 3. Proje Klasör Yapısı
```
proje/
├── nlp.ipynb                  # Tüm adımların işlendiği Jupyter Notebook
├── requirements.txt           # Gerekli kütüphaneler
├── data/
│   ├── ai_detect_essays_filtered.csv
│   ├── essays_lemmatized.csv
│   ├── essays_stemmed.csv
│   ├── tfidf_lemmatized.csv
│   ├── tfidf_stemmed.csv
│   └── ...
│   📂 Veri dosyaları: https://drive.google.com/drive/folders/1UGJqj4RXZFYhrM9JNuiv_EW1AmysHLoT?usp=drive_link
├── models/
│   └── ...
│   📂 Model dosyaları: https://drive.google.com/drive/folders/1WfYMtv1BK6r9mruu_WVl0g6H3MDGeXg4?usp=drive_link
└── README.md
```

## 4. Kurulum ve Gerekli Kütüphaneler
Aşağıdaki Python kütüphanelerinin sisteminizde kurulu olması gerekmektedir:

```
pandas
numpy
nltk
gensim
scikit-learn
matplotlib
seaborn
re
collections
ast
shutil
ipython
```

Kurmak için terminalde şunu çalıştırabilirsiniz:
```
pip install -r requirements.txt
```

## 5. Adım Adım Kullanım

### 5.1 Veri İnceleme ve Örnekleme
Veri setinin boyutu, formatı ve örnek satırları analiz edilir.

### 5.2 Zipf Yasası Analizi
Ham, lemmatize ve stem yapılmış veriler için Zipf Yasası grafikleri çizilir.

### 5.3 Ön İşleme (Preprocessing)
Aşağıdaki işlemler uygulanır:
- Küçük harfe çevirme
- Tokenization (kelime ayırma)
- Stopword removal (önemsiz kelimeleri kaldırma)
- Lemmatization (kök hale getirme)
- Stemming (kök kesme)
- Özel karakter temizliği

**Çıktılar:**
- `essays_lemmatized.csv`
- `essays_stemmed.csv`
- `ai_detect_essays_filtered.csv`

### 5.4 TF-IDF Vektörleştirme
TF-IDF yöntemi ile lemmatize ve stem yapılmış metinlerin sayısal vektörleri oluşturulur.

**Çıktılar:**
- `tfidf_lemmatized.csv`
- `tfidf_stemmed.csv`

### 5.5 Word2Vec Model Testi
Hazırlanan Word2Vec modelleriyle kelime benzerliği testleri yapılmıştır.

- Örnek model dosyası: `lemmatized_model_cbow_window2_dim100.model`
- Bir kelime girildiğinde, modele göre en benzer 5 kelime listelenir.
- Not: Model dosyalarının bazıları boyut nedeniyle GitHub'a yüklenmemiştir. Tüm model ve veri dosyaları ilgili Google Drive klasörlerinde yer almaktadır.

📂 [Model dosyaları](https://drive.google.com/drive/folders/1WfYMtv1BK6r9mruu_WVl0g6H3MDGeXg4?usp=drive_link)

---

.
