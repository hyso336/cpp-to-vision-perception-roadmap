# 📘 cpp-to-perception-roadmap

Modern C++ ile **bilgisayarlı görü (computer vision)** ve **algılama (perception)** sistemlerine adım adım ilerleyen kapsamlı bir öğrenme ve uygulama yol haritası.  
Bu repo, C++ temellerinden başlayarak **OpenCV, LibTorch, TorchScript, CIFAR-10 ve YOLO** tabanlı gerçek zamanlı algılama pipeline’larına kadar uzanan **12 bölümlük eksiksiz bir mühendislik eğitim setidir.**

---

## 🎯 Amaç
Bu çalışma, C++ bilen veya öğrenen bir kişinin aşağıdaki alanlarda uzmanlaşmasını hedefler:

🔹 Görüntü işleme (**OpenCV**)  
🔹 Derin öğrenme inference (**LibTorch / TorchScript**)  
🔹 **CIFAR-10** ve **YOLO** modelleriyle çalışmak  
🔹 Modüler **Perception Node** mimarisi kurmak  
🔹 Modern C++ proje yapıları (**CMake**)  
🔹 Gerçek zamanlı algılama sistemi tasarlamak  

Hedef, basit kodlardan çıkıp **gerçek bir algılama pipeline’ı** geliştirme becerisine ulaşmaktır.

---

## 📂 Bölümler (Klasör Yapısı)

`01-temel-cpp`  
`02-fonksiyon-ve-pointer`  
`03-pointer-ve-bellek`  
`04-oop-temelleri`  
`05-ileri-oop`  
`06-veri-yapilari`  
`07-cpp-kolayliklari`  
`08-hata-ayiklama-try-catch`  
`09-cmake`  
`10-opencv`  
`11-libtorch`  
`12-perception-node`  

---

# 🧩 Öğrenme Yolculuğu – Katmanlı Yapı

Aşağıdaki yapı, C++ temelinden başlayıp gerçek zamanlı bir algılama modülüne (Perception Node) uzanan öğrenme akışını göstermektedir.  
Her bölüm bir sonrakine temel oluşturur ve toplam **151 farklı örnek / algoritma / proje** içerir.

---

### 🔹 **01 – Temel C++**  
**12 temel örnek**

----

### 🔹 **02 – Fonksiyon & Pointer**  
**10 örnek**

----

### 🔹 **03 – Pointer & Bellek Yönetimi**  
**15 örnek**

---

### 🔹 **04 – OOP Temelleri**  
**8 örnek**

----

### 🔹 **05 – İleri OOP**  
**10 örnek**

----

### 🔹 **06 – Veri Yapıları**  
📌 20 dizi algoritması  
📌 8 linked list algoritması  
📌 9 sıralama algoritması  
➡️ **Toplam: 37 algoritma**

---

### 🔹 **07 – C++ Kolaylıkları**  
📌 10 integer algoritması  
📌 10 string algoritması  
📌 10 vector uygulaması  
➡️ **Toplam: 30 örnek**

---

### 🔹 **08 – Hata Ayıklama**  
**5 örnek**

----

### 🔹 **09 – Modern CMake**  
**4 proje**

---

### 🔹 **10 – OpenCV**  
📌 10 görüntü işleme uygulaması  
📌 11 video akış uygulaması  
➡️ **Toplam: 21 örnek**

---

### 🔹 **11 – LibTorch**  
**8 örnek / proje**

---

### 🔹 **12 – Perception Node**  
📌 5 tam algılama projesi  
📌 ImageFrame & DetectedObject yapıları  
📌 PerceptionNode mimarisi  
📌 CIFAR10 & YOLO inference pipeline  

---

### **📌 Genel Toplam**
**12 bölüm – 151 uygulama / algoritma / proje**

Bu katmanlı yapı, temel programlama becerilerinden başlayıp gerçek zamanlı algılama sistemi geliştirme seviyesine ulaşan uçtan uca bir mühendislik yolculuğunu temsil eder.

---

# 🧩 Genel Öğrenme Diyagramı

Bu diyagram, C++ temelinden başlayıp gerçek zamanlı algılama modülüne (Perception Node) kadar uzanan tek yönlü ve katmanlı bir öğrenme yolunu ifade eder:

```bash
[ 01 Temel C++ ]
        ↓
[ 02 Fonksiyon & Pointer ]
        ↓
[ 03 Pointer & Bellek ]
        ↓
[ 04 OOP Temelleri ]
        ↓
[ 05 İleri OOP ]
        ↓
[ 06–07 Veri Yapıları & Kolaylıklar ]
        ↓
[ 08–09 Hata Ayıklama & CMake ]
        ↓
[ 10 OpenCV ]
        ↓
[ 11 LibTorch ]
        ↓
[ 12 Perception Node ]
```

---

## 🔁 Algılama Pipeline Akış Şeması (PerceptionNode)
```bash
flowchart LR
A[📷 Camera / Video Source] --> B[🧩 ImageFrame oluştur]
B --> C[⚙️ Preprocess (cv::Mat → Tensor)]
C --> D[🧠 Model Inference (LibTorch / TorchScript)]
D --> E[📦 Postprocess (bbox, score, class)]
E --> F[📋 DetectedObject listesi]
F --> G[🖥️ Çizim & Görselleştirme (OpenCV window)]
```

Bu akış şeması, 12-perception-node bölümünde geliştirilen projelerin temel mimarisidir:

* Giriş: Kamera veya video kaynağı

* Orta Katman: Preprocess → Inference → Postprocess

* Çıkış: Tespit edilen nesneler + görselleştirme

----

# 🚀 Sonuç

Bu repo, C++ temellerinden başlayarak gerçek zamanlı algılama sistemlerinin çekirdek tasarımına uzanan tam kapsamlı bir Perception Roadmap sunar.
Her bölüm, sayısal olarak tanımlanmış örnekler ve projelerle gerçek mühendislik pratiğini öğretir.
C++ → OpenCV → LibTorch → PerceptionNode zincirini uçtan uca görmek isteyenler için referans niteliğinde bir çalışmadır.



Pair Extraordinaire test contribution

