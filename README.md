# Principal-Parts-Detection

This repository contains the multilingual dataset introduced in the paper:  
📄 [*Principal Parts Detection for Computational Morphology: Task, Models and Benchmark* (CoNLL 2025)](https://aclanthology.org/2025.conll-1.17/)

---

## 📚 Overview

**Principal parts** are the minimal subset of cells in an inflectional paradigm from which all other forms can be deterministically deduced. While foundational in linguistic theory, they have been largely overlooked in computational morphology.

We formalize **Principal Parts Detection** as a computational task under the static principal-parts scheme:

> Given a collection of inflection tables for a syntactic category, identify a single, minimal set of cells that uniformly serve as principal parts across all lexemes.

This dataset provides a standardized benchmark for evaluating computational models on this task.

---

## 🌍 Dataset Description

The dataset covers **verbal inflection tables** and **gold principal parts** for ten typologically diverse languages:

- Hebrew
- English
- French
- German
- Spanish
- Danish
- Swedish
- Finnish
- Turkish
- Latin
  
Each subdirectory under [`data/`](./data/) includes:
- `inflection_data.txt`: cleaned inflection tables derived from UniMorph 4.0, with normalization and error correction applied for consistency and accuracy (see paper for details)
- `gold_principal_parts.json`: manually curated principal parts for that language

The dataset preparation involved rigorous normalization and error correction. Only strictly inflectional forms are retained, with exactly one form per feature set. Inconsistent or marginal feature sets were removed to ensure dataset reliability.

---

## 🔍 Purpose

This dataset supports research in computational morphology and the study of implicative structure in inflectional paradigms. It provides a reliable empirical foundation for modeling principal parts in a cross-linguistic setting.

---

## 📄 Citation

If you use this dataset, please cite:

> Dorin Keshales, Omer Goldman, and Reut Tsarfaty. 2025.  
> *Principal Parts Detection for Computational Morphology: Task, Models and Benchmark.*  
> In *Proceedings of the 29th Conference on Computational Natural Language Learning (CoNLL)*, pages 251–267, Vienna, Austria. Association for Computational Linguistics.  
> [https://aclanthology.org/2025.conll-1.17](https://aclanthology.org/2025.conll-1.17)

*(Note: an updated version will be made available on arXiv.)*

---

## 📝 License

This dataset is released under the [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/) license.

It incorporates data derived from [UniMorph 4.0](https://unimorph.github.io/), which is also licensed under CC BY-SA 4.0.  
By using this dataset, you agree to comply with the terms of this license.

See the [LICENSE](./LICENSE) file for full details.
