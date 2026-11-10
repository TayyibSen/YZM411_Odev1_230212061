# YZM 411 Bilgisayarlı Görü — Ödev #1
**Renk Uzayları, Aydınlatma Dönüşümleri ve İki Boyutlu Örnekleme Analizi**

* **Öğrenci Adı Soyadı:** Muhammed Tayyib Şen
* **Öğrenci Numarası:** 230212061
* **Ders Sorumlusu:** Öğr. Gör. Melisa GÖZET
* **Teslim Tarihi:** 10 Kasım 2026

---

##  Proje Özeti
Bu çalışma kapsamında sabit bir masaüstü sahnesi üzerinde üç farklı aydınlatma koşulunda (Karanlık, Normal, Aydınlık) çekilen fotoğraflar üzerinden sayısal görüntü analizi, RGB ve HSV renk uzaylarının ışık değişimine dayanıklılığı, noktasal parlaklık ve gama dönüşümleri ile iki boyutlu örnekleme/çözünürlük kaybı (`INTER_NEAREST` vs. `INTER_AREA`) deneysel ve sayısal olarak incelenmiştir.

---

##  Depo İçeriği

* **`YZM411_Odev1.ipynb`**: Tüm görüntü işleme, homografi hizalama, maskeleme, gama dönüşümü ve küçültme/profil analizlerini içeren çalıştırılabilir Jupyter/Colab not defteri.
* **`YZM411_Odev1_Rapor_230212061.pdf`**: İki sayfalık resmi akademik ödev raporu (Deney hipotezleri, karşılaştırma tabloları, grafikler ve metodolojik çıkarımlar).
* **`sonuc_tablosu.csv`**: Kontrol pikselleri, ortalama parlaklıklar, maske oranları ve dönüşüm sonuçlarını içeren sayısal veri tablosu.
* **`IMG20261110163354.jpg`**: Gölge / Karanlık test fotoğrafı.
* **`IMG20261110163420.jpg`**: Normal ışık (referans) test fotoğrafı.
* **`IMG20261110163440.jpg`**: Aydınlık / Yönlendirilmiş lamba test fotoğrafı.

---

##  Kullanılan Kütüphaneler ve Sürümler

* **Python:** 3.12+ / 3.13
* **OpenCV (`cv2`):** Görüntü okuma, BGR/RGB dönüşümü, SIFT homografi ve yeniden boyutlandırma
* **NumPy:** Dizi işlemleri, kırpma (`clip`) ve matematiksel dönüşümler
* **Matplotlib:** Maske, profil ve karşılaştırma görselleştirmeleri
* **Pandas:** Sayısal sonuçların tablolandırılması ve CSV aktarımı

---

##  Çalıştırma Talimatı

1. Girdi fotoğraflarını (`IMG*.jpg`) çalışma dizinine veya Google Colab ortamına yükleyin.
2. `YZM411_Odev1.ipynb` dosyasını sırasıyla yukarıdan aşağıya çalıştırın:
   ```bash
   jupyter notebook YZM411_Odev1.ipynb
