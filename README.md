# SuperSem

Repository for the superlatives dataset from the NAACL 2025 paper: **Superlatives in Context: Modeling the Implicit Semantics of Superlatives**

## Paper Information
**Authors:** Valentina Pyatkin, Bonnie Webber, Ido Dagan, Reut Tsarfaty  
**Conference:** North American Chapter of the Association for Computational Linguistics (NAACL) 2025  
**Year:** 2025

## Overview
This repository contains the SuperSem dataset, a collection of superlative expressions annotated with their implicit semantic properties in context. The dataset was introduced in our NAACL 2025 paper "Superlatives in Context: Modeling the Implicit Semantics of Superlatives."

## Dataset
The SuperSem dataset includes: the full file, called supersem_full.tsv, the train split, called supersem_train.tsv, the test split, supersem_test.tsv, and the dev split, supersem_dev.tsv.

The dataset is provided in TSV format with the following columns:

| Column | Description |
|--------|-------------|
| `ID` | Unique identifier for each sentence |
| `source` | Source domain or corpus of the original text |
| `context` | The surrounding paragraph or discourse context |
| `sentence` |  The full sentence containing the superlative expression |
| `sup_idx_sent` | Index position of the superlative within the sentence  |
| `sup_idx_context` | Index position of the superlative within the context |
| `title` | Title of the article or document (if applicable) |
| `sup_class` | Classification of the superlative type (only for instances from Wikipedia, source of the classes is Silke et al. 2009) |
| `superlative` |The extracted superlative expression |
| `turn_idx (only for dialogue)` |  Turn index in dialogue (only for dialogue-based examples) |
| `target` | The entity that is being described by the superlative |
| `CS` | Comparison Set - the group of entities being compared  |
| `Anchor` | Reference point or entity for the comparison |
| `Property` | The property or dimension along which entities are compared |
| `Orientation` | Whether the superlative indicates maximum or minimum value|
| `Implicit` | Binary annotation indicating if there are implicit elements  |
| `Amount` | Quantity information related to the superlative (if applicable) |
| `Rank` |  Ranking position indicated by the superlative (if applicable) |

**Note:** Fields marked with `-`, or empty fields, indicate that the specific instance is not a superlative expression (but syntactically tagged as one).


## Citation
If you use this dataset in your research, please cite our paper:

```bibtex
@inproceedings{pyatkin2025superlatives,
  title     = {Superlatives in Context: Modeling the Implicit Semantics of Superlatives},
  author    = {Pyatkin, Valentina and Webber, Bonnie and Dagan, Ido and Tsarfaty, Reut},
  booktitle = {Proceedings of the 2025 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies},
  year      = {2025},
  publisher = {Association for Computational Linguistics}
}
```

## License
The SuperSem dataset is released under the Creative Commons Attribution 4.0 International License (CC BY 4.0).
You are free to:

Share — copy and redistribute the material in any medium or format
Adapt — remix, transform, and build upon the material for any purpose, even commercially

Under the following terms:

Attribution — You must give appropriate credit and citation, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
