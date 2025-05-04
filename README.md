# NLP Ödev 1: Metin Tabanlı Veri Setleri ile Yapay Zekâ Modelleri Geliştirme

## 1. Proje Amacı
Bu projede, seçilen metin tabanlı bir veri seti üzerinde doğal dil işleme (NLP) teknikleriyle ön işleme, vektörleştirme ve benzerlik analizi adımları uygulanmıştır. Amaç, metinlerin makine öğrenmesi modelleriyle sayısal olarak temsil edilmesi ve benzerliklerinin ölçülmesidir.

## 2. Kullanılan Veri Seti
- **Kaynak:** [Kaggle - Bank Transaction Data](https://www.kaggle.com/datasets/apoorvwatsky/bank-transaction-data)  
- **Boyut:** 6 MB

## 3. Proje Klasör Yapısı
```
proje/
├── nlp.ipynb               # Tüm adımların işlendiği Jupyter Notebook
├── requirements.txt        # Gerekli kütüphaneler
├── data/
│   ├── bank.xlsx
│   ├── stemmed data.csv
│   ├── lemmatized data.csv
│   ├── tfidf_lemmatized.csv
│   ├── tfidf_stemmed.csv
│   └── ...
├── models/
│   └── ...
└── README.md
```

📂 [Google Drive klasörüne buradan erişebilirsiniz.](https://drive.google.com/drive/folders/1WfYMtv1BK6r9mruu_WVl0g6H3MDGeXg4?usp=drive_link)

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
- `sentences_lemmatized.csv`
- `sentences_stemmed.csv`

### 5.4 TF-IDF Vektörleştirme
TF-IDF yöntemi ile lemmatize ve stem yapılmış metinlerin sayısal vektörleri oluşturulur.

**Çıktılar:**
- `tfidf_lemmatized.csv`
- `tfidf_stemmed.csv`

---

📌 Geri bildirim ve katkılar için pull request gönderebilirsiniz.
