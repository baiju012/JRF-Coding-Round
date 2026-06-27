Assignment 1: Dataset Processing
Objective

Process the English–Hindi parallel dataset and create a cleaned dataset according to the following conditions:

Use at least 10,000 sentence pairs.
Keep sentences having 5–50 words in both English and Hindi.
Calculate the word count difference.
Keep only rows where the difference is between -10 and +10.
Export the final data to an Excel file.
Output File
assignment1_cleaned_dataset.xlsx
Excel Columns
English Sentences
Hindi Sentences
Word Count (English)
Word Count (Hindi)
Difference between Word Count (English) and Word Count (Hindi)
Assignment 2: Translation with LLM
Objective
Select 100 English sentences from Assignment 1.
Translate them into Hindi using an LLM.
Calculate BLEU, CHRF, and TER scores.
Save the translations and evaluation results.
Translation Model Used
Helsinki-NLP/opus-mt-en-hi
Output Files
assignment2_translation.xlsx
evaluation_scores.txt
Translation Excel Columns
Original English Sentence
Model-generated Hindi Translation
Requirements

Install the required Python packages:

pip install pandas openpyxl transformers sentencepiece sacrebleu datasets

Alternatively:

pip install -r requirements.txt
How to Run Assignment 1

Navigate to the Assignment1 folder:

cd Assignment1

Run:

python dataset_processing.py

The script will:

Read the English and Hindi text files.
Create a DataFrame.
Calculate word counts.
Apply filtering conditions.
Generate:
assignment1_cleaned_dataset.xlsx
How to Run Assignment 2

Navigate to the Assignment2 folder:

cd Assignment2

Run:

python translation.py

The script will:

Load the cleaned dataset.
Select 100 English sentences.
Translate them into Hindi using the LLM.
Calculate BLEU, CHRF, and TER scores.
Generate:
assignment2_translation.xlsx
evaluation_scores.txt
Evaluation Metrics

The following evaluation metrics are used:

BLEU (Bilingual Evaluation Understudy)
CHRF (Character n-gram F-score)
TER (Translation Edit Rate)

The results are stored in:

evaluation_scores.txt
Tools and Libraries Used
Python 3
Google Colab
Pandas
Hugging Face Transformers
SentencePiece
SacreBLEU
OpenPyXL
Author

Name: Mr. Baiju Kumar

Date: 27/06/2026
