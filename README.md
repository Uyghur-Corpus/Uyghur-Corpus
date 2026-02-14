---
license: mit
task_categories:
- text-generation
- text-classification
- translation
- token-classification
- question-answering
language:
- ug
tags:
- uyghur
- uighur
- nlp
- llm
- deep-learning
- low-resource-language
- corpus
- text-dataset
- central-asia
pretty_name: Uyghur Large-Scale Text Corpus
size_categories:
- 100M<n<1B
dataset_info:
  features:
  - name: text
    dtype: string
  - name: label
    dtype: string
  - name: source
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
```json
{
  "text": "Full article text content... / ماقالىنىڭ تولۇق تېكىستى...",
  "label": "Category (e.g., Politics, History, Literature) / تۈرى",
  "source": "Source Filename or URL / مەنبەسى"
}
