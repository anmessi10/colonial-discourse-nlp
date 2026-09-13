# NLP Analysis of Colonial and Settler-Colonial Newspaper Discourse in 1939

An NLP-based analysis of English-language newspaper discourse concerning
People, Land, and Culture in India, British Malaya, and Australia in 1939.

## Overview

This project examines how English-language newspapers represented people,
land, and culture across India, British Malaya, and Australia in 1939.

India and British Malaya were under British colonial rule at the time,
while Australia is examined as a settler-colonial context. The year 1939
provides an important historical setting because it was the year the Second
World War began, creating a broader context of political and imperial
uncertainty.

The project combines manual thematic annotation with natural language
processing (NLP) techniques to identify differences in vocabulary and
contextual patterns across the three settings.

## Research Question

How did English-language newspaper discourse differ in its representation
of people, land and culture across India, British Malaya and Australia in
1939, and what common linguistic patterns can be identified using NLP?

## Corpus

The final corpus contains 36 newspaper articles and 8,380 clean word tokens.

| Country | Articles | Clean Tokens |
|---------|----------|--------------|
| India | 9 | 2,302 |
| British Malaya | 10 | 3,178 |
| Australia | 17 | 2,900 |
| **Total** | **36** | **8,380** |

Articles were identified through targeted searches of historical newspaper
archives and then manually reviewed for relevance to the research question.

The corpus focuses on three themes:

- **People** – representation, race, labour, welfare, political rights,
  identity, discrimination, and government treatment
- **Land** – land ownership, settlement, agriculture, reserves, territory,
  development, and displacement
- **Culture** – customs, traditions, religion, language, education,
  ceremonies, and other cultural practices

Articles may be assigned to more than one theme.

## Data Sources

The newspaper corpus was constructed from historical newspaper archives,
including:

- **India:** The Bombay Chronicle
- **British Malaya:** The Straits Times and Malaya Tribune
- **Australia:** The Sydney Morning Herald

Article metadata, thematic annotations, and archive information are
provided in `master_dataset.csv`.

## Methodology

The analysis consists of four main stages:

1. **Corpus construction and validation**
2. **Manual thematic annotation**
3. **Conservative OCR preprocessing**
4. **NLP analysis**

The NLP analysis includes:

- normalized word-frequency analysis
- article-level TF-IDF
- collocation analysis
- concordance analysis
- exploratory lexical comparison

Historical vocabulary was retained rather than modernized. OCR cleaning was
limited to obvious formatting and spacing artefacts.

## Key Findings

The analysis identified different lexical patterns across the three settings.

- **India:** discourse was strongly associated with political and
  institutional vocabulary, including terms relating to Congress,
  government, conferences, freedom, and social groups.
- **British Malaya:** discourse showed a strong focus on the multiethnic and
  colonial setting, with frequent references to Malay, Indian, Chinese,
  labour, government, and Malaya.
- **Australia:** discourse was strongly centred on Aboriginal populations,
  government policy, reserves, administration, racial classification, and
  cultural practices.

The results suggest that newspaper discourse varied according to the
specific colonial or settler-colonial context, while also showing recurring
patterns involving government authority, racial categorisation, labour,
land, and cultural identity.

## Repository Structure

```text
colonial-discourse-nlp/
│
├── data/
│   ├── raw/
│   │   ├── india/
│   │   ├── british-malaya/
│   │   └── australia/
│   └── processed/
│
├── notebooks/
│   ├── 01_data_quality.ipynb
│   ├── 02_preprocessing.ipynb
│   └── 03_results.ipynb
│
├── results/
│   ├── figures/
│   ├── corpus_composition.csv
│   ├── thematic_distribution.csv
│   ├── article_level_tfidf.csv
│   └── normalized_frequencies.csv
│
├── master_dataset.csv
├── requirements.txt
├── README.md
└── paper/
    └── colonial_discourse_1939.pdf
```
## Research Paper

[Read the full research paper (PDF)](paper/colonial_discourse_1939.pdf)

## Notebooks

- [Data Quality](notebooks/01_data_quality.ipynb)
- [Preprocessing](notebooks/02_preprocessing.ipynb)
- [Results](notebooks/03_results.ipynb)

## Reproducibility

Clone the repository and install the required Python packages:

```bash
git clone https://github.com/anmessi10/colonial-discourse-nlp.git
cd colonial-discourse-nlp
pip install -r requirements.txt
```

The notebooks are intended to be run in the following order:

1. `01_data_quality.ipynb` — validates the corpus and metadata.
2. `02_preprocessing.ipynb` — performs OCR cleaning and text preprocessing.
3. `03_results.ipynb` — generates the NLP analysis and results.

The raw and processed OCR text files are not included in the public repository. The repository contains the metadata, analysis notebooks, results, and research paper.

## Limitations

The corpus is relatively small and was constructed through targeted historical newspaper sampling rather than comprehensive archival collection. OCR errors may remain despite conservative preprocessing, and historical terminology has been preserved rather than modernized. The thematic annotations are also interpretive and may involve overlap between People, Land, and Culture.

The three country corpora are not equal in size, and the selected newspapers do not represent all newspaper discourse in their respective historical contexts. Therefore, the findings should be interpreted as patterns within the sampled corpus rather than as comprehensive representations of India, British Malaya, or Australia in 1939.

## Research Paper

[Read the full research paper (PDF)](paper/colonial_discourse_1939.pdf)

[View the editable Word version](paper/Colonial%20and%20Settler-Colonial%20Discourse%20in%201939%20An%20NLP%20%20Analysis%20of%20%20People%2C%20Land%2C%20and%20Culture%20in%20India%2C%20British%20Malaya%2C%20and%20Australia.docx)

## Title:

NLP Analysis of Colonial and Settler-Colonial Newspaper Discourse in 1939:
People, Land, and Culture in India, British Malaya, and Australia

## Author:

Anish Sanjay Kulkarni

Master of Information Technology
UNSW Sydney


