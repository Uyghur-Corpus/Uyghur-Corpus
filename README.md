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
- political-critique
- history
---


# Uyghur Socio-Political and Literary Dataset (109 Articles)
### ئۇيغۇر ئىجتىمائىي-سىياسىي ۋە ئەدەبىي ماقالىلەر سانلىق مەلۇمات توپلىمى

This repository contains a curated dataset of **109 Uyghur articles**. The dataset is provided in **JSONL** format, making it ideal for Natural Language Processing (NLP) and AI research.

بۇ ئامباردا جەمئىي **109 پارچە** ماقالە جەملەندى. سۈنئىي ئىدراك مودېللىرىنى مەشىق قىلدۇرۇش ۋە تىل تەتقىقاتى ئۈچۈن **JSONL** فورماتىدا تەييارلاندى.

---

## 📋 Dataset Overview / ئومۇمىي ئەھۋال
* **Total Articles:** 109
* **Format:** `.jsonl` (UTF-8)
* **Authors:** Burhan Muhammed, Enwer Haji Muhammed (Erturk), etc.

---

## 🚀 How to Use / ئىشلىتىش ئۇسۇلى
You can load this dataset in Python:
```python
import json
with open('Uyghur_Dataset_Final.jsonl', 'r', encoding='utf-8') as f:
    for line in f:
        data = json.loads(line)
        print(data['title'])
