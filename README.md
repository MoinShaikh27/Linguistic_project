# Linguistic_project
Semantic Textual Relatedness being a superset of the Semantic Textual Similarity task, is a much more complicated task and its solution would significantly improve a lot of downstream NLP activities.

# Problem Definition
The problem involves predicting the semantic textual
relatedness (STR) of sentence pairs in the form
of real-valued scores specifying their closeness in
meaning between 0 (completely unrelated) and 1
(maximally related).

# Corpus/Data Description                    
| Language|  Training | Testing|
|---------|:----------|--------:|
|English |5500 |2600|
|Marathi |1200 |300|
|Telugu |1170| 300|
|Augmented Hindi |7870 |3200|

|Languauge| count| mean| min |max|
|--------|:------|:-----|:------|:---|
|English |5500 |0.50 |0.00| 1.0|
|Marathi| 1200| 0.47 |0.03 |1.00|
|Telugu |1170 |0.49| 0.08 |0.88|
|Augmented Hindi|5500| 0.50 |0.00 |1.00|

# Model Finetuned For this task
|E5| LaBSE| XLNet| IndicBERT| IndicSBERT|

#Results After Finetune
### Performance post finetuning XLNet,indic-BERT with whole English and Hindi training dataset
over 3 epochs
| Model           | MSE  | Spearman correlation coefficient |
|-----------------|------|----------------------------------|
| XLNet (English) | 0.02 | 0.81                             |
| XLNet (Hindi)   | 0.03 | 0.12                             |
| Indic-BERT (English) | 0.02 | 0.81                        |
| Indic-BERT (Hindi)   | 0.02 | 0.75                        |
| IndicSBERT       |           |  0.801                     |

### Performance post finetuning E5, LaBSE with only Augmented Hindi sentences in the training dataset over 3 epochs.
| Model | Discrete Labels | Continuous Labels |
|-------|-----------------|-------------------|
| E5    | 0.86            | 0.81              |
| LaBSE | 0.86            | 0.80              |


### Performance post finetuning E5,LaBSE with multilingual training dataset over 3 epochs
| Model      | Discrete Labels | Continuous Labels |
|------------|-----------------|-------------------|
| E5[3]      | 0.86            | 0.82              |
| LaBSE[3]   | 0.85            | 0.79              |





