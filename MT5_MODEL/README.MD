# MT5 Fine-Tuning for Arabic-Swahili Bidirectional Translation

## Overview
This directory contains the MT5 fine-tuning model designed for bidirectional translation between Arabic and Swahili. The model leverages Google's MT5, a variant of the T5 model optimized for multilingual understanding and generation. 

To calculate the BLEU score for this model, the fine-tuned model is fed with both test sets since this model is trained to translate in both
directions, and then, the predictions of the model are used alongside the target sentences to calculate BLEU score.
This model scored 20.14 BLEU points outperforming the baseline model by(+6) BLEU points in the Arabic to Swahili direction. The model also scored 11.66 BLEU points in the opposite direction outperforming the Baseline by one BLEU point.
This result proves our hypothesis that pre-trained models can outperform The models trained from scratch, but for MT5, the margin was not that large

## Structure
- `MT5_FINAL.ipynb`: The main Jupyter notebook with the complete fine-tuning and evaluation process.
- `mt5_data.zip`: The dataset used for training and evaluating the model.
- `Arabic_to_Swahili_REPORT_RESULTS.txt`: Contains Arabic to Swahili predicted translations alongside the true translations.
- `Swahili_to_Arabic_REPORT_RESULTS.txt`: Contains Swahili to Arabic predicted translations alongside the true translations.

## Getting Started
To use this model, you need to upload the Jupyter notebook (`MT5_FINAL.ipynb`) and the `mt5_data.zip` file to a compatible environment like Google Colab.

### Prerequisites
- Google Colab or a similar Jupyter Notebook environment.
- Basic understanding of Python, Machine Learning, and the T5/MT5 models.

### Installation and Setup
1. **Download Files**: Download the `MT5_FINAL.ipynb` notebook and `mt5_data.zip` from this repository.
2. **Upload to Colab**: Transfer these files to your Google Colab workspace.
3. **Open and Run the Notebook**: Follow the steps in `MT5_FINAL.ipynb` for model fine-tuning and evaluation.

## Model Description
This MT5 fine-tuning model is set up for bidirectional translation:
- The model is capable of translating both from Arabic to Swahili and Swahili to Arabic.
- It utilizes the pre-trained 'google/mt5-base' model as a starting point.
- The fine-tuning process includes several epochs of training with carefully chosen hyperparameters.

## Dataset
- The dataset includes parallel sentences in Arabic and Swahili in tsv formats which are used then to train the model in both directions.
- It's split into training and test sets for both translation directions.

## Results
- BLEU scores are calculated for both translation directions.
- For Arabic to Swahili, the BLEU score reached 20.14 after 6 epochs.
- For Swahili to Arabic, the BLEU score reached 11.66 after 6 epochs.

## See the model Checkpoint
https://drive.google.com/drive/folders/1t7pB6iPiBAC5AwhQzz6Ddm2_JphQZqoo?usp=sharing

## Contributing
Contributions to improve the model or its implementation are welcome. Please refer to the main project repository for contribution guidelines.

