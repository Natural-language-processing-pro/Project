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
├── requirements.txt
├── data/
│   ├── PetSemetary_updated.txt        (ignored)
│   ├── TheShining_updated.txt         (ignored)
│   ├── fear_lexicon.txt
├── .gitignore
└── README.md
```

## Note on Text Files and Copyright

The full novel text files (`PetSemetary_updated.txt` and `TheShining_updated.txt`) are not included in the repository and are explicitly excluded using `.gitignore` to comply with copyright restrictions.

Only derived outputs (frequency tables, figures, embeddings, and network graphs) are included.

# Notebook 1 — Text Cleaning and Tokenization  
Purpose: Prepare the raw text for linguistic and statistical analysis.

Includes:
- Loading local text files 
- Text normalization (lowercasing, noise removal, whitespace cleanup) 
- Word and sentence tokenization 
- Basic corpus statistics 

Outcome: Clean, standardized datasets for both novels.

# Notebook 2 — Fear Word Frequency Analysis  
Purpose: Measure the use of fear-related vocabulary across the two novels.

Includes:
- Loading a curated fear-lexicon (`fear_lexicon.txt`) 
- Counting fear-word frequencies 
- Side-by-side visual comparisons with static axes 

Findings: 
- Pet Sematary emphasizes death, grief, and physical danger 
- The Shining emphasizes psychological, supernatural, and internal fear 

# Notebook 3 — Fear Collocations and Co-Occurrence Networks  
Purpose: Identify deeper fear patterns through contextual and relational analysis.

Includes:
- Extraction of 2-gram and 3-gram fear collocations 
- Correction of contraction-tokenization artifacts 
- Construction of fear-word co-occurrence graphs 
- Community detection for thematic clustering 
- Refined “top-30 fear word” networks for clear visualization 

Findings: 
- Pet Sematary: clusters around death, injury, grief, trauma 
- The Shining: clusters around madness, haunting, psychological breakdown 

# Notebook 4 — Sentence-Level Structure and Readability  
Purpose: Compare stylistic and structural writing patterns.

Includes:
- Sentence length distribution 
- Readability metrics (Flesch, FK Grade Level) 
- Dialogue vs. narration analysis 
- Punctuation statistics 
- Sentence-type classification 

Findings: 
- Pet Sematary uses more direct, emotionally expressive structures 
- The Shining exhibits more complex, introspective narrative forms 

# Notebook 5 — Embedding-Based Semantic Analysis  
Purpose: Analyze deeper semantic and stylistic differences.

Includes:
- Sentence embeddings (e.g., Sentence Transformers, spaCy) 
- Cosine similarity distributions 
- Semantic clustering of fear-related contexts 
- PCA / t-SNE visualizations 

Outcome: High-level conceptual similarity and separation between fear contexts in both novels.

## Research Aim

This project investigates:

How does Stephen King construct fear differently in *Pet Sematary* compared to *The Shining*?

Summary:

| Novel | Dominant Fear Themes | Linguistic Style |
|-------|-----------------------|------------------|
| Pet Semetary | death, injury, grief, bodily decay | concrete, physical, emotionally direct |
| The Shining | madness, haunting, isolation, psychological collapse | introspective, atmospheric, supernatural |

## Setup Instructions

All Python dependencies used across the notebooks are provided in `requirements.txt`.

To install the full environment:

```
pip install -r requirements.txt
```

Download the necessary NLTK resources:

```python
import nltk
nltk.download("punkt")
nltk.download("punkt_tab")
```

Launch the notebooks:

```
jupyter notebook
```

## Data Handling

- The novel text files are local only and excluded from version control using `.gitignore`. 
- `fear_lexicon.txt` is included and safe to distribute. 
- All analysis is performed on cleaned, tokenized, or embedded representations of the text.
