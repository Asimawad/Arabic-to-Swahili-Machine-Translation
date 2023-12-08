# Arabic-Swahili Translation Dataset

## Overview
This dataset is a crucial component of our neural machine translation project, aimed at facilitating translation between Arabic and Swahili. It comprises 32,000 sentence pairs, providing a rich resource for training and evaluating machine translation models for these languages.

## Data Sources
- **Primary Source:** The dataset predominantly features text from the Bible, which offers thematic cohesion and linguistic depth. The Bible's text, split into individual verses, forms the backbone of this dataset. Arabic text was sourced from DOCX formats from [here](http://www.bible.org), while Swahili text was extracted from a publicly available PDF file [available here](http://www.arabicbible.com/).
- **Microsoft NTREX-128 Dataset:** To enhance the dataset with non-religious content, 2,000 sentence pairs from Microsoft’s NTREX-128 dataset were integrated. This addition broadens the dataset's scope to encompass a diverse range of subjects and styles.

## Usage
This dataset is intended for use in machine translation tasks between Arabic and Swahili. It can be employed to train models, evaluate translation accuracy, and conduct research in the field of low-resource language processing.

## Acknowledgments
- The Bible text, a common source in MT systems for low-resource languages, was instrumental in creating this dataset.
- Microsoft’s NTREX-128 dataset provided valuable additional content, enhancing the diversity and realism of the translation challenges.

## Citation
If you use this dataset in your research, please cite the following:

```bibtex
@misc{
osman2023machine,
title={{MACHINE} {TRANSLATION} {BASELINES} {FOR} {ARABIC} - {SWAHILI}},
author={Asim Awad Osman and Ahmed Emadeldin Almahady and Muhammed Saeed and Hiba Hassan Sayed},
year={2023},
url={https://openreview.net/forum?id=aVepdnlRb5}
}
```
- C. Federmann, T. Kocmi, and Y. Xin, “NTREX-128–news test references for MT evaluation of 128 languages,” in Proceedings of the First Workshop on Scaling Up Multilingual Evaluation, 2022, pp. 21–24.


