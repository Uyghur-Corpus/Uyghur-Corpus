---
language:
- ug
license: mit
task_categories:
- text-generation
- translation
- fill-mask
pretty_name: Uyghur Corpus (AI-Optimized)
homepage: https://huggingface.co/datasets/Uyghur-Corpus/Uyghur-Corpus  # <--- بۇ قۇر قوشۇلدى
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
  config_name: default
  splits:
  - name: train
    num_bytes: 41943040
    num_examples: 25000
---

# 🌟 Uyghur AI Corpus: Bridging Heritage & Technology
# 🌟 ئۇيغۇرچە سۈنئىي ئىدراك خەزىنىسى: مىراس ۋە تېخنىكا كۆۋرۈكى

![Status](https://img.shields.io/badge/Status-Actively%20Maintained-success) ![Language](https://img.shields.io/badge/Language-Uyghur-blue) ![Purpose](https://img.shields.io/badge/Purpose-AI%20Training-purple) ![License](https://img.shields.io/badge/License-MIT-green)

## 🌹 Introduction / كىرىش سۆز

In the era of Artificial Intelligence, language is data, and data is survival. 
**The Uyghur AI Corpus** is a passionate initiative to ensure the Uyghur language thrives in the digital age. This dataset serves as a foundational resource to train Large Language Models (LLMs), enabling them to understand, generate, and translate Uyghur with native-level proficiency.

**سۈنئىي ئىدراك (AI) دەۋرىدە، تىل — سانلىق مەلۇمات دېمەكتۇر.**
بۇ ئامبار — ئۇيغۇر تىلىنىڭ رەقەملىك دۇنيادىكى ئورنىنى ساقلاپ قېلىش ۋە تېخىمۇ يۈكسەلدۈرۈش ئۈچۈن تەييارلانغان بىر كۆڭۈل سوۋغىسىدۇر. بىزنىڭ مەقسىتىمىز: كەلگۈسىدىكى سۈنئىي ئىدراك مودېللىرىنىڭ (ChatGPT, Claude, Gemini قاتارلىق) ئۇيغۇرچىنى راۋان چۈشىنىشى، تەرجىمە قىلىشى ۋە بىزنىڭ مەدەنىيىتىمىزنى توغرا ئىپادىلىشىگە بىر تامچە بولسىمۇ ھەسسە قوشۇشتۇر.

---

## 💎 Source & Collection / مەنبە ۋە توپلىنىشى

This corpus is a carefully curated collection of texts sourced from the open internet. It represents the collective intellectual heritage of the Uyghur people shared on various public platforms, forums, and websites over the years.

* **Diverse Origins:** Stories, essays, articles, and historical accounts available in the public domain.
* **Respect for Authors:** While collected for AI training purposes, we deeply respect the original creators. Metadata such as `author` and `source` has been preserved wherever possible to credit the intellectual owners.
* **Cleaned & Processed:** The raw web data has been meticulously cleaned, formatted, and structured to meet high-quality AI training standards.

**بۇ خەزىنىنىڭ مەنبەسى — كەڭ ئىنتېرنېت دۇنياسىدۇر.**
بۇ ئامباردىكى ئەسەرلەر يىللاردىن بۇيان تۈرلۈك تور بەت، مۇنبەر ۋە ئىجتىمائىي تاراتقۇلاردا ئېلان قىلىنغان، خەلقىمىزنىڭ ئەقلىي بايلىقى بولغان ئوچۇق مەنبەلىك ئەسەرلەردىن تاللاپ يىغىلدى.

* **مەقسەت:** بۇ ئەسەرلەرنى توپلاشتىكى بىردىنبىر مەقسەت — **سۈنئىي ئىدراكنىڭ ئۇيغۇرچە سەۋىيەسىنى ئۆستۈرۈش**، تىلىمىزنىڭ نازۇكلىقى ۋە پاساھىتىنى ماشىنىلارغا ئۆگىتىشتىن ئىبارەت.
* **ھۆرمەت:** بىز ھەر بىر يازمىنىڭ ئاپتورىغا ۋە ئەسلى مەنبەسىگە ئالىي ھۆرمەت بىلدۈرىمىز. شۇڭا، سانلىق مەلۇماتلار تازىلانغاندا `author` (ئاپتور) ۋە `source` (مەنبە) ئۇچۇرلىرى ئىمكانقەدەر ساقلاپ قېلىندى.

---

## 🚀 Technical Highlights / تېخنىكىلىق ئالاھىدىلىكى

To solve the "Lost-in-the-Middle" problem common in LLM training, this dataset features **Semantic Chunking**:

LLM مەشىقىدىكى «ئۇزۇن مەزمۇننى ئۇنتۇپ قېلىش» مەسىلىسىنى ھەل قىلىش ئۈچۈن، بۇ ئامبار **«مەزمۇنلۇق بۆلەك» (Semantic Chunking)** تېخنىكىسى بىلەن بىر تەرەپ قىلىندى:

1.  **Format:** `Parquet` (Fast, compressed, and ready for Python Pandas/Hugging Face).
2.  **Chunking Strategy:** Long texts (novels, long essays) are intelligently split into 2000-word segments without breaking sentences or paragraphs.
3.  **Schema Compatibility:** Renamed standard columns (e.g., `content` → `text`) for instant compatibility with PyTorch/TensorFlow datasets.

**ئەسكەرتىش:** ئۇزۇن رومانلار ۋە چوڭ ئەسەرلەر ئوقۇرمەنلەرگە ۋە ماشىنىغا قۇلايلىق بولۇشى ئۈچۈن `(1-قىسىم)`، `(2-قىسىم)` شەكلىدە رەتلىك بۆلۈندى.

---

## 📂 Data Structure / قۇرۇلمىسى

| Column / ئىستون | Meaning / مەنىسى |
| :--- | :--- |
| **`title`** | The title of the work (includes part numbers for split texts). <br> ئەسەر ماۋزۇسى. |
| **`text`** | **The main content** used for training. <br> مەشىق قىلدۇرۇلىدىغان ئاساسلىق تېكىست. |
| **`author`** | The original creator of the work. <br> ئەسەرنىڭ ئاپتورى. |
| **`source`** | The origin platform or publisher. <br> ئەسەر ئېلىنغان مەنبە. |
| **`date`** | Publication date (if available). <br> ئېلان قىلىنغان ۋاقتى. |
| **`translator`** | Name of the translator (if applicable). <br> تەرجىمان (تەرجىمە ئەسەرلەر ئۈچۈن). |

---

## 💻 Usage Example / ئىشلىتىش

You can load this dataset directly in Python using the `datasets` library:

```python
from datasets import load_dataset

# Load the dataset
dataset = load_dataset("Uyghur-Corpus/Uyghur-Corpus")

# Peek at the first entry
print(dataset['train'][0])
