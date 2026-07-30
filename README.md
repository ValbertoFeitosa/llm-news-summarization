# LLM News Summarization

Automatic news summarization using open-source Large Language Models (LLMs), with a custom-built evaluation dataset, ROUGE metrics, and comparison against ChatGPT-generated reference summaries.

---

## Overview

Automatic text summarization is one of the most important applications of Natural Language Processing (NLP). The objective is to generate concise summaries while preserving the most relevant information from the original text.

This project implements an end-to-end summarization pipeline using an open-source Large Language Model (LLM). The generated summaries are evaluated quantitatively using ROUGE metrics and compared against reference summaries generated with ChatGPT.

Unlike many demonstration projects, this work also includes the manual construction of a custom evaluation dataset, enabling reproducible experiments and objective model assessment.

---

## Objectives

The main objectives of this project are:

- Develop an automatic news summarization pipeline.
- Apply an open-source Large Language Model.
- Create a custom dataset for summarization evaluation.
- Compare generated summaries with ChatGPT reference summaries.
- Evaluate summary quality using ROUGE metrics.
- Analyze execution time and summarization performance.

---

## Features

- Automatic abstractive news summarization
- Open-source LLM inference
- Prompt engineering
- Batch processing of multiple news articles
- Custom evaluation dataset
- ROUGE-1 and ROUGE-2 evaluation
- Comparison with ChatGPT-generated summaries
- Performance analysis
- Data visualization

---

## Project Workflow

```text
News Collection
        │
        ▼
Dataset Construction
        │
        ▼
Prompt Engineering
        │
        ▼
LLM Summary Generation
        │
        ▼
Reference Summary (ChatGPT)
        │
        ▼
ROUGE Evaluation
        │
        ▼
Performance Analysis
```

---

## Dataset

A custom evaluation dataset was created specifically for this project.

The news articles were manually collected from publicly available online news sources after extensive research and selection. Different topics and writing styles were considered to improve the robustness of the evaluation.

For each news article, a reference summary was generated using ChatGPT, allowing objective comparison between the open-source language model and the reference summaries through ROUGE metrics.

**The original news articles are not distributed in this repository due to copyright restrictions.**

Users interested in reproducing the experiments may create their own dataset following the same directory structure adopted in this project.

---

## Model

This project uses an open-source Large Language Model available through Hugging Face.

The notebook performs:

- Model loading
- Tokenization
- Prompt generation
- Automatic summarization
- Batch inference
- Execution time measurement

---

## Evaluation

The generated summaries are evaluated using the ROUGE metric.

The following indicators are calculated:

- ROUGE-1 Precision
- ROUGE-1 Recall
- ROUGE-1 F1-score
- ROUGE-2 Precision
- ROUGE-2 Recall
- ROUGE-2 F1-score

The reference summaries used during evaluation were generated with ChatGPT exclusively for research and comparison purposes.

---

## Technologies

- Python
- Hugging Face Transformers
- PyTorch
- AutoAWQ
- Accelerate
- Pandas
- Matplotlib
- ROUGE Score
- Google Colab

---

## Repository Structure

```text
llm-news-summarization/
│
├── README.md
├── LICENSE
├── requirements.txt
├── llm_news_summarization.ipynb
│
├── data/
│   └── README.md
│
└── images/
    └── results.png
```

---

## Running the Project

1. Clone the repository.

```bash
git clone https://github.com/ValbertoFeitosa/llm-news-summarization.git
```

2. Install the required libraries.

```bash
pip install -r requirements.txt
```

3. Open the notebook.

```text
llm_news_summarization.ipynb
```

4. Configure the dataset directory.

5. Execute the notebook cells sequentially.

---

## Main Contributions

This project demonstrates:

- Construction of a custom evaluation dataset
- Manual research and selection of news articles
- Practical application of Large Language Models
- Prompt engineering for abstractive summarization
- Automatic quantitative evaluation
- Comparison between open-source LLMs and ChatGPT
- Integration of NLP, data analysis and visualization
- End-to-end reproducible summarization pipeline

---

## Future Work

Possible improvements include:

- Evaluation with BERTScore
- Human evaluation of summary quality
- Comparison with additional LLMs
- PDF document summarization
- Web application deployment
- API development
- Multilingual summarization

---

## Disclaimer

The original news articles are not included in this repository due to copyright restrictions.

The reference summaries generated with ChatGPT are used exclusively for comparative evaluation and should not be interpreted as absolute ground truth.

ROUGE measures lexical similarity and does not fully evaluate factual consistency or semantic quality.

---

## Author

**Valberto Feitosa**

Professor • Data Scientist

Machine Learning • Statistics • Artificial Intelligence • Computer Vision • NLP

GitHub: https://github.com/ValbertoFeitosa

LinkedIn: https://www.linkedin.com/in/valbertofeitosa/
