# Real-time Classification and Span-based Detection of Comments on Facebook Sales Posts
## Introduction
We build a data set ViCCSP for the comment classification problem based on user intent, along with the ViSDC dataset for named entity recognition task. The ViCCSP dataset includes five labels (question, order, judge, spam, other), collected from sales posts in social networking groups on Facebook. The ViSDC dataset consists of four entities (phone number, quantity, product, and address). We build real-time systems for streaming data collection, training, and visualization. In this paper, we use Kafka language models for system implementation. PhoBERT-base gives the highest results in task 1 (comment classification), reaching 91.15\% for measuring accuracy and 87.24\% for measuring F1 scores. For task 2 (NER), XLM-RoBERTa-large gives the highest results, reaching 96.03\% - accuracy, 94.37\% - F1 at the word level, 94.77\% - accuracy, 89.39\% - F1 at the span level, 82.88\%-strict. In addition, we have implemented the system and satisfied the users.
## Example
### ViCCSP dataset 
<img width="1118" alt="ViCCSP_example" src="https://github.com/the-ntg/ViCCSP-ViSDC/assets/109457460/277ec5f1-81c6-4a5c-875f-354cf9f6c880">

### ViSDC dataset

<img width="693" alt="ViSDC_example" src="https://github.com/the-ntg/ViCCSP-ViSDC/assets/109457460/70ab6c9b-43dd-4074-8b11-63a754b48133">

## Model Performance
### ViCCSP
|Model | F1-score | Accuracy |
|--------------|----------|----------|
| `PhoBERT-base` | `87.24` | `91.15` |
| XLM-R-base | 84.11 | 88.92 | 
| mBERT-base-cased  | 83.96 | 88.43 |
| BERT-base-uncased  | 80.91 | 87.53 |
| BERT-base-cased  | 79.34 | 86.06 |
| BERT-base  | 79.34 | 86.06 |


### ViSDC
|Model | F1-score | Accuracy |
|--------------|----------|----------|
| XLM-RoBERTa-large | 94.04 | 87.09 |
| XLM-RoBERTa-base | 94.97 | 87.54 | 
| `ViSoBERT`  | `94.77` | `89.39` |
| mBERT-base-uncased  | 94 | 86.92 |
| ViBERT  | 93.46 | 85.39 |
| ViDeBERTa-base  | 84.35 | 62.55 |

## Contact
Authors:
Tam Huu Minh Nguyen, Tinh Pham Phuc Do, Ngoc Dinh Duy Cao, The Tran Gia Nguyen, and Trong-Hop Do

Faculty of Information Science and Engineering, University of Information Technology, Ho Chi Minh City, Vietnam

Vietnam National University, Ho Chi Minh City, Vietnam

{20521871,20522020,20521661,20521940}@gm.uit.edu.vn and hopdt@uit.edu.vn
