# Arabic-Swahili Neural Machine Translation

## Introduction
Africa has over 2,000 spoken languages, and many of these languages are spoken by millions or
tens of millions of speakers. However, these languages are poorly represented in existing natural
language processing (NLP) datasets, research, and tools.
Most developments in NLP have been focused on the English language, other European
languages, and a few Asian languages like Chinese and Japanese; these languages are regarded
as high-resource languages based on the size of available labeled and unlabelled corpora on the
web. While there are many low-resource languages in different regions of the world, the situation
of African languages is grave, with all the indigenous African languages falling within the class of
low-resource languages. thus limiting the opportunities of NLP to over 1.2 billion people living
in Africa whose native languages are rarely supported by technology.
There are many factors responsible for the underrepresentation of African languages. Some
are data-related, i.e., the lack of labeled datasets for several NLP tasks, and others are societal
factors, such as the geographical and language diversity of NLP researchers. In this context,
we address the NLP task of Neural Machine Translation (NMT) for the low-resource African
language pair Arabic and Swahili.

## Background/Problem Statement
The problem at hand pertains to the challenges associated with low-resource language pairs.
The primary issue lies in the scarcity of parallel corpora because there is no known work nor
parallel corpora on machine translation for Arabic and Swahili languages. Also, the effectiveness
of state-of-the-art NMT architectures has not been investigated on this language pair. The
purpose of this work is to develop Neural Machine Translation systems that benchmarks NMT
research between Arabic and Swahili languages as well as create a parallel dataset for future
work. We investigate and compare different methods for building NMT models, both building
from scratch models and fine-tuning pre-trained multilingual models.

## Research Objectives
a. Create and publish the largest parallel corpus for the Arabic-Swahili language pair to address
the challenge of the lack of standardized datasets for MT tasks for these languages.
b. Leverage deep learning models to create a baseline NMT system.
c. Validate that using a small dataset to fine-tune large multilingual models improves translation.
quality significantly, even for a morphologically rich language like Arabic.
d. Evaluate and compare the performance of both approaches using quantitative and qualitative methods.

## Methodology
Our methods for benchmarking the translation between Arabic and Swahili revolve around
modifying Large multilingual translation models with a little fine-tuning training using our new
dataset.
We leveraged that pre-training and saw much better results than training our own smaller model
from scratch.
Hence, to further expand our experiments to more advanced models, a baseline model is constructed.
A baseline model serves as a fundamental point of reference and comparison in machine translation experiments. Its primary role is to provide a benchmark against the performance of more
advanced models.
In the context of validating the fine-tuning of a large model using a small dataset, the baseline model offers several critical benefits. Firstly, it offers a clear starting point, showcasing the
initial translation quality achievable with standard methods. By comparing the performance of
the fine-tuned model against this baseline, we can quantitatively and qualitatively measure the
extent to which the limited data and fine-tuning process have enhanced translation accuracy and
fluency.
Fine-tuning means taking a model that was trained on a large amount of data and doing a little
bit more training with a specific dataset.
As already mentioned, resources for solving this problem are scarce, and transformer-based models do not perform well with insufficient data. For this reason, we leverage transfer learning to
speed up the learning process.
Conditional text generation (CTG) multilingual models available for fine-tuning are not as common as encoder-based models. However, after an extensive search, we were left with two equally
interesting candidates, which will be discussed later in this chapter.

## Dataset
Datasets stand as a cornerstone, driving the remarkable progress witnessed in the current
era of deep learning and large-scale neural models. The ability of deep learning to excel across
tasks is inherently linked to the presence of representative datasets. To that extent, there is a
notable dataset gap in the context of neural models geared toward translation tasks, specifically
the translation between Arabic and Swahili.
Translation datasets consist of parallel sentences in source and target languages, allowing models
to learn the relationships between linguistic structures and meanings.
We introduce a new dataset to the machine translation community by collecting 32000 sentence
pairs for the Arabic-Swahili language pair.

## Installation and Usage
All Notebooks and project codes were implemented using google Colab/Colab Pro and VScode with python 3.8 or newer version

## Results
Our findings, evaluated using Blue scores, indicate the effectiveness of fine-tuning pre-trained
models. Our best-performing model achieved a remarkable 30.9 Blue Points, marking a significant
16-point improvement over the baseline model. This demonstrates that fine-tuning pre-trained
models can substantially enhance translation quality for the Arabic-Swahili language pair, even
with limited parallel data. These results provide valuable insights into the potential for further
advancements in MT systems, particularly for underrepresented languages spoken in Africa.

## Contributors
- Asim Osman 
- Ahmed Elmahdy
- Mohammed Saeed

## License
[MIT License](LICENSE)

## Contact Informations:
Email Address :Asim.awad98@gmail.com

