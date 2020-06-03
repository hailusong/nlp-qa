# NLP QA and more

## Options
### Intent Classification
| Model | Action | Data | How to use it |
| ----- | ---- | ---- | ------ |
| pre-trained BERT | Add classification head and fine-tune | domain data | Use the fine-tuned model to test the target data set |
| pre-trained BERT | Continuous learning with domain data | public legal document data | BERT language model trained on domain data |
| pre-trained BERT model on domain data |  Add classification head and fine-tune | domain data | Use the fine-tuned model to test the target data set |

### QA
| Model | Action | Data | How to use it |
| ----- | ---- | ---- | ------ |
| pre-trained BERT | Add QA head and fine-tune | SQuAD 1.1 dataset | Use the fine-tuned model to test the target data set |
| pre-trained BERT with QA head | | | Use the pre-trained QA model to test the target data set |
| pre-trained BERT | Continuous learning with domain data | public legal document data | BERT language model trained on domain data |
| pre-trained BERT model on domain data |  Add QA head and fine-tune | SQuAD 1.1 dataset | Use the fine-tuned model to test the target data set |

### Fine-tune Resourcing
1. According to [**HuggingFace SQuAD readme**](https://github.com/huggingface/transformers/tree/master/examples/question-answering)
  - fine-tunes BERT on the SQuAD1.0 dataset ...
  - completed in 24 min (with BERT-base) or 
  - 68 min (with BERT-large) ...
  - on a single tesla V100 16GB

## Data Enriching
1. By page
2. By paragraph
