Overview:

This project focuses on the cleaning, analysis, and processing of publicly available English conversational datasets to identify conversations with potential commercial intent. By leveraging advanced language models, such as GPT4ALL with the LLaMA 38B model, the analysis determines whether a conversation demonstrates commercial intent.

Key Dataset:

The primary dataset used for analysis is WildChat:
1. WildChat - https://huggingface.co/datasets/allenai/WildChat-1M/tree/main/data

Additionally, the following datasets were were cleaned and prepared:

1. Dialog Studio - https://huggingface.co/datasets/Salesforce/dialogstudio
2. UltraChat200k - https://huggingface.co/datasets/HuggingFaceH4/ultrachat_200k
3. ShareGPT - https://huggingface.co/datasets/RyokoAI/ShareGPT52K

Objectives:

Data Cleaning: Standardize and preprocess conversations in the datasets.
Keyword Identification: Detect commercial keywords within conversations.
Commercial Intent Analysis: Use GPT4ALL (LLaMA 38B) to classify conversations as having commercial intent.

Repository Content:

Code for WildChat Dataset: Scripts for data cleaning and preparation specific to the WildChat dataset.
Code for Other Datasets: Cleaning scripts for the Dialog Studio, UltraChat200k, and ShareGPT datasets.

Cleaning Wildchat - 
This folder has the code to filter the WildChat data for English conversaations by eliminating the conversations that are in the filter out words list in the code. Download all WildChat data from the above link.

Cleaning other Datasets - 
This folder has the code to clean the other above mentioned datasets based on the search keywords and filterout key words.
To use this code download the data from the links above and change the paths as required.

Llama_wildchat_analysis.ipynb - Uses LLama to analyse the cleaned wildchat data for potential commercial intent and updates the conversations with the commercial intent, the commercial intent type, indusrty and confidence score to a google sheet automatically. 
To setup an automatic google sheet update refer to this article -https://medium.com/daily-python/python-script-to-edit-google-sheets-daily-python-7-aadce27846c0

Usage:

Clone the repository and ensure required dependencies are installed.
Use the provided cleaning scripts to preprocess individual datasets.
Run the analysis module to identify conversations with commercial intent.
This repository serves as a foundation for processing large-scale conversational datasets with a focus on commercial relevance.
