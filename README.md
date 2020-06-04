# NLP QA and more
A combination of techniques like
- Intent classification, to classify the intent(s) of the documents
- QA, to extract parameters
- NER, to highlight all Nouns

Also, worthy trying out
- Summaization -> Intent classification

## Options
### Intent Classification
| Model | Action | Data | How to use it |
| ----- | ---- | ---- | ------ |
| pre-trained ALBERT (albert-xxlarge-v2) | fine-tune with classification head | domain dataset with intent labels | Split domain dataset into dev/test and verify accuracy  |

### QA
| Model | Action | Data | How to use it |
| ----- | ---- | ---- | ------ |
| pre-trained ALBERT with QA head on SQuAD2 | | | Use the pre-trained QA model to test the target data set |

### DIY Fine-Tuning
1. Soures
    - According to [**HuggingFace SQuAD readme**](https://github.com/huggingface/transformers/tree/master/examples/question-answering)
2. Fine-tunes BERT on the SQuAD1.0 dataset, BERT-base

| Environment | Speed (s/it) | Total Time |
| ----------- | ------------ | ---------- |
| TPU | - completed in 24 min (with BERT-base) or <br>- 68 min (with BERT-large) ...<br>- on a single tesla V100 16GB | |
| Colab GPU<br>(10GB GPU memory) | out-of-memory | |
| Colab TPU | 52.24s/it | 2 Epoch * 7387 iter * 52s = 214h |

        
## Data Enriching
1. By page
2. By paragraph
