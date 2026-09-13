# AI Resume Screening System

## Project Overview

The AI Resume Screening System is a Natural Language Processing (NLP) based system that analyzes resumes and automatically shortlists candidates based on a given job description.

The system reads multiple resume PDFs, converts them into text, preprocesses the text using NLP techniques, extracts features using TF-IDF and Bag of Words, calculates similarity with the job description, ranks resumes, and identifies shortlisted candidates.

## Objective

To build an AI-based resume screening system that:

- Analyzes resume content
- Compares resumes with a job description
- Calculates resume-job similarity
- Ranks candidates based on relevance
- Filters low-scoring resumes

## Dataset

The project uses the Resume Dataset by Snehaan Bhawal from Kaggle.

The project uses 10 Information Technology resume PDFs from the dataset.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- NLTK
- PyPDF2
- Jupyter Notebook

## Project Workflow

### 1. Data Collection

- Collected multiple resume PDF files.
- Converted PDF resumes into text.
- Loaded the job description from a text file.

### 2. Data Preprocessing (NLP)

The resume and job description text are preprocessed using:

- Lowercase conversion
- Punctuation and special-character removal
- Stopword removal
- Tokenization
- Lemmatization

### 3. Feature Extraction

Two feature extraction techniques are used:

- TF-IDF
- Bag of Words (BoW)

### 4. Matching Algorithm

The resumes are matched with the job description using:

- Cosine Similarity
- Keyword Matching
- NLP Similarity Scoring

### 5. Ranking System

Resumes are:

- Ranked according to their similarity score
- Used to display the top matching candidates
- Filtered using a similarity threshold to identify shortlisted candidates

### 6. Output

The system produces:

- Candidate name
- Resume file name
- Resume match score (%)
- Ranking list
- Shortlisted candidates

## Project Structure

```text
AI_Resume_Screening_System/
│
├── data/
│   ├── resumes/
│   │   ├── 27372171.pdf
│   │   ├── 27485716.pdf
│   │   └── ...
│   │
│   └── job_description.txt
│
├── notebooks/
│   └── resume_screening.ipynb
│
├── .gitignore
├── requirements.txt
└── README.md
