# Uyghur Corpus (Uyghurche Til Ambiri)

![Status](https://img.shields.io/badge/Status-Active_&_Expanding-brightgreen?style=for-the-badge)
![Language](https://img.shields.io/badge/Language-Uyghur-blue?style=for-the-badge)
![Data Type](https://img.shields.io/badge/Data_Type-Text_/_Essays-green?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-orange?style=for-the-badge)

## 📖 Introduction (تونۇشتۇرۇش)

**Uyghur Corpus** is a growing, living archive of high-quality Uyghur language texts, specifically designed for **Natural Language Processing (NLP)**, **Machine Learning (ML)** training, and **Linguistic Research**.

**⚠️ Note:** This repository is **actively maintained and updated**. New articles, essays, and literary works are being uploaded regularly to expand the dataset.

This repository serves as a critical resource for low-resource language preservation, focusing on:
* **Political & Social Commentary:** Deep essays reflecting the contemporary Uyghur psyche.
* **Literary & Philosophical Works:** Preserving the intellectual heritage of the Uyghur people.
* **Structured Metadata:** Each file includes a YAML header (title, author, topics) for automated parsing.
* **Clean Format:** All texts are stored in Markdown (`.md`) format to ensure readability for both humans and machines.

---

## 📂 Dataset Structure (ماتېرىيال قۇرۇلمىسى)

The corpus is organized to be machine-readable. As new texts are added, they will appear in the `Articles/` folder.

```text
Uyghur-Corpus/
│
├── Articles/                  # Main content folder (Growing collection)
│   ├── Burhan_Binnormalliq_2019.md       # Essay on Social Abnormality
│   ├── Burhan_Uyghurluq_Rohi.md          # Essay on Uyghur Spirit
│   ├── Burhan_Wijdan_We_Mahbusluq.md     # Essay on Conscience & Prison
│   ├── ... (More files added regularly)
│   └── ...
│
└── README.md                  # Documentation (You are here)


import os
import frontmatter  # pip install python-frontmatter

def load_uyghur_corpus(data_dir="Articles"):
    corpus = []
    # Automatically iterate through all files in the directory
    for filename in os.listdir(data_dir):
        if filename.endswith(".md"):
            filepath = os.path.join(data_dir, filename)
            try:
                # Load file and metadata
                post = frontmatter.load(filepath)
                entry = {
                    "filename": filename,
                    "title": post.get("title"),
                    "author": post.get("author"),
                    "topics": post.get("topics"),
                    "content": post.content
                }
                corpus.append(entry)
            except Exception as e:
                print(f"Error loading {filename}: {e}")
                
    return corpus

# Usage
data = load_uyghur_corpus()
print(f"Successfully loaded {len(data)} documents from the archive.")



---
title: "Article Title"
author: "Author Name"
date: "YYYY-MM-DD"
genre: "Category (e.g., Politics, History)"
topics: ["Topic1", "Topic2"]
language: "ug"
---

[Full Text Content Here...]


@misc{uyghur-corpus,
  author = {Uyghur Archive Team},
  title = {Uyghur Corpus: High-Quality Texts for NLP},
  year = {2026},
  publisher = {GitHub},
  journal = {GitHub repository},
  note = {Active and Expanding Archive},
  howpublished = {\url{[https://github.com/Uyghur-Archive/Uyghur-Corpus](https://github.com/Uyghur-Archive/Uyghur-Corpus)}}
}
