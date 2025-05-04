NLP Ödev 1: Metin Tabanlı Veri Setleri ile Yapay Zekâ Modelleri Geliştirme
1. Proje Amacı
Bu projede, seçilen metin tabanlı bir veri seti üzerinde doğal dil işleme (NLP) teknikleriyle ön işleme, vektörleştirme ve benzerlik analizi adımları uygulanmıştır.
Amaç, metinlerin makine öğrenmesi modelleriyle sayısal olarak temsil edilmesi ve benzerliklerinin ölçülmesidir.

2. Kullanılan Veri Seti
Kaynak: https://www.kaggle.com/datasets/apoorvwatsky/bank-transaction-data
Boyut:6mb

3. Proje Klasör Yapısı
proje/
│
├── nlp.ipynb                  # Tüm adımların işlendiği Jupyter Notebook
├── requirements.txt           # Gerekli kütüphaneler
├── data/
│   ├── bank.xlsx
│   ├── stemmed data.csv
│   ├── lemmatized data.csv
│   ├── tfidf_lemmatized.csv
│   ├── tfidf_stemmed.csv
│   └── ... 
├── models/
│   └── ... https://drive.google.com/drive/folders/1WfYMtv1BK6r9mruu_WVl0g6H3MDGeXg4?usp=drive_link
└── README.md

4. Kurulum ve Gerekli Kütüphaneler

Aşağıdaki Python kütüphaneleri gereklidir:
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

6. Adım Adım Kullanım
 Veri İnceleme ve Örnekleme
Veri setinin boyutu, formatı ve örnek satırı ekrana yazdırılır.
 Zipf Yasası Analizi
Ham, lemmatized ve stemmed veri için Zipf grafikleri oluşturulur.
 Ön İşleme (Preprocessing)
Stopword removal, tokenization, lowercasing, lemmatization, stemming ve özel karakter temizliği yapılır.
Çıktılar:

essays_lemmatized.csv
essays_stemmed.csv
sentences_lemmatized.csv
sentences_stemmed.csv
4. TF-IDF Vektörleştirme
TF-IDF ile lemmatize ve stem yapılmış metinlerin vektörleştirilmesi sağlanır.
Çıktılar:

tfidf_lemmatized.csv
tfidf_stemmed.csv
