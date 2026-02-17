---
language:
- ug
license: mit
task_categories:
- text-generation
- translation
- fill-mask
pretty_name: Uyghur Corpus (LLM Ready)
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

# Uyghur Large-Scale Text Corpus for AI & LLM Training
### سۈنئىي ئىدراك ۋە چوڭ تىل مودېللىرى ئۈچۈن ئۇيغۇرچە تىل ئامبىرى

![Status](https://img.shields.io/badge/Status-Actively%20Maintained-success) ![Language](https://img.shields.io/badge/Language-Uyghur-blue) ![License](https://img.shields.io/badge/License-MIT-green) ![AI Ready](https://img.shields.io/badge/AI-LLM%20Ready-orange)

## 📖 Dataset Description / ئامبار ھەققىدە چۈشەندۈرۈش

This repository hosts a **comprehensive and actively maintained** dataset of the Uyghur language (Ug), designed specifically to train **Large Language Models (LLMs)**, **Machine Translation systems**, and **NLP tools**. 

The dataset aggregates high-quality texts from socio-political, literary, historical, and general domains to solve the "low-resource" problem for the Uyghur language in Artificial Intelligence.

The data has been pre-processed, cleaned, and semantically chunked to ensure optimal performance for model training.

بۇ ئامبار ئۇيغۇر تىلىدىكى **سۈنئىي ئىدراك (AI)**، **چوڭ تىل مودېللىرى (LLM)** ۋە **تەرجىمە ماشىنىلىرىنى** مەشىق قىلدۇرۇش ئۈچۈن مەخسۇس قۇرۇلغان، داۋاملىق يېڭىلىنىپ تۇرىدىغان ئۇنىۋېرسال سانلىق مەلۇمات ئامبىرىدۇر. بۇ ئامبار سىياسىي، ئىجتىمائىي، تارىخىي ۋە ئەدەبىي تېمىلارنى ئۆز ئىچىگە ئالىدۇ.

بارلىق مەلۇماتلار تازىلانغان، رەتلەنگەن ۋە مودېللارغا ماسلىشىشى ئۈچۈن مەزمۇنلۇق بۆلەكلەرگە (Semantic Chunking) ئايرىلغان.

## 📊 Real-Time Statistics / سانلىق مەلۇمات ئەھۋالى

**Note:** This dataset is dynamic. The number of articles and total size grows regularly.
**ئەسكەرتىش:** بۇ ئامبار داۋاملىق چوڭىيىۋاتىدۇ.

> **Please refer to the file list or Hugging Face Dataset Viewer for the exact, real-time row count and data size.**
> **ئېنىق ماقالە سانى ۋە ھەجىمىنى كۆرۈش ئۈچۈن، ھۆججەت تىزىملىكىگە ياكى Hugging Face نىڭ كۆرۈش كۆزنىكىگە قاراڭ.**

## 📂 Data Structure / قۇرۇلمىسى

The dataset uses the optimized `Parquet` format, which is faster and smaller than JSONL but fully compatible with Pandas and Hugging Face datasets.
مەلۇماتلار ئەلالاشتۇرۇلغان `Parquet` فورماتىدا ساقلانغان. بۇ فورمات JSONL غا قارىغاندا تېز ۋە ئىخچام.

### Schema (ئىستونلارنىڭ مەنىسى):

| Field / ئىستون | Description / چۈشەندۈرۈش |
| :--- | :--- |
| **`title`** | The title of the article. Long articles are split into parts (e.g., "Title (1-قىسىم)"). <br> ماقالە ماۋزۇسى. ئۇزۇن ئەسەرلەر (1-قىسىم، 2-قىسىم) دەپ ئايرىلغان. |
| **`text`** | **The main content.** Renamed from 'content' to 'text' for standard LLM compatibility. <br> ئاساسلىق تېكىست مەزمۇنى. |
| **`author`** | Name of the author (if available). <br> ئاپتور (ئەگەر بار بولسا). |
| **`source`** | The origin of the text (website, book, or publisher). <br> مەنبە (تور بەت، كىتاب ياكى نەشرىيات). |
| **`date`** | Publication date (YYYY-MM-DD format). <br> ئېلان قىلىنغان ۋاقتى. |
| **`translator`** | Name of the translator (for translated works). <br> تەرجىمان (تەرجىمە ئەسەرلەر ئۈچۈن). |

### Example Row (مىسال):

```json
{
  "title": "قۇتادغۇبىلىك (1-قىسىم)",
  "text": "بۇ ۋاپاسىز دۇنيانىڭ قىلىقلىرىنى ئەقىل ئىشلىتىپ تەسەۋۋۇر قىلساڭ...",
  "author": "يۈسۈپ خاس ھاجىپ",
  "source": "قەدىمكى ئەسەرلەر",
  "date": "1069"
}
