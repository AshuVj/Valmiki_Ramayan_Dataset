# 📜 Valmiki Ramayana Dataset  
**A structured, machine-readable dataset of Valmiki Ramayana, including Sanskrit shlokas, translations, and explanations.**  

![GitHub stars](https://img.shields.io/github/stars/AshuVj/Valmiki_Ramayan_Dataset?style=social)  
![License](https://img.shields.io/badge/license-MIT-blue)  

---

## 📌 About the Dataset  
This is an **open-source dataset** for **Valmiki Ramayana**, containing:
- 📜 **Sanskrit Shlokas** (Original script)
- 🏛 **Romanized Transliterations**  
- 📖 **English Translations** (Word-by-word & sentence meanings)  
- 📝 **Explanations & Commentary**  

🔹 **Intended Uses:**  
- AI/NLP Research & Sanskrit Language Processing  
- Computational Linguistics & Machine Learning  
- Sanskrit Studies & Digital Archives  

---

## 📂 Dataset Structure  
```
Valmiki_Ramayan_Dataset/
│── data/                        # Main dataset
│   ├── Valmiki_Ramayan_Shlokas.json  # Structured shloka dataset
│
│── resources/                   # Scholarly resources, PDFs, external datasets
│   ├── MN_Dutt_Volume_1_2.pdf
│   ├── MN_Dutt_Volume_3_5.pdf
│   ├── MN_Dutt_Volume_6.pdf
│   ├── MN_Dutt_Volume_7.pdf
│
│── docs/                        # Additional explanations or future work
│   ├── dataset_structure.md     # Explanation of dataset columns & structure
│   ├── preprocessing_notes.md   # Notes on dataset processing
│
│── Resources.md                 # 📚 One-stop scholarly reference (✅ Completed!)
│── README.md                    # 🚀 This file!
│── LICENSE                      # 📜 MIT License
│── .gitignore                   # GitHub ignore file
```

---

## 🔍 Sample Data Format  
Each entry in the JSON dataset follows this structure:  
```json
    {
        "kanda": "Bala Kanda",
        "sarga": 1,
        "shloka": 1,
        "shloka_text": "तपस्स्वाध्यायनिरतं तपस्वी वाग्विदां वरम् । नारदं परिपप्रच्छ वाल्मीकिर्मुनिपुङ्गवम् ।।1.1.1।।",
        "transliteration": "tapassvādhyāyanirataṁ tapasvī vāgvidāṁ varam। nāradaṁ paripapraccha vālmīkir munipuṅgavam।।",
        "translation": "तपस्वी ascetic, वाल्मीकि: Valmiki, तप: स्वाध्यायनिरतम् highly delighted in the practice of religious austerities and study of vedas, वाग्विदां वरम् eloquent among the knowledgeable, मुनिपुङ्गवम् preeminent among sages, नारदम् Narada, परिपप्रच्छ enquired.",
        "explanation": "Ascetic Valmiki enquired of Narada, preeminent among the sages ever engaged in the practice of religious austerities or study of the Vedas and best among the eloquent.",
        "comments": "Saint Narada visits hermitage of Valmiki -- Valmiki queries about a single perfect individual bestowed with all good qualities enumerated by him -- Narada, knower of past, present and future, identifies such a man -- describes virtues, qualities of Sri Rama -- narrates briefly the story of his life."
    },
```

---

## 🔗 **Sources & Credits**  
This dataset was compiled from **verified Sanskrit corpora and structured for better usability**, referencing key translations and academic sources.

📚 **Primary Texts & Translations:**  
- 📚  **M.N. Dutt's English Translation (1891-1894)** [(Archive.org)](https://archive.org)  
- 🏛  **IIT Kanpur Gita Supersite** [(IIT-Kanpur)](https://www.valmiki.iitk.ac.in/)  
- 🌐 **Gyaandweep** [(Gyaandweep.com)](https://www.gyaandweep.com)  

🏛 **Data Structuring & Processing:**  
- Extracted & cleaned text from **multiple verified sources**  
- Reformatted for **AI/NLP usability**  
- Included **word-by-word translations & explanations**  

🔹 **Note:** *The dataset is continuously improving. Contributions are welcome to enhance accuracy!*  

---

## 📥 **Download & Usage**  
### **Clone the Repository**  
```bash
git clone https://github.com/AshuVj/Valmiki_Ramayan_Dataset.git
```
Or download the dataset directly:  
🔗 [**Download `Valmiki_Ramayan_Shlokas.json`**](https://github.com/AshuVj/Valmiki_Ramayan_Dataset/raw/main/data/Valmiki_Ramayan_Shlokas.json)  

---

## 🎯 **Contribute & Improve**  
🚀 Want to **improve the dataset** or **add missing translations**?  

1️⃣ **[Open an Issue](https://github.com/AshuVj/Valmiki_Ramayan_Dataset/issues)** (Report errors, suggest improvements)  
2️⃣ **Submit a Pull Request** (Fix errors, add better explanations, or help refine the dataset)  
3️⃣ **Contribute additional scholarly sources**  

🙌 **Let's make Sanskrit AI & NLP stronger together!** 🚀  

---

## ⚠️ **Known Issues & Future Improvements**
This dataset is a **work in progress**, and we are actively working on refining it.

### ❌ **Current Challenges**
- 📜 **Merged Shlokas:** Some shlokas are incorrectly combined due to OCR/formatting errors  
- 🔍 **Missing Translations & Explanations:** Some entries lack **English meanings and explanations**  
- 📖 **Verification Needed:** A thorough **manual validation** of Sanskrit-to-English translations is pending  

👨‍💻 **We welcome contributions!** If you find errors or can help improve the dataset, please open an issue or submit a PR. 🙌  

---

## 📜 **License**  
This dataset is released under the **MIT License** – Free to use for **research, learning, and non-commercial projects**.  

---

## 🕉️ **Conclusion – A Ramayana Shloka for Wisdom & Knowledge**  

**न हि ज्ञानेन सदृशं पवित्रमिह विद्यते।  
तत्स्वयं योगसंसिद्धः कालेनात्मनि विन्दति॥**  

*(There is nothing as purifying as knowledge. One who attains self-realization through devotion to learning finds wisdom within himself in due time.)*