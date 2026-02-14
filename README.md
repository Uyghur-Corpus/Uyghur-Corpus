---
license: mit
task_categories:
- text-generation
- text-classification
language:
- ug
tags:
- uyghur
- uighur
- nlp
- llm
- socio-political
- history
- literature
pretty_name: Uyghur Socio-Political & Literary Dataset
dataset_info:
  features:
  - name: title
    dtype: string
  - name: author
    dtype: string
  - name: date
    dtype: string
  - name: tags
    sequence: string
  - name: content
    dtype: string
  - name: language
    dtype: string
  - name: source
    dtype: string
  - name: sections
    list:
    - name: content
      dtype: string
    - name: tags
      sequence: string
    - name: title
      dtype: string
  config_name: default
---

# Uyghur Large-Scale Text Corpus for AI & LLM Training
### سۈنئىي ئىدراك ۋە چوڭ تىل مودېللىرى ئۈچۈن ئۇيغۇرچە تىل ئامبىرى

![Status](https://img.shields.io/badge/Status-Actively%20Maintained-success) ![Language](https://img.shields.io/badge/Language-Uyghur-blue) ![License](https://img.shields.io/badge/License-MIT-green) ![AI Ready](https://img.shields.io/badge/AI-LLM%20Ready-orange)

## 📖 Dataset Description / ئامبار ھەققىدە چۈشەندۈرۈش

This repository hosts a **comprehensive and actively maintained** dataset of the Uyghur language (Ug), designed specifically to train **Large Language Models (LLMs)**, **Machine Translation systems**, and **NLP tools**. 

The dataset aggregates high-quality texts from socio-political, literary, historical, and general domains to solve the "low-resource" problem for the Uyghur language in Artificial Intelligence.

بۇ ئامبار ئۇيغۇر تىلىدىكى **سۈنئىي ئىدراك (AI)**، **چوڭ تىل مودېللىرى (LLM)** ۋە **تەرجىمە ماشىنىلىرىنى** مەشىق قىلدۇرۇش ئۈچۈن مەخسۇس قۇرۇلغان، داۋاملىق يېڭىلىنىپ تۇرىدىغان ئۇنىۋېرسال سانلىق مەلۇمات ئامبىرىدۇر. بۇ ئامبار سىياسىي، ئىجتىمائىي، تارىخىي ۋە ئەدەبىي تېمىلارنى ئۆز ئىچىگە ئالىدۇ.

## 📊 Real-Time Statistics / سانلىق مەلۇمات ئەھۋالى

**Note:** This dataset is dynamic. The number of articles and total size grows regularly.
**ئەسكەرتىش:** بۇ ئامبار داۋاملىق چوڭىيىۋاتىدۇ.

> **Please refer to the file list or Hugging Face Dataset Viewer for the exact, real-time row count and data size.**
> **ئېنىق ماقالە سانى ۋە ھەجىمىنى كۆرۈش ئۈچۈن، ھۆججەت تىزىملىكىگە ياكى Hugging Face نىڭ كۆرۈش كۆزنىكىگە قاراڭ.**

## 📂 Data Structure / قۇرۇلمىسى

The dataset follows the industry-standard `JSONL` format, optimized for direct ingestion by training frameworks like PyTorch, TensorFlow, and Hugging Face Transformers.
مەلۇماتلار خەلقئارالىق ئۆلچەم `JSONL` فورماتىدا ساقلانغان بولۇپ، مودېللار بىۋاسىتە ئوقۇيالايدۇ.

**Schema:**
{
  "title": "Article Title / ماقالە ماۋزۇسى",
  "author": "Author Name / ئاپتور",
  "date": "Publication Date / ۋاقتى",
  "tags": ["Topic1", "Topic2"],
  "content": "Full text in Markdown... / تولۇق تېكىست"
  "language": "ug",
   "sections": [{"title": "تارماق ماۋزۇ", "content": "بۆلەك مەزمۇنى", "tags": []}]
}
