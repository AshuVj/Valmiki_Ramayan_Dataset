# 🛠️ Preprocessing Notes – Valmiki Ramayana Dataset

## 📌 Overview
This document explains the preprocessing steps applied to **Valmiki Ramayana Dataset**, including:
* **Data Collection & Sources**
* **Cleaning & Formatting**
* **Handling Merged Shlokas & Missing Values**
* **Challenges & Future Work**

## 🔍 1. Data Collection & Sources
The dataset was **compiled from multiple online sources**, structured for machine readability.

### **Primary Data Sources:**
* 🔗 **GitaSuperset** – Scraped Sanskrit shlokas, translations, and metadata
* 🔗 **IIT Kanpur Sanskrit Repository** – Used as reference for transliteration corrections
* 📚 **M.N. Dutt's English Translation (1891-1894)** – Included for validation

## 🧹 2. Data Cleaning & Formatting
### **Standardization Applied:**
✅ **Converted Sanskrit text to UTF-8 encoding** for proper rendering  
✅ **Removed extra spaces & special characters** from extracted text  
✅ **Ensured proper JSON formatting** for structured storage  
✅ **Normalized transliteration using IAST (International Alphabet of Sanskrit Transliteration)**

## 🛑 3. Handling Merged Shlokas
### 🔍 **Issue:**
* Some shlokas were merged due to **OCR errors or source formatting**
* Example of merged shloka:
```
"shloka_text": "तमेवं गुणसम्पन्नं रामं सत्यपराक्रमम्।।1.1.19।। ज्येष्ठं श्रेष्ठगुणैर्युक्तं प्रियं दशरथस्सुतम्।।"
```
* This caused misalignment in translation & explanation fields

### **Solution Implemented:**
✔️ **Detection:** A script was written to identify merged shlokas based on **duplicate numbering patterns (e.g., 1.1.19, 1.1.20 appearing together)**  
✔️ **Manual Review:** Detected entries were flagged for **manual verification & correction**  
✔️ **Future Plan:** AI-based segmentation might be explored

## 🔍 4. Handling Missing Values (Null Entries)
### 🔍 **Issue:**
* Some **translations, explanations, and transliterations were missing** due to incomplete data sources
* Example:
```json
    {
        "kanda": "Uttara Kanda",
        "sarga": 18,
        "shloka": 20,
        "shloka_text": "ततस्तं निर्जितं मत्वा घोषयामास वै शुकः । रावणो जयतीत्युच्चैर्हर्षान्नादं विमुक्तवान् ।। 7.18.20 ।।",
        "transliteration": "tatastaṃ nirjitaṃ matvā ghoṣayāmāsa vai śukaḥ | rāvaṇo jayatītyuccairharṣānnādaṃ vimuktavān || 7.18.20 ||",
        "translation": null,
        "explanation": null,
        "comments": null
    }
```

### **Solution Implemented:**
✔️ **Flagged Missing Entries:** Entries with `null` values were marked for further improvement  
✔️ **Cross-referenced other sources** (GitaPress, IITK) to manually fill gaps **where possible**  
✔️ **Future Plan:** AI-based translation (using **IndicBERT / MuRIL**) to fill gaps **automatically**

## ⚠️ 5. Known Challenges & Future Work
🔸 **Shloka Segmentation**: AI-based segmentation might be used for better handling of **merged texts**  
🔸 **Translation Completion**: Missing translations may be auto-filled with **AI models trained on Sanskrit texts**  
🔸 **Validation with Scholars**: Cross-verification with Sanskrit scholars can **improve accuracy**

## 🔗 6. Contribution Guide
👨‍💻 If you want to **help improve the dataset**, follow these steps:

1️⃣ **Identify errors/missing translations** – Open an **issue** on GitHub  
2️⃣ **Suggest better corrections** – Submit a **Pull Request** with proper references  
3️⃣ **Provide additional scholarly sources** – Help refine **translations & explanations**

## 🕉️ Final Thought
*"May this dataset serve as a foundation for Sanskrit AI research & preservation of ancient knowledge."*

🙏 **Jai Shri Ram!** 🚀