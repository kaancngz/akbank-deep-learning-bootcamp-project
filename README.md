# Beyin Tümörü Sınıflandırması  
*Akbank & Global AI Hub Deep Learning Bootcamp Bitirme Projesi*  

Bu proje, MR görüntülerinden **Glioma, Meningioma, Pituitary tümörü** ve **Normal beyin dokusunu** derin öğrenme yöntemleriyle sınıflandırmayı amaçlamaktadır.  

---

## Giriş  

Projemizde kullanılan veri seti [Brain Tumor MRI Dataset](https://www.kaggle.com/datasets) olup, eğitim ve test olmak üzere ikiye ayrılmıştır.  
- Eğitim: `Training` klasörü  
- Test: `Testing` klasörü  
- Sınıflar: **Glioma, Meningioma, No Tumor, Pituitary**  

Çalışmada **VGG16 transfer learning** yöntemi uygulanmıştır. Veri ön işleme, data augmentation, model mimarisi tasarımı ve açıklanabilir yapay zeka (Grad-CAM) ile model yorumlama adımları yer almaktadır.  

---

## Metrikler  

Modelin performansı test setinde şu şekilde elde edilmiştir:  

- **Accuracy (Doğruluk):** ~%83  
- **Loss / Accuracy Eğrileri:** Eğitim süresince düzenli iyileşme kaydedilmiştir.  
- **Confusion Matrix:**  
  - “No Tumor” ve “Pituitary” sınıflarında yüksek başarı.  
  - “Glioma” ve “Meningioma” sınıflarında karışıklık eğilimi.  
- **Grad-CAM Görselleştirmeleri:** Modelin odaklandığı bölgeler incelenmiştir.  

---

## Ekler  

- `notebooks/bootcamp_proje.ipynb` → Veri analizi, eğitim ve değerlendirme adımları.  
- `saved_models/brain_tumor_classification_model.keras` → Eğitilmiş model dosyası.  

---

## Sonuç ve Gelecek Çalışmalar  

Model 4 sınıfta başarılı sonuçlar vermiştir. Ancak daha ileri doğruluk için:  
- Daha güçlü mimariler (ResNet, EfficientNet vb.)  
- Hiperparametre optimizasyonu  
- Daha geniş veri seti  
- Ensemble yöntemleri  

gelecekte değerlendirilebilir. Ayrıca modelin klinik geçerliliği için farklı veri kaynaklarında test edilmesi önerilir.  

---

## Linkler  

- [Kaggle Notebook](https://www.kaggle.com/code/kaancengizx/bootcamp-proje)  

