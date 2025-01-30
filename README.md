# WSDM Cup 2025 - Multilingual Chatbot Arena

## Overview

This repository contains my project submission for the WSDM Cup 2025, part of the 18th ACM International Conference on Web Search and Data Mining. The competition challenges participants to predict which chatbot responses users will prefer in a multilingual setting.

## Problem Statement

Participants are tasked with predicting user preferences between two responses provided by large language models (LLMs) to a given prompt in various languages. My solution leverages the Language-agnostic BERT Sentence Embedder (LaBSE) model to understand and compare the semantic similarity of responses to determine user preference.

## Dataset

The data provided by Kaggle includes:
- `train.parquet`: Contains training data with prompts, responses, and user-selected preferences.
- `test.parquet`: Test dataset for which the model will predict preferences.

## Model

My approach utilizes:
- **SentenceTransformer**: For generating embeddings from text data.
- **Cosine Similarity**: To measure the similarity between the embeddings of prompts and responses, forming the basis of our prediction.

## File Structure

. ├── models │ └── LaBSE_model ├── notebooks │ └── prediction_notebook.ipynb ├── src │ ├── model.py │ └── utils.py ├── README.md └── requirements.txt

## Setup & Installation

Install the necessary Python packages:

```bash
pip install -r requirements.txt
bash```

## Usage

To execute the prediction model, navigate to the `notebooks` directory and open the Jupyter notebook:


## Competition Rules

Participants must adhere to the following rules set forth by the competition:
- No internet access during run-time.
- Use of publicly available data is allowed.
- All submissions must be made through Kaggle Notebooks.

Detailed rules are available [here](https://kaggle.com/competitions/wsdm-cup-multilingual-chatbot-arena/rules).

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.

## Citation

If you use the dataset or methodologies described in this competition, please cite the competition organizers:

@misc{wsdm2025chatbot, title={WSDM Cup - Multilingual Chatbot Arena}, author={Chiang, Wei-lin and others}, year={2024}, publisher={Kaggle}, url={https://kaggle.com/competitions/wsdm-cup-multilingual-chatbot-arena} }


