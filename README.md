---
language:
  - ug
license: mit
task_categories:
  - text-generation
  - translation
  - fill-mask
pretty_name: Uyghur Corpus (AI-Optimized)
homepage: https://huggingface.co/datasets/Uyghur-Corpus/Uyghur-Corpus
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

---
language:
  - ug
license: mit
task_categories:
  - text-generation
  - translation
  - fill-mask
pretty_name: Uyghur Corpus (AI-Optimized)
homepage: https://huggingface.co/datasets/Uyghur-Corpus/Uyghur-Corpus
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

# 🌟 Uyghur AI Corpus: Bridging Heritage & Technology
# 🌟 ئۇيغۇرچە سۈنئىي ئىدراك خەزىنىسى: مىراس ۋە تېخنىكا كۆۋرۈكى

![Status](https://img.shields.io/badge/Status-Actively%20Maintained-success) ![Language](https://img.shields.io/badge/Language-Uyghur-blue) ![Purpose](https://img.shields.io/badge/Purpose-AI%20Training-purple) ![License](https://img.shields.io/badge/License-MIT-green)

## 🌹 Introduction / كىرىش سۆز

In the era of Artificial Intelligence, language is data, and data is survival. 
**The Uyghur AI Corpus** is an initiative to ensure the Uyghur language thrives in the digital age. This dataset serves as a foundational resource to train Large Language Models (LLMs), enabling them to understand, generate, and translate Uyghur with native-level proficiency.

**سۈنئىي ئىدراك (AI) دەۋرىدە، تىل — سانلىق مەلۇمات دېمەكتۇر.**
بۇ ئامبار — ئۇيغۇر تىلىنىڭ رەقەملىك دۇنيادىكى ئورنىنى ساقلاپ قېلىش ۋە تېخىمۇ يۈكسەلدۈرۈش ئۈچۈن تەييارلانغان بىر كۆڭۈل سوۋغىسىدۇر. بىزنىڭ مەقسىتىمىز: كەلگۈسىدىكى سۈنئىي ئىدراك مودېللىرىنىڭ ئۇيغۇرچىنى راۋان چۈشىنىشى، تەرجىمە قىلىشى ۋە بىزنىڭ مەدەنىيىتىمىزنى توغرا ئىپادىلىشىگە ھەسسە قوشۇشتۇر.

---

## 🆕 What's New (Feb 2026 Update) / يېڭىلىنىشلار

- **Content Update:** Added new Uyghur articles and poetry to the dataset.
- **مەزمۇن يېڭىلاندى:** ئامبارغا يېڭىدىن نۇرغۇن ماقالىلەر ۋە شېئىرلار قوشۇلدى.

---

## 💎 Source & Collection / مەنبە ۋە توپلىنىشى

This corpus is a carefully curated collection of texts sourced from the open internet. Metadata such as `author` and `source` has been preserved wherever possible to credit the intellectual owners.

**بۇ خەزىنىنىڭ مەنبەسى — كەڭ ئىنتېرنېت دۇنياسىدۇر.**
بۇ ئامباردىكى ئەسەرلەر يىللاردىن بۇيان تور بەت، مۇنبەر ۋە ئىجتىمائىي تاراتقۇلاردا ئېلان قىلىنغان، خەلقىمىزنىڭ ئەقلىي بايلىقى بولغان ئوچۇق مەنبەلىك ئەسەرلەردىن تاللاپ يىغىلدى.

* **Diversity:** Stories, essays, articles, and historical accounts.
* **Respect:** Metadata is preserved to credit original authors.
* **مەقسەت:** سۈنئىي ئىدراكنىڭ ئۇيغۇرچە سەۋىيەسىنى ئۆستۈرۈش.
* **ھۆرمەت:** ئاپتور ۋە مەنبە ئۇچۇرلىرى ئىمكانقەدەر ساقلاپ قېلىندى.

---

## 🚀 Technical Highlights / تېخنىكىلىق ئالاھىدىلىكى

To solve the "Lost-in-the-Middle" problem common in LLM training, this dataset features **Semantic Chunking**:



1. **Format:** `Parquet` (Fast, compressed, and ready for Python Pandas/Hugging Face).
2. **Chunking Strategy:** Long texts are intelligently split into 2000-word segments without breaking sentences.
3. **Compatibility:** Standardized columns for instant use with PyTorch/TensorFlow datasets.

---

## 📂 Data Structure / قۇرۇلمىسى

| Column / ئىستون | Meaning / مەنىسى |
| :--- | :--- |
| **`title`** | The title of the work. / ئەسەر ماۋزۇسى. |
| **`text`** | **The main content** used for training. / ئاساسلىق تېكىست. |
| **`author`** | The original creator. / ئەسەرنىڭ ئاپتورى. |
| **`source`** | The origin platform. / ئەسەر ئېلىنغان مەنبە. |
| **`date`** | Publication date. / ئېلان قىلىنغان ۋاقتى. |
| **`translator`** | Name of the translator. / تەرجىمان. |

---

## 💻 Usage Example / ئىشلىتىش ئۈلگىسى

You can load this dataset directly in Python using the `datasets` library:

```python
from datasets import load_dataset

# Load the dataset
dataset = load_dataset("Uyghur-Corpus/Uyghur-Corpus")

# Peek at the first entry
print(dataset['train'][0])
