# NLP Ödev 1: Metin Tabanlı Veri Setleri ile Yapay Zekâ Modelleri Geliştirme

## 1. Proje Amacı
Bu projede, seçilen metin tabanlı bir veri seti üzerinde doğal dil işleme (NLP) teknikleriyle ön işleme, vektörleştirme ve benzerlik analizi adımları uygulanmıştır. Amaç, metinlerin makine öğrenmesi modelleriyle sayısal olarak temsil edilmesi ve benzerliklerinin ölçülmesidir.

## 2. Kullanılan Veri Seti
- **Kaynak:** [Kaggle - Bank Transaction Data](https://www.kaggle.com/datasets/apoorvwatsky/bank-transaction-data)
- **Boyut:** 6 MB

## 3. Proje Klasör Yapısı
proje/
├── nlp.ipynb # Tüm adımların işlendiği Jupyter Notebook
├── requirements.txt # Gerekli kütüphaneler
├── data/
│ ├── bank.xlsx
│ ├── stemmed data.csv
│ ├── lemmatized data.csv
│ ├── tfidf_lemmatized.csv
│ ├── tfidf_stemmed.csv
│ └── ...
├── models/
│ └── ...
└── README.md

## 4. Kurulum ve Gerekli Kütüphaneler
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
