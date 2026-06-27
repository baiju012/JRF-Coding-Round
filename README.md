# English–Hindi Dataset Processing and Translation Assessment

## Overview

This repository contains the solutions for:

- Assignment 1: English–Hindi Dataset Processing and Analysis
- Assignment 2: English-to-Hindi Translation using a Large Language Model (LLM)

All tasks were implemented and executed using Google Colab.

---

## Repository Structure

```text
English-Hindi-Assessment/
│
├── assignment1_and_2.ipynb
├── assignment1_cleaned_dataset.xlsx
├── assignment2_translation.xlsx
├── evaluation_scores.txt
└── README.md
```

---

## Assignment 1: Dataset Processing

### Objective

The objective of Assignment 1 was to process an English–Hindi parallel dataset and create a cleaned dataset according to the following conditions:

- Use at least 10,000 sentence pairs.
- Calculate word counts for English and Hindi sentences.
- Keep only sentences with word counts between 5 and 50 in both languages.
- Calculate the difference between English and Hindi word counts.
- Keep only sentence pairs where the difference is between -10 and +10.
- Export the final cleaned dataset to an Excel file.

### Output File

```text
assignment1_cleaned_dataset.xlsx
```

### Columns in the Excel File

1. English Sentences
2. Hindi Sentences
3. Word Count (English)
4. Word Count (Hindi)
5. Difference between Word Count (English) and Word Count (Hindi)

---

## Assignment 2: Translation with LLM

### Objective

The objective of Assignment 2 was to:

- Select 100 English sentences from the cleaned dataset.
- Translate them into Hindi using a Large Language Model (LLM).
- Calculate BLEU, CHRF, and TER evaluation metrics.
- Save the translated sentences and evaluation scores.

### Translation Model Used

```text
Helsinki-NLP/opus-mt-en-hi
```

### Output Files

```text
assignment2_translation.xlsx
evaluation_scores.txt
```

### Columns in the Translation Excel File

1. Original English Sentence
2. Model-generated Hindi Translation

---

## Requirements

The following Python libraries were installed in Google Colab:

```python
!pip install pandas openpyxl transformers sentencepiece sacrebleu datasets
```

---

## How to Run Assignment 1 (Google Colab)

1. Open `Assignment1.ipynb` in Google Colab.
2. Upload or clone the dataset repository.
3. Run all cells sequentially.
4. The notebook generates:

```text
assignment1_cleaned_dataset.xlsx
```

---

## How to Run Assignment 2 (Google Colab)

1. Open `Assignment2.ipynb` in Google Colab.
2. Upload `assignment1_cleaned_dataset.xlsx`.
3. Run all cells sequentially.
4. The notebook:
   - Selects 100 English sentences.
   - Translates them into Hindi using the LLM.
   - Calculates BLEU, CHRF, and TER scores.
   - Generates:

```text
assignment2_translation.xlsx
evaluation_scores.txt
```

---

## Evaluation Metrics Used

The following metrics were used to evaluate the translation quality:

- BLEU (Bilingual Evaluation Understudy)
- CHRF (Character n-gram F-score)
- TER (Translation Edit Rate)

The scores are stored in:

```text
evaluation_scores.txt
```

---

## Tools and Technologies Used

- Google Colab
- Python 3
- Pandas
- Hugging Face Transformers
- SentencePiece
- SacreBLEU
- OpenPyXL

---

## Author

Name: Mr. Baiju Kumar

Date: 27 June 2026
