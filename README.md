---
language:
  - ug
license: mit
task_categories:
  - text-generation
  - fill-mask
pretty_name: Uyghur AI Corpus
homepage: https://huggingface.co/datasets/Uyghur-Corpus/Uyghur-Corpus
tags:
  - nlp
  - llm
  - uyghur
  - uighur
  - parquet
  - text-corpus
dataset_info:
  features:
    - name: title
      dtype: string
    - name: text
      dtype: string
    - name: author
      dtype: string
    - name: source
      dtype: string
    - name: date
      dtype: string
    - name: translator
      dtype: string
---

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "Uyghur AI Corpus",
  "alternateName": [
    "ئۇيغۇرچە سۈنئىي ئىدراك خەزىنىسى",
    "Uyghur Corpus",
    "Uygurca Metin Veri Seti",
    "维吾尔语文本数据集"
  ],
  "description": "An open-source, cleaned Uyghur text dataset for NLP, language modeling, and text processing.",
  "url": "https://huggingface.co/datasets/Uyghur-Corpus/Uyghur-Corpus",
  "keywords": "Uyghur, Uighur, ئۇيغۇر, ئۇيغۇرچە, Uyghur NLP, ug, uig, ISO 639-3, Parquet, 维吾尔语",
  "inLanguage": "ug",
  "license": "https://opensource.org/licenses/MIT",
  "isAccessibleForFree": true
}
</script>

# 📚 Uyghur AI Corpus | ئۇيغۇرچە سۈنئىي ئىدراك خەزىنىسى

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Hugging%20Face-yellow)](https://huggingface.co/datasets/Uyghur-Corpus/Uyghur-Corpus)
[![Language](https://img.shields.io/badge/Language-Uyghur%20(ug%20%7C%20uig)-red)](#)
[![Format](https://img.shields.io/badge/Format-Parquet-green)](#)
[![Last Commit](https://img.shields.io/github/last-commit/Uyghur-Corpus/Uyghur-Corpus?label=Last%20Update&color=blue)](https://github.com/Uyghur-Corpus/Uyghur-Corpus/commits/main)
[![Repo Size](https://img.shields.io/github/repo-size/Uyghur-Corpus/Uyghur-Corpus?label=Total%20Size&color=orange)](https://github.com/Uyghur-Corpus/Uyghur-Corpus)

ئۇيغۇر تىلىدىكى تەبىئىي تىل بىر تەرەپ قىلىش (NLP)، چوڭ تىل مودېللىرى (LLM) ۋە تېكىست ئانالىزى ئۈچۈن تور مەنبەلىرىدىن يىغىلىپ تازىلانغان ئوچۇق مەنبەلىك سانلىق مەلۇمات ئامبىرى.

An open-source, cleaned Uyghur text corpus designed for NLP experiments, language modeling, and computational linguistics.

---

### 📊 سانلىق مەلۇمات ھەققىدە / Dataset Info

| كۆرسەتكۈچ / Attribute | تەپسىلاتى / Details |
| :--- | :--- |
| **تىلى (Language)** | ئۇيغۇرچە / Uyghur (`ug` / `uig` / ISO 639-3) |
| **ھۆججەت تىپى (Format)** | Apache Parquet (ئىخچام ۋە تېز بىر تەرەپ قىلىنىدۇ) |
| **تازىلىنىشى (Cleaning)** | تەكرار مەزمۇنلار ۋە كېرەكسىز بەلگىلەر سۈزۈلگەن |
| **ئىجازەتنامە (License)** | MIT License |

---

### 💎 مەنبە ۋە ئەسكەرتىش / Sources & Attribution

بۇ ئامباردىكى مەزمۇنلار تور مۇھىتىدىكى ئوچۇق يازما، ماقالە ۋە ئەدەبىي مەنبەلەردىن يىغىپ تۈزۈلدى.

- ئەسلى يازغۇچى ۋە تېكىست مەنبەلىرىگە ھۆرمەت قىلىش ئۈچۈن، تېكىستلەردىكى ئاپتور (`author`)، مەنبە (`source`) ۋە تەرجىمان (`translator`) ئۇچۇرلىرى ئىمكانقەدەر ئەسلى پېتى ساقلاپ قېلىندى.
- ئاساسلىق مەقسەت — ئۇيغۇر تىلىنىڭ سۈنئىي ئىدراك ۋە ماشىنا تىلى تەتقىقاتىدىكى سانلىق مەلۇمات ئېھتىياجىنى قامداشقا كۈچ قوشۇش.

---

### 📂 سانلىق مەلۇمات قۇرۇلمىسى / Schema

| ئىستون / Column | تىپى / Type | مەزمۇنى / Description |
| :--- | :--- | :--- |
| **`title`** | `string` | ماۋزۇ ياكى تېما نامى |
| **`text`** | `string` | بىر تەرەپ قىلىنغان ئاساسلىق تېكىست |
| **`author`** | `string` | ئەسەرنىڭ ئاپتورى (ئەگەر بار بولسا) |
| **`source`** | `string` | ئەسەر ئېلىنغان تور بەت ياكى مەنبە |
| **`date`** | `string` | يېزىلغان ياكى ئېلان قىلىنغان ۋاقتى |
| **`translator`** | `string` | تەرجىمانى (ئەگەر بار بولسا) |

---

### 🚀 تېز ئىشلىتىش / Quick Start

#### Hugging Face Datasets
```python
from datasets import load_dataset

dataset = load_dataset("Uyghur-Corpus/Uyghur-Corpus")
print(dataset["train"][0])
