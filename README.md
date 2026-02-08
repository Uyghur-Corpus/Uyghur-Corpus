---
license: mit
language:
- ug
pretty_name: Uyghur Socio-Political Articles Dataset
size_categories:
- n<1k
task_categories:
- text-generation
- text-classification
tags:
- uyghur
- nlp
- dataset
- political-critique
- history
- llm-training
---

# Uyghur Socio-Political and Literary Dataset (109+ Articles)
### ئۇيغۇر ئىجتىمائىي-سىياسىي ۋە ئەدەبىي ماقالىلەر سانلىق مەلۇمات توپلىمى

This repository contains a curated dataset of **109+ Uyghur articles**. This is an **actively maintained** project, and new content is added regularly.

بۇ ئامباردا جەمئىي **109 پارچىدىن ئارتۇق** ماقالە جەملەندى. بۇ سانلىق مەلۇمات توپلىمى **ئاكتىپ يېڭىلىنىپ تۇرىدىغان تۈر** بولۇپ، يېڭى ماقالىلەر دائىملىق قوشۇلۇپ تۇرىدۇ.

## 🔄 Project Status / يېڭىلىنىش ئەھۋالى
* **Status:** Active / ئاكتىپ
* **Update Frequency:** Regular updates / دائىملىق يېڭىلىنىدۇ
* **Current Count:** 109 articles (As of Feb 2026)



## 📋 Dataset Overview / ئومۇمىي ئەھۋال
* **Format:** `.jsonl` (UTF-8)
* **Authors:** Burhan Muhammed, Enwer Haji Muhammed (Erturk), Karimjan Ghafuri, Mahmud Muhiti, Muhammad Amin Bughra, etc.

## 🛠 Usage Guide / تېخنىكىلىق قوللانما
Developers can integrate this dataset using the Hugging Face `datasets` library:

```python
from datasets import load_dataset

# Load the dataset
dataset = load_dataset("Uyghur-Corpus/Uyghur-Corpus")

# Access an article
print(dataset['train'][0]['content'])
