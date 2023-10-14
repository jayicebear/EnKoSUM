# EnKoSUM: English-Korean Summarization Via Pyramid structure for MD summarization 

![python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

## overview

## Major Requirements

## Evaluation with Trained Models

## Model Training

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



