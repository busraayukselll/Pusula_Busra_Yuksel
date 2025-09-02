# Pusula_Busra_Yuksel
Pusula Talent Academy Data Science Intern Case Study kapsamında verilen verisetinin  EDA ve veri ön işleme çalışması.
# Pusula Talent Academy - Data Science Intern Case Study

**Ad Soyad:** Büşra Yüksel 
**E-posta:** busraayukselll@gmail.com  

---

## 📌 Genel Bakış
Bu repo, **Pusula Talent Academy Data Science Intern Case Study** için hazırlanmıştır.  
Veri seti, **Hastaların Tedavi sürelerine**  ilişkin olup **2235 gözlem** ve **13 özelliğe** sahiptir.  

- **Hedef Değişken:** `TedaviSuresi` (seans sayısı olarak tedavi süresi)  
- **Amaç:** Veri üzerinde ayrıntılı Keşifsel Veri Analizi (EDA) yapmak ve veriyi *modelleme için hazır hale getirmek*.  

---

## 🧾 Yapılan Çalışmalar

### 1. Keşifsel Veri Analizi (EDA)
- Veri seti yapısının incelenmesi (`info`, `describe`)  
- Eksik değerlerin ve anomalilerin belirlenmesi  
- **Sayısal değişkenlerin** görselleştirilmesi (histogram, boxplot)  
- **Kategorik değişkenlerin** görselleştirilmesi (barplot, countplot)  
- Değişkenler arası ilişkilerin incelenmesi (**scatter plot, korelasyon ısı haritası, pivot heatmap**)  
- Liste biçimindeki alanların (`Tanilar`, `Alerji`, `KronikHastalik`, `UygulamaYerleri`) explode edilerek analiz edilmesi  

### 2. Veri Ön İşleme (Preprocessing)
- Süre sütunlarının sayısallaştırılması:
  - `TedaviSuresi` → `TedaviSuresi_num`  
  - `UygulamaSuresi` → `UygulamaSuresi_dk`  
- Eksik değerlerin doldurulması:
  - **Sayısal kolonlar** → median ile  
  - **Kategorik kolonlar** → `"bilinmiyor"` etiketi ile  
  - **Liste tabanlı kolonlar** → boş değer ile  
- Metin kolonlarının normalize edilmesi (küçük harfe çevirme, boşluk temizleme, basit mapping işlemleri)  
- Ek özelliklerin üretilmesi:
  - Liste kolonlarından eleman sayısı (`*_count`)  
  - En sık görülen N değer için one-hot encoding  
- Tekil kategorik değişkenlerin one-hot encoding ile dönüştürülmesi (`Cinsiyet`, `KanGrubu`, `Uyruk`, `Bolum`, `TedaviAdi`)  

---

## 📂 Repo İçeriği
- `Pusula_Intern_DataScience.ipynb` → EDA ve preprocessing adımlarının tamamı  

