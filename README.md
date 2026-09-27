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
  - uyghur-language
  - parquet
  - text-corpus
  - poetry
  - literature
  - ghazal
  - rubaiyat
  - folk-poetry
  - turkic-languages
  - low-resource-nlp
  - machine-translation
  - language-modeling
  - ocr
  - uyghur-ocr
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
configs:
  - config_name: default
    data_files:
      - split: train
        path: "data/train-*.parquet"
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
[![GitHub](https://img.shields.io/badge/GitHub-Uyghur--Corpus-black)](https://github.com/Uyghur-Corpus/Uyghur-Corpus)

<!-- ئاپتوماتىك يېڭىلىنىدىغان قوش تىللىق بەلگىلەر -->
[![Last Update](https://img.shields.io/github/last-commit/Uyghur-Corpus/Uyghur-Corpus?label=Last%20Update%20%7C%20يېڭىلانغان%20ۋاقتى&color=blue)](https://github.com/Uyghur-Corpus/Uyghur-Corpus/commits/main)
[![Total Size](https://img.shields.io/github/repo-size/Uyghur-Corpus/Uyghur-Corpus?label=Total%20Size%20%7C%20ئومۇمىي%20ھەجىمى&color=orange)](https://github.com/Uyghur-Corpus/Uyghur-Corpus)

---

## 📑 مۇندەرىجە / Table of Contents

* [📖 چۈشەندۈرۈش / Overview](#-چۈشەندۈرۈش--overview)
* [📊 ئاساسىي ئۇچۇرلار / Dataset Information](#-ئاساسىي-ئۇچۇرلار--dataset-information)
* [📚 مەزمۇن دائىرىسى / Content](#-مەزمۇن-دائىرىسى--content)
* [💎 مەنبە ۋە ھۆرمەت / Sources & Attribution](#-مەنبە-ۋە-ھۆرمەت--sources--attribution)
* [📂 سانلىق مەلۇمات قۇرۇلمىسى / Schema](#-سانلىق-مەلۇمات-قۇرۇلمىسى--schema)
* [🚀 تېز ئىشلىتىش / Quick Start](#-تېز-ئىشلىتىش--quick-start)
* [🎯 ئىشلىتىش دائىرىسى / Intended Uses](#-ئىشلىتىش-دائىرىسى--intended-uses)
* [⚠️ چەكلىمىلەر / Limitations](#️-چەكلىمىلەر--limitations)
* [🛡️ ئەخلاقىي ئەسكەرتىش / Ethical Considerations](#️-ئەخلاقىي-ئەسكەرتىش--ethical-considerations)
* [📝 نەقىل كۆرسىتىش / Citation](#-نەقىل-كۆرسىتىش--citation)
* [⚖️ ئىجازەت ۋە نەشر ھوقۇقى / License & Copyright](#️-ئىجازەت-ۋە-نەشر-ھوقۇقى--license--copyright)
* [🌐 ئۇلانمىلار / Links](#-ئۇلانمىلار--links)

---

## 📖 چۈشەندۈرۈش / Overview

### ئۇيغۇرچە
**Uyghur AI Corpus** — ئۇيغۇر تىلىدىكى تېكىست، ئەدەبىيات ۋە تارىخىي-مەدەنىي مەزمۇنلارنى بىر يەرگە جەم قىلغان ئوچۇق سانلىق مەلۇمات خەزىنىسى. بۇ خەزىنە سۈنئىي ئىدراك، چوڭ تىل مودېللىرى (LLM)، تەبىئىي تىل بىر تەرەپ قىلىش (NLP)، ماشىنىلىق تەرجىمە ۋە كومپيۇتېرلىق تىلشۇناسلىق تەتقىقاتى ئۈچۈن مەخسۇس يىغىلىپ تازىلانغان.

### English
**Uyghur AI Corpus** is an open-source, cleaned Uyghur-language text and literature corpus designed for natural language processing, language modeling, machine translation, and computational linguistics. It is intended to support research and development for low-resource Uyghur NLP and AI.

---

## 📊 ئاساسىي ئۇچۇرلار / Dataset Information

| كۆرسەتكۈچ / Field | تەپسىلاتى / Details |
| :--- | :--- |
| **Language** | ئۇيغۇرچە / Uyghur (`ug` / `uig` / ISO 639-3) |
| **Script** | Uyghur Perso-Arabic script |
| **Format** | Apache Parquet (ئىخچام ۋە تېز بىر تەرەپ قىلىنىدۇ) |
| **Tasks** | Text generation, fill-mask, NLP |
| **Domain** | Literature, poetry, prose, articles, archives |
| **License** | MIT for repository/data structure; see License & Copyright |

> **ئەسكەرتىش:** Dataset نىڭ ئەمەلىي قۇر سانى ۋە ھۆججەت ھەجىمى سىز يېڭى سانلىق مەلۇمات قوشقاندا Hugging Face سىستېمىسى تەرىپىدىن ئاپتوماتىك ھېسابلىنىپ كۆرسىتىلىدۇ.

---

## 📚 مەزمۇن دائىرىسى / Content

Corpus دا تۆۋەندىكىدەك مەزمۇنلار بار:
* 📜 كىلاسسىك ۋە ھازىرقى زامان ئۇيغۇر ئەدەبىياتى
* 🪶 شېئىر، غەزەل، رۇبائىي، قوشاق ۋە خەلق شېئىرلىرى
* 📚 نەسىر، ھېكايە ۋە ماقالىلەر
* 🗂️ ئوچۇق تور مەنبەلىرى ۋە ئارخىپلار
* 🔤 OCR ئارقىلىق ئېلىنغان ۋە كېيىن تۈزىتىلگەن تېكىستلەر

---

## 💎 مەنبە ۋە ھۆرمەت / Sources & Attribution

مەزمۇنلار ئوچۇق تور مەنبەلىرى، ئەدەبىي سەھىپىلەر ۋە باشقا ئاممىۋى ئېلان قىلىنغان مەنبەلەردىن توپلانغان.
ئەسلى ئاپتور ۋە مەنبەلەرنىڭ ئەجرىگە ھۆرمەت قىلىش يۈزىسىدىن، تېكىستلەردىكى `author` (ئاپتور)، `source` (مەنبە) ۋە `translator` (تەرجىمان) ئۇچۇرلىرى ئىمكانقەدەر ساقلىنىپ قېلىندى.

---

## 📂 سانلىق مەلۇمات قۇرۇلمىسى / Schema

| ئىستون / Column | تىپى / Type | مەزمۇنى / Description |
| :--- | :--- | :--- |
| **`title`** | `string` | ئەسەرنىڭ ماۋزۇسى ياكى تېما نامى / Title |
| **`text`** | `string` | بىر تەرەپ قىلىنغان ئاساسلىق تېكىست / Cleaned text |
| **`author`** | `string` | ئاپتور ياكى شائىر / Author or poet |
| **`source`** | `string` | ئەسەرنىڭ مەنبەسى ياكى تور بەت / Origin source |
| **`date`** | `string` | ئېلان قىلىنغان ياكى يېزىلغان ۋاقىت / Date |
| **`translator`** | `string` | تەرجىمانى (ئەگەر بار بولسا) / Translator |

---

## 🚀 تېز ئىشلىتىش / Quick Start

### 1. Hugging Face `datasets` بىلەن
```python
from datasets import load_dataset

dataset = load_dataset("Uyghur-Corpus/Uyghur-Corpus")
print(dataset["train"][0])

---


### 2. Pandas بىلەن Parquet ئوقۇش

```python
import pandas as pd

df = pd.read_parquet("hf://datasets/Uyghur-Corpus/Uyghur-Corpus/data/train-00000-of-00001.parquet")
print(df.head())

```

### 3. Streaming ھالەتتە ئىشلىتىش

```python
from datasets import load_dataset

dataset = load_dataset("Uyghur-Corpus/Uyghur-Corpus", streaming=True)
for example in dataset["train"]:
print(example["title"], "-", example["author"])
break

```

---

## 🎯 ئىشلىتىش دائىرىسى / Intended Uses

* ئۇيغۇرچە LLM ئالدىن تەربىيىلەش (Pretraining) ۋە Fine-tuning
* Text generation, Fill-mask ۋە تېكىست تولۇقلاش
* ماشىنىلىق تەرجىمە ۋە ئۇيغۇرچە NLP سىستېمىلىرى
* ئەدەبىيات، شېئىرىيەت تەھلىلى ۋە كومپيۇتېرلىق تىلشۇناسلىق
* OCR دىن كېيىنكى ئۇيغۇرچە تېكىست تۈزىتىش قوراللىرى قاتارلىقلار.

---

## ⚠️ چەكلىمىلەر / Limitations

1. مەنبەلەرنىڭ تىل ۋە ئىملا سۈپىتى بىر-بىرىدىن پەرقلىنىشى مۇمكىن.
2. بەزى تېكىستلەردە كۆزدىن قېچىپ قالغان OCR خاتالىقلىرى ياكى خاتا ھەرپلەر بولۇشى مۇمكىن.
3. تارىخىي ۋە زامانىۋى ئۇيغۇرچە، شۇنداقلا رايونلۇق تىل پەرقلىرى سەۋەبلىك لۇغەت ۋە ئىملا پەرقى كۆرۈلۈشى مۇمكىن.
4. Dataset نى ئۇيغۇر تىلىنىڭ %100 تولۇق ۋەكىللىك ئەۋرىشكىسى دەپ قاراشقا بولمايدۇ.

---

## 🛡️ ئەخلاقىي ئەسكەرتىش / Ethical Considerations

بۇ خەزىنە ئاممىۋى ھالەتتە ئېلان قىلىنغان مەزمۇنلارنى جەم قىلىدۇ. تېكىستلەرنى تازىلاش جەريانىدا شەخسىي ئۇچۇرلارنى (PII) ئازايتىشقا تىرىشىلغان بولسىمۇ، **مۇتلەق تازىلانغانلىقىغا كاپالەت بېرىلمەيدۇ**. ئەگەر شەخسىي ياكى سەزگۈر ئۇچۇر بايقالسا، Issue ئارقىلىق مەلۇم قىلىشىڭىزنى سورايمىز.

بۇ Dataset نى سودا ياكى باشقا ئىشلارغا ئىشلەتكۈچىلەر مەزمۇننىڭ نەشر ھوقۇقى ۋە ئىشلىتىش شەرتلىرىنى ئايرىم تەكشۈرۈپ كۆرۈشى كېرەك.

---

## 📝 نەقىل كۆرسىتىش / Citation

ئەگەر بۇ خەزىنىنى تەتقىقاتىڭىزدا ئىشلەتسىڭىز، تۆۋەندىكىدەك نەقىل كۆرسىتىشىڭىزنى ئۆتۈنىمىز:

```bibtex
@misc{uyghur_ai_corpus,
title = {Uyghur AI Corpus},
author = {Uyghur-Corpus Contributors},
year = {2026},
publisher = {Hugging Face},
url = {[https://huggingface.co/datasets/Uyghur-Corpus/Uyghur-Corpus](https://huggingface.co/datasets/Uyghur-Corpus/Uyghur-Corpus)},
note = {Uyghur text and literature corpus for NLP, language modeling, and computational linguistics}
}

```

---


## ⚖️ ئىجازەت ۋە نەشر ھوقۇقى / License & Copyright

**مۇھىم:** Repository كودى، Dataset قۇرۇلمىسى ۋە پىروگرامما ھۆججەتلىرى **MIT License** ئاستىدا تارقىتىلىدۇ.

لېكىن Dataset ئىچىدىكى ئەسلى ئەدەبىي ۋە باشقا تېكىستلەرنىڭ نەشر ھوقۇقى ئاپتور، نەشر قىلغۇچى ياكى ئەسلى مەزمۇن ئىگىلىرىگە تەۋە بولۇشى مۇمكىن. شۇڭلاشقا **MIT License نى Dataset ئىچىدىكى بارلىق ئەسلى ئەدەبىي ئەسەرلەرنىڭ نەشر ھوقۇقىغا ئاپتوماتىك كېڭەيتىپ قاراشقا بولمايدۇ.**

---

## 🌐 ئۇلانمىلار / Links

* 🤗 **Hugging Face Dataset:** [https://huggingface.co/datasets/Uyghur-Corpus/Uyghur-Corpus](https://huggingface.co/datasets/Uyghur-Corpus/Uyghur-Corpus?utm_source=gemini)
* 💻 **GitHub Repository:** [https://github.com/Uyghur-Corpus/Uyghur-Corpus](https://github.com/Uyghur-Corpus/Uyghur-Corpus?utm_source=gemini)

> **📌 Project Goal:** More Uyghur data. Better Uyghur AI.
> **كۆپ ئۇيغۇرچە سانلىق مەلۇمات — تېخىمۇ ياخشى ئۇيغۇرچە سۈنئىي ئىدراك.**
