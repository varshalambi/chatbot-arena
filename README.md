WSDM Cup 2025 - Multilingual Chatbot Arena
Overview
This repository contains the machine learning model developed for the WSDM Cup 2025, part of the 18th ACM International Conference on Web Search and Data Mining. The competition challenges participants to predict human preference across multiple languages in a head-to-head battle between chatbots.

Problem Statement
Large Language Models (LLMs) are being integrated into digital interactions; however, aligning their responses with human preferences remains a challenge. This project involves creating a model that predicts which responses from LLMs will be preferred by users in the Chatbot Arena, a platform where users interact with multiple chatbots.

Dataset
The dataset used in this project includes:

train.parquet: Training data consisting of prompts and responses from LLMs, along with user preferences.
test.parquet: Test data to evaluate the model.
The data is sourced from the official competition hosted on Kaggle.

Model Description
The model utilizes the LaBSE (Language-agnostic BERT Sentence Embedder) to generate embeddings for the text data, which are then used to compute cosine similarities between prompts and responses. The model predicts the preferred response based on these similarities.

Repository Structure
plaintext
Copy
/
|- models/
|   |- LaBSE_model/
|- notebooks/
|   |- prediction_notebook.ipynb
|- src/
|   |- model.py
|   |- utils.py
|- README.md
|- requirements.txt
Installation
To set up the project environment, run:

bash
Copy
pip install -r requirements.txt
Usage
To run the prediction notebook:

bash
Copy
jupyter notebook notebooks/prediction_notebook.ipynb
Competition Rules & Ethics
Participants must adhere to the rules set forth by the competition:

No internet access during run-time.
Use only freely and publicly available external data.
Submissions must be made through Kaggle Notebooks.
Refer to the official competition rules for more details.

Citation
If you use the contents of this repository, please cite:

bibtex
Copy
@misc{wsdm2025chatbot,
  title={WSDM Cup - Multilingual Chatbot Arena},
  author={Wei-lin Chiang, Evan Frick, Lisa Dunlap, and others},
  year={2024},
  publisher={Kaggle},
  howpublished={\url{https://kaggle.com/competitions/wsdm-cup-multilingual-chatbot-arena}}
}
Contributing
Contributions to this project are welcome. Please refer to the contributing guidelines before making a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.
