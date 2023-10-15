# EnKoSUM: English-Korean Summarization Via Pyramid structure for MD summarization 

![python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

## Overview
In countries where English is not the native language, such as South Korea, Japan, and Russia, people often encounter documents written in English. To understand and utilize these documents, individuals who are not proficient in English often face the laborious task of first translating the content into their native language and then summarizing it for their specific needs. This process consumes significantly more time and effort compared to reading content directly in their native language.

To address this inconvenience, we propose "ENkosum: English-Korean Summarization Via Pyramid structure for MD summarization." ENkosum is designed to efficiently summarize multi-document content written in English into Korean. It aims to reduce the time complexity associated with traditional cross-lingual tasks, thus lowering the overall cost. Additionally, it enhances the accuracy of key point extraction, enabling precise and effective summarization. ENkosum is a solution that streamlines the process of accessing English content for non-native speakers and facilitates the efficient extraction of valuable information.

## Major Requirements

* python 3.8
* Pytorch 1.1
  
## Evaluation with Trained Models

## Model Training


## Code structure
.
├── run_EnkoSum40k.py
│
├── data
│   └── EnkoSum
│   │       ├── train.json
│   │       ├── val.json
│   │       └── test.json
│   └── XMediaSum40k
│           ├── train.json
│           ├── val.json
│           └── test.json
└── model_output

## Usage of ENKOSUM

```python
from transformers import AutoTokenizer
from longformer import LongformerEncoderDecoderForConditionalGeneration
from longformer import LongformerEncoderDecoderConfig

tokenizer = AutoTokenizer.from_pretrained('./EnKoSUM_model/')
config = LongformerEncoderDecoderConfig.from_pretrained('./EnKoSUM_model/')
model = LongformerEncoderDecoderForConditionalGeneration.from_pretrained(
            './EnKoSUM_model/', config=config)
```


## Model Results



