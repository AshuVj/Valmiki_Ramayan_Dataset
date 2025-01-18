# 📜 Valmiki Ramayana Dataset – Structure Guide  

## Dataset Overview  
This dataset contains structured Sanskrit shlokas from the Valmiki Ramayana, along with translations, transliterations, and explanations.

## JSON Fields Explained  
Each entry in the JSON dataset contains the following fields:

| Field | Description |
|--------|-------------|
| `kanda` | The book (Kanda) of the Ramayana (e.g., Bala Kanda, Ayodhya Kanda) |
| `sarga` | The chapter (Sarga) within the Kanda |
| `shloka` | The verse number (Shloka) |
| `shloka_text` | The original Sanskrit shloka in Devanagari script |
| `transliteration` | Romanized version of the Sanskrit text (IAST format) |
| `translation` | English translation of the shloka |
| `explanation` | Detailed meaning or commentary on the shloka |
| `comments` | Additional notes or scholarly observations (if available) |

## Example JSON Entry  
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
}

