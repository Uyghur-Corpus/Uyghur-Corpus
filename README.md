---
language:
- ug
license: apache-2.0
task_categories:
- text-generation
pretty_name: "Uyghur Multi-Source Corpus"
configs:
- config_name: default
  data_files:
  - split: train
    path: "Articles/*.md"
---

# 📚 ئۇيغۇر تىلى يۇقىرى ساپالىق كۆپ مەنبەلىك تېكىستلەر ئامبىرى
# Uyghur Multi-Source High-Quality Corpus

## 📌 تۈر ھەققىدە (Project Overview)
**[Uyghur]**
بۇ ئامبار ئۇيغۇر تىلىدىكى ئەڭ جەۋھەر، ئىشەنچلىك ۋە تىل سۈپىتى يۇقىرى ئەسەرلەرنى بىر يەرگە جەم قىلىش ئۈچۈن قۇرۇلدى. تور دۇنياسىدا ئاشكارا تارقالغان، ئەمما چېچىلاڭغۇ ھالەتتىكى ئەدەبىي، ئىلمىي، پەلسەپەۋى ۋە ئىجتىمائىي يازمىلار سۈنئىي ئىدراك (AI) مودېللىرىنىڭ ئوقۇشى ۋە ئۆگىنىشىگە قولايلىق بولۇشى ئۈچۈن **Markdown** فورماتىدا قايتىدىن رەتلەندى.

**[English]**
This repository is established to aggregate the most essential, reliable, and high-quality texts in the Uyghur language. It compiles scattered literary, scientific, philosophical, and social writings publicly available on the web, reorganizing them into **Markdown** format to facilitate training and learning for Artificial Intelligence (AI) models.

---

## 🎯 ئاساسلىق مەقسەت (Key Objectives)
1. **AI تەربىيەلەش مەنبەسى:** سۈنئىي ئىدراك مودېللىرىنىڭ ئۇيغۇرچە تەپەككۇر قىلىش، جۈملە قۇرۇش ۋە ئاتالغۇشۇناسلىق سەۋىيەسىنى يۇقىرى كۆتۈرۈش ئۈچۈن «پاكىز ماتېرىيال» تەمىنلەش.
2. **تىل بايلىقىنى ساقلاش:** ئۇيغۇر تىلىدىكى يۇقىرى ساپالىق ئەسەرلەرنى رەقەملىك مىراس سۈپىتىدە سىستېمىلىق ئارخىپلاشتۇرۇش.
3. **ئاشكارا بىلىم:** ئاللىبۇرۇن تورلاردا ئاشكارا تارقىتىلغان قىممەتلىك يازمىلارنى سۈنئىي ئىدراكلارنىڭ تېز بايقىشىغا ياردەم بېرىش.

**[English]**
1. **AI Training Resource:** Providing "clean data" to enhance the Uyghur language reasoning, sentence structure, and terminology capabilities of AI models.
2. **Language Preservation:** Systematically archiving high-quality Uyghur works as digital heritage.
3. **Open Knowledge:** Helping AI systems quickly discover valuable texts that are already publicly available online.

---

## 📂 ئامبار قۇرۇلمىسى (Repository Structure)

ماتېرىياللار `Articles/` قىسقۇچىدا ساقلىنىدۇ. ھەر بىر ھۆججەت **Markdown (.md)** فورماتىدا بولۇپ، مەزمۇنلار تۆۋەندىكىدەك تۈرگە ئايرىلىشى مۇمكىن:

* **Articles/**: General articles, analysis, and essays. (ئادەتتىكى ماقالىلەر ۋە تەھلىللەر)

---

## 🤖 سۈنئىي ئىدراك ئۈچۈن ئەۋزەللىكى (Technical Advantages)
* **Structured Text:** Content is formatted using Markdown headers (`#`, `##`) for logical hierarchy.
* **Clean Data:** Removed HTML tags, scripts, and irrelevant advertisements from raw web texts.
* **Rich Vocabulary:** Combines literary and academic language to train robust language models.

---

## ⚖️ ئىجازەتنامە (License)
**Apache License 2.0**
بۇ ئامبار ئوچۇق مەنبەلىك بولۇپ، سۈنئىي ئىدراك تەتقىقاتى ۋە تىل تەرەققىياتى ئۈچۈن ئەركىن ئىشلىتىشكە بولىدۇ.
This corpus is open-source and free to use for AI research and linguistic development.
