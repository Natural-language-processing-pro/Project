# Stephen King Fear Language Analysis
### Comparative NLP Study of *Pet Sematary* and *The Shining*

This repository contains a five-notebook Natural Language Processing workflow analyzing how Stephen King constructs fear, emotional intensity, and psychological tension across two novels.

## Project Structure

```
.
├── Notebook1.ipynb
├── Fear Emotion Analysis.ipynb
├── notebook3.ipynb
├── notebook4.ipynb
├── notebook5.ipynb
├── data/
│   ├── PetSemetary_updated.txt        (ignored)
│   ├── TheShining_updated.txt         (ignored)
│   ├── fear_lexicon.txt
├── .gitignore
└── README.md
```

## Note on Text Files and Copyright

The full novel text files are excluded using `.gitignore` due to copyright restrictions. Only derived analytical outputs are included.

# Notebook 1 — Text Cleaning and Tokenization
Prepares raw text for linguistic and statistical analysis:
- Loading local text files
- Normalization
- Tokenization
- Corpus statistics

# Notebook 2 — Fear Word Frequency Analysis
Measures fear vocabulary frequency and compares usage across novels.

# Notebook 3 — Fear Collocations and Co-Occurrence Networks
Identifies fear collocations, builds co-occurrence graphs, and detects thematic clusters.

# Notebook 4 — Sentence-Level Structure and Readability
Analyzes readability metrics, sentence structures, punctuation, and dialogue ratios.

# Notebook 5 — Semantic Embedding Analysis
Uses sentence embeddings to analyze deeper stylistic and conceptual patterns.

## Research Aim

How does Stephen King construct fear differently in *Pet Semetary* compared to *The Shining*?

| Novel | Dominant Themes | Style |
|-------|-----------------|-------|
| *Pet Sematary* | death, grief, trauma | concrete and emotional |
| *The Shining* | madness, haunting, isolation | psychological and atmospheric |

## Installation

```
pip install pandas numpy matplotlib nltk networkx
```

Download NLTK:

```python
import nltk
nltk.download("punkt")
nltk.download("punkt_tab")
```

## Data Handling

- Novel text files are local only and excluded from version control.
- `fear_lexicon.txt` is included and safe to distribute.
