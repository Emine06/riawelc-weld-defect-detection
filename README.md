# riawelc-weld-defect-detection
Kaynak Hatası Tespit Sistemi - ResNet18 %100 Accuracy
# 🔧 Kaynak Hatası Tespit Sistemi (RIAWELC)

Radyografik kaynak görüntülerinde hata tespiti için derin öğrenme projesi.

## 🏆 Sonuçlar

| Model | Epoch | Test Accuracy |
|-------|-------|---------------|
| Basit CNN | 10 | %87.88 |
| Basit CNN | 20 | %96.97 |
| **ResNet18** | **15** | **%100.00** 🏆 |

## 📊 Veri Seti

- **RIAWELC:** 24,407 radyografik görüntü
- **Sınıflar:** 4 (Çatlak, Nüfuziyet Eksikliği, Gözeneklilik, Hatasız)
- **Kaynak:** [GitHub](https://github.com/stefyste/RIAWELC)

## 🔍 Tespit Edilen Hatalar

- 🔴 **Difetto1:** Çatlak (Crack)
- 🟡 **Difetto2:** Nüfuziyet Eksikliği (Lack of Penetration)
- 🟢 **Difetto4:** Gözeneklilik (Porosity)
- ⚪ **NoDifetto:** Hatasız (No Defect)

## 🚀 Kullanılan Teknolojiler

- Python 3.10
- PyTorch
- ResNet18 (Transfer Learning)
- Gradio (Web Arayüzü)
- Anaconda Jupyter Notebook

## 📂 Proje Yapısı
```
├── riawelc_anaconda.ipynb         # Veri analizi + Model eğitimi
├── riawelc_gradio_resnet18.ipynb  # Gradio arayüzü
└── images/                        # Sonuç grafikleri
```

## 💻 Nasıl Çalıştırılır?

1. Repoyu klonla
2. `conda create -n weld_app python=3.10`
3. `pip install torch torchvision gradio pillow numpy`
4. `riawelc_anaconda.ipynb` çalıştır (model eğitimi)
5. `riawelc_gradio_resnet18.ipynb` çalıştır (arayüz)

## 📖 Referans

Benito Totino, Fanny Spagnolo, Stefania Perri (2022)
