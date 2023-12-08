# M2M100 Arabic-Swahili Translation Models

## Overview
This directory contains the fine-tuned M2M100 models for machine translation between Arabic and Swahili. The M2M100, a multilingual machine translation model, was specifically fine-tuned to enhance the performance of translation tasks in both directions: Arabic to Swahili and Swahili to Arabic.

## Model Descriptions
1. **Arabic to Swahili Model**: This model is trained to translate text from Arabic to Swahili. It leverages the M2M100 architecture, fine-tuned on a dataset comprising sentence pairs in both languages.

2. **Swahili to Arabic Model**: Similarly, this model translates Swahili text to Arabic. It also utilizes the M2M100 architecture and is fine-tuned on the same dataset.

## Dataset
The training and validation datasets consist of parallel sentences in Arabic and Swahili. The datasets were prepared by following steps:
- Removal of duplicates and redundant data
- Lowercasing and trimming of spaces
- Tokenization using Byte Pair Encoding (BPE) for efficient handling of subword units in both languages.

## Training
Both models were fine-tuned from an initial M2M100 checkpoint (`418M_last_checkpoint.pt`). The training involved:
- Batch size of 16
- Optimization with Adafactor
- Learning rate scheduling with cosine
- A total of 40,000 updates and a frequency of 100 updates for saving intervals

## Evaluation
The models' performance was evaluated using the BLEU score metric. The BLEU score calculation was done using the Fairseq toolkit, ensuring a standardized measure of translation quality.

## Requirements
- Python packages: `sentencepiece`, `wandb`, `numpy`, `pandas`, `torch`
- Fairseq toolkit
- Google Colab (for easy setup and training)


## Acknowledgments
Special thanks to the creators of the M2M100 model and the Fairseq toolkit, which facilitated the development of these models.

##Results
The BLEU score for this model is calculated the same way as the baseline model, nevertheless, this model proved to be our best-performing model by scoring 30.9 and 26.3 BLEU points in the Arabic to Swahili and Swahili to Arabic respectively.

###Arabic to Swahili:
Without BPE:24.29
With BPE : 30.9

###Swahili to Arabic:
Without BPE:12.55
With BPE : 26.28
