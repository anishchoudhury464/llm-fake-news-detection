# Fake News Detection using FLAN-T5

## Overview

This project develops a Fake News Detection system using Google's FLAN-T5 Large Language Model (LLM). The project investigates how instruction-tuned transformer models perform on fake news classification through prompt engineering and supervised fine-tuning.

The study compares three different approaches:

- Zero-Shot Prompting
- Few-Shot Prompting
- Supervised Fine-Tuning

The objective is to evaluate how supervised fine-tuning improves classification performance compared to prompt-based inference.

---

## Course Information

**Course:** ADS-509 – Applied Large Language Models for Data Science

**University:** University of San Diego

**Project Type:** Final Team Project

---

## Dataset

The project uses the publicly available Fake and Real News Dataset.

Dataset consists of:

- Fake News Articles
- Real News Articles

After preprocessing:

- Total Articles: 44,689
- Fake News: 23,478
- Real News: 21,211

The preprocessing stage removes duplicate records, combines article title and text, cleans formatting issues, and produces a final dataset suitable for model training.

---

## Project Workflow

Raw Dataset

↓

Data Cleaning & Preprocessing

↓

Exploratory Data Analysis

↓

Zero-Shot Prompting

↓

Few-Shot Prompting

↓

Supervised Fine-Tuning

↓

Model Evaluation

---

## Repository Structure

```
fake-news-detection-flan-t5/

├── data/
│   ├── Fake.csv
│   ├── True.csv
│   └── clean_news.csv
│
├── notebooks/
│   ├── 01_Data_Preprocessing.ipynb
│   ├── 02_Exploratory_Data_Analysis.ipynb
│   ├── 03_ZeroShot_FewShot.ipynb
│   └── 04_FLAN_T5_FineTuning.ipynb
│
├── figures/
│
├── requirements.txt
│
├── README.md
│
└── LICENSE
```

---

## Notebook Description

### 01_Data_Preprocessing.ipynb

This notebook performs:

- Loading Fake.csv and True.csv
- Data inspection
- Duplicate removal
- Label creation
- Dataset merging
- Content generation
- Exporting clean_news.csv

---

### 02_Exploratory_Data_Analysis.ipynb

This notebook performs:

- Dataset overview
- Missing value analysis
- Class distribution
- Article length analysis
- Word count analysis
- Correlation analysis
- Word cloud visualization
- Top word frequency analysis

---

### 03_ZeroShot_FewShot.ipynb

This notebook evaluates Google's pretrained FLAN-T5 model without fine-tuning.

Experiments include:

- Zero-Shot Prompting
- Few-Shot Prompting
- Accuracy comparison
- Confusion Matrix
- Classification Report

---

### 04_FLAN_T5_FineTuning.ipynb

This notebook performs supervised fine-tuning of FLAN-T5.

Main steps include:

- Prompt formatting
- Tokenization
- Dataset preparation
- Training
- Validation
- Model evaluation

---

## Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- FLAN-T5
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- WordCloud
- Jupyter Notebook

---

## Installation

Clone the repository

```bash
git clone https://github.com/<username>/fake-news-detection-flan-t5.git
```

Move into the project

```bash
cd fake-news-detection-flan-t5
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Project

Execute the notebooks in the following order:

1. Data Preprocessing
2. Exploratory Data Analysis
3. Zero-Shot vs Few-Shot Prompting
4. FLAN-T5 Fine-Tuning

---

## Results

The project demonstrates that supervised fine-tuning substantially improves fake news classification performance compared to prompt engineering approaches alone.

---

## Future Work

Possible future improvements include:

- LoRA Fine-Tuning
- PEFT
- Quantization
- Larger LLMs
- Instruction Optimization
- RAG-based Fake News Detection

---

## Team Members

- Anish Choudhury
- Krishna Sindhu Karri
- Praseeda Saripalle

---

## License

This project is developed for educational purposes as part of ADS-509 – Applied Large Language Models for Data Science.
