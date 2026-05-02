# 🛡️ Semantic Plagiarism Detector

Yapay Zeka destekli, semantik (anlamsal) intihal tespit sistemi. Bu araç, sadece kelime bazlı eşleşmeleri değil, cümlelerin arkasındaki mantıksal akışı ve bağlamı analiz ederek intihal riskini raporlar.

## 🚀 Proje Hakkında
Geleneksel intihal tespit yazılımları, genellikle birebir kopyalanmış (copy-paste) metinleri bulmaya odaklanır. **Semantic Plagiarism Detector** ise `Sentence-Transformers` (vektörleştirme) ve `Gemini 1.5 Flash` (derinlemesine analiz) modellerini kullanarak, kelimeleri değiştirilmiş (paraphrase edilmiş) içerikleri bile yüksek doğrulukla yakalar.

## ✨ Temel Özellikler
- **Semantik Analiz:** Metinleri vektör uzayına taşıyarak anlamsal benzerlik araması (Cosine Similarity).
- **LLM Destekli Raporlama:** Tespit edilen benzerliklerin, yapay zeka tarafından akademik bir dille yorumlanması.
- **Modern Web Arayüzü:** `Streamlit` ile geliştirilmiş, kullanıcı dostu dosya yükleme ve analiz paneli.
- **Otomatik Raporlama:** Analiz sonuçlarını `JSON` formatında indirilebilir rapor haline getirme.
- **Hata Yönetimi:** Dosya bozulmalarına ve veri hatalarına karşı geliştirilmiş güvenlik katmanları.

## 🛠️ Kullanılan Teknolojiler
- **Backend:** Python
- **AI/ML:** Google Gemini API, Sentence-Transformers, FAISS (Vektör Veritabanı)
- **UI:** Streamlit
- **Doküman İşleme:** PyPDF2, python-docx

## Görseller
<img width="498" height="251" alt="image" src="https://github.com/user-attachments/assets/9c735c65-cf8a-425f-97e8-584353cf6a1f" />
<img width="482" height="243" alt="image" src="https://github.com/user-attachments/assets/9d9b2a90-8a05-432b-a7d8-518522c87c89" />
<img width="750" height="380" alt="image" src="https://github.com/user-attachments/assets/86ab5ba2-e41c-41cc-b59a-955fa1e19662" />
<img width="749" height="373" alt="image" src="https://github.com/user-attachments/assets/1cd7ee7d-a44f-4c20-ab17-cf4589c6343d" />


## 📂 Proje Yapısı
```text
SemanticPlagiarismDetector/
├── app.py              # Streamlit Web Arayüzü
├── main.py             # Analiz boru hattı (Pipeline)
├── config/
│   └── settings.py     # Yapılandırma ve Eşik değerleri
├── src/
│   ├── core/           # Motor ve Analiz mantığı
│   └── nlp/            # İşleme ve Chunking mantığı
├── requirements.txt    # Bağımlılık listesi
└── README.md


