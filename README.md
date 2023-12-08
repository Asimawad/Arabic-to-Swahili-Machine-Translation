# Arabic-Swahili Neural Machine Translation

## Introduction
In Africa, with over 2,000 languages spoken, the representation of these languages in natural language processing (NLP) is disproportionately low. This underrepresentation is stark considering that many African languages are native to millions. The focus in NLP has largely been on high-resource languages like English, other European languages, and some Asian languages. This leaves a significant portion of the African population, with their native languages largely unsupported by technological advancements in NLP. 

## Background/Problem Statement
This project addresses the gap in Neural Machine Translation (NMT) for low-resource languages, specifically between Arabic and Swahili. The lack of parallel corpora and research for these languages poses a challenge. Our goal is to establish NMT systems that benchmark research in Arabic-Swahili translation and contribute a parallel dataset for future research. The project explores various NMT model-building approaches, including constructing models from scratch and fine-tuning pre-trained multilingual models.

## Research Objectives
- Develop the largest parallel corpus for Arabic-Swahili translation to mitigate the lack of standardized datasets.
- Implement deep learning models to establish a baseline NMT system.
- Demonstrate that fine-tuning large multilingual models with a smaller dataset significantly enhances translation quality, even for complex languages like Arabic.
- Conduct both quantitative and qualitative evaluations to compare the performance of the developed approaches.

## Methodology
Our approach focuses on modifying large multilingual translation models with minimal fine-tuning using our newly developed dataset. This method yielded superior results compared to training smaller models from scratch. We establish a baseline model to serve as a reference for performance comparison. This baseline aids in quantifying the improvements brought about by fine-tuning with limited data.

## Dataset
We present a new dataset comprising 32,000 sentence pairs for Arabic-Swahili translation. This dataset aims to fill the existing gap in translation datasets for these languages, providing a foundation for models to understand linguistic structures and meanings in both languages.

## Installation and Usage
The project code and notebooks are compatible with Google Colab/Colab Pro and VScode, using Python 3.8 or newer.

## Results
Evaluated through BLEU scores, our best-performing model achieved an impressive 30.9 BLEU points, a significant leap from the baseline model's score. This outcome underscores the efficiency of fine-tuning pre-trained models in enhancing translation quality for Arabic-Swahili, even with limited data.

## Contributors
- Asim Osman 
- Ahmed Elmahdy
- Mohammed Saeed

## License
This project is licensed under the [MIT License](LICENSE).

## Contact Information
For inquiries, please reach out via email at Asim.awad98@gmail.com.
