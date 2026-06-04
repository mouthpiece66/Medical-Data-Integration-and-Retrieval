# Healthcare Information Retrieval System

## Project Overview

This project implements a domain-specific search engine in the healthcare domain. The system integrates multiple datasets related to drug prescriptions and diseases into a centralized data warehouse and provides an information retrieval system capable of searching and ranking relevant medical information.

The project was developed as part of the Information Integration and Analytic Data Processing (IPAI) course.

---

## Objectives

* Integrate healthcare datasets from different sources.
* Design and implement a data warehouse.
* Build an ETL pipeline for data cleaning and integration.
* Generate searchable medical documents.
* Implement information retrieval techniques.
* Evaluate retrieval performance using standard IR metrics.

---

## Datasets

### Dataset 1: Drug Prescription to Disease

Contains relationships between prescribed drugs and associated diseases.

### Dataset 2: Drug Library Dataset

Contains drug descriptions, indications, and medical information.

The datasets were integrated to create a unified healthcare repository suitable for search and analysis.

---

## Data Warehouse Design

### Fact Table

* Drug-Disease Relationships

### Dimension Tables

* Drug
* Disease
* Category
* Source

The dimensional model was designed to support analytical queries and efficient retrieval.

---

## ETL Pipeline

The ETL process includes:

1. Data extraction from CSV and TSV files.
2. Data cleaning and preprocessing.
3. Handling missing values.
4. Text normalization.
5. Dataset integration.
6. Loading transformed data into warehouse tables.

---

## Information Retrieval System

### Text Preprocessing

* Tokenization
* Stopword removal
* Text normalization
* TF-IDF vectorization

### Retrieval Models

* Vector Space Model (TF-IDF)
* BM25

The system ranks documents according to their relevance to the user's query.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* NLTK
* Rank-BM25
* Jupyter Notebook

---

## Project Structure

```text
├── data/
│   ├── Drug prescription to disease.csv
│   └── drugLibTrain_raw.tsv
│
├── notebooks/
│   └── Project_final_IPAI.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Installation

```bash
git clone https://github.com/yourusername/Healthcare-Information-Retrieval-System.git

cd Healthcare-Information-Retrieval-System

pip install -r requirements.txt
```

---

## Usage

Open the notebook and execute all cells:

```bash
jupyter notebook
```

Then open:

```text
Project_final_IPAI.ipynb
```

---

## Results

The search engine successfully retrieves healthcare information by combining structured warehouse data and textual medical descriptions, allowing users to search for drugs, diseases, and related medical information.

---

## Author

Nathalia Alvear       Adilcia D´alva        Rita Barbas

Information Integration and Analytic Data Processing (IPAI)
2025/2026
