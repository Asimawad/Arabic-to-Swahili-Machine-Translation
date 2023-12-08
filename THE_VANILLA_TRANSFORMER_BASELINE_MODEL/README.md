# Arabic-Swahili Neural Machine Translation - Vanilla Transformer Model (BASELINE)

## Overview
This file contains the Vanilla Transformer models for the Arabic-Swahili Neural Machine Translation (NMT) project. It's part of a research effort to develop effective machine translation systems for low-resource language pairs. This specific model is one of several explored in the project, focusing on the Transformer architecture.
The results reported from the Baseline model were considered good in the context of low resource neural machine translation. The model scored 14.25 BLEU points in the Arabic to
Swahili direction and 10.5 BLEU points in the Swahili to Arabic Direction giving good indicators for future models.
## Getting Started
To run this model, you'll need to upload one of the provided notebooks along with the data files contained inside the DATA_USED file to Google Colab or a similar Jupyter Notebook environment.

### Prerequisites
- Google Colab account or Jupyter Notebook environment
- Basic understanding of Python and machine learning concepts

### Installation and Setup
1. **Download Files**: Download the Jupyter notebook (`ARTOSW_FINAL_BASELINE_MODEL.ipynb`) and the accompanying data files from this repository.
2. **Upload to Colab**: Upload these files to your Google Colab workspace.
3. **Open the Notebook**: Open `ARTOSW_FINAL_BASELINE_MODEL.ipynb` in Colab.

### Running the Notebook
- Follow the instructions in the notebook to install dependencies, preprocess data, train the model, and evaluate its performance.
- The notebook is well-commented to guide you through each step of the process.

## Models Description
This model utilizes the Vanilla Transformer architecture for machine translation. Key features include:
- Encoder-Decoder structure based on attention mechanisms
- Custom hyperparameters tuned for the Arabic-Swahili language pair
- Preprocessing steps including tokenization and subword segmentation

## Dataset-DATA_USED
The Data.zip file contains all of the training data, which is used to traing the bpe models
The dataset used in this model includes parallel corpora for Arabic and Swahili languages, tailored for machine translation tasks. The data is already included in the provided files.
27531 training set  
2000 validation set
3281 test set
## Results
After approximately 300 epochs of training:
1-With BPE:
The Arabic to Swahili Model : 14.25 BLEU points
The Swahili to Arabic Model : 10.51 BLEU points

1-Without BPE:
The Arabic to Swahili Model : 11.71 BLEU points
The Swahili to Arabic Model : 8.64  BLEU points

##Check the models checkpoints
Arabic to Swahili: https://drive.google.com/file/d/151MsZWz5ZQGK-VrzepwMnzYRCSKWUZoG/view?usp=sharing
Swahili to Arabic: https://drive.google.com/file/d/1TZKJuO-M_ZRRlnKNMciXWmueirJaJuxP/view?usp=sharing

