# English-Amharic-Augmented-corpus
This repository provides an augmented English–Amharic parallel corpus, designed to improve machine translation performance for this low-resource language pair. The augmentation approach follows the methodology described in Biadgligne & Smaïli, 2022, and incorporates the following processes:
**1. Base Corpus Collection**
    * A parallel English–Amharic corpus was collected from web sources, news articles, and legal documents.
    * The raw sentences were preprocessed and cleaned to ensure high-quality alignment.

**2. Offline Corpus Augmentation**
    * Several augmentation operations were applied to the transliterated corpus:
        - Token-level insertion
        - Token-level replacement
        - Token-level deletion
        - Token-level swapping
    * Augmented sentences were filtered using semantic similarity metrics (cosine similarity) to ensure that each augmented sentence retained at least ~90% of the original semantic content.

**3. Augmented Corpus Assembly**
    * The original corpus and the validated augmented sentences were combined to form a larger, enriched training dataset.
    * Multiple versions of the augmented corpus were generated to explore different augmentation parameters (e.g., deletion probability, swapping range).
    
# Corpus Statistics
| Language | Original Sentences | Augmented Sentences | Total Sentences | Encoding |
| -------- | -----------------: | ------------------: | --------------: | -------- |
| English  |            225,304 |             225,304 |         450,608 | UTF-8    |
| Amharic  |            225,304 |             225,304 |         450,608| UTF-8     |



**BibTeX**

```bibtex
@inproceedings{biadgligne2022offline,
     title        = {Offline Corpus Augmentation for English-Amharic Machine Translation},
     author       = {Biadgligne, Yohannes and Sma{\"i}li, Kamel},
     booktitle    = {ICICT CPS Conference Proceedings},
     year         = {2022},
     organization = {IEEE}
}
```

**APA Style**

```text
Biadgligne, Y., & Smaïli, K. (2022). Offline corpus augmentation for English–Amharic machine translation. In ICICT CPS Conference Proceedings. IEEE.
```

