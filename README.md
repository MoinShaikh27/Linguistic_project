# Linguistic_project
Semantic Textual Relatedness being a superset of the Semantic Textual Similarity task, is a much more complicated task and its solution would significantly improve a lot of downstream NLP activities.

# Problem Definition
The problem involves predicting the semantic textual
relatedness (STR) of sentence pairs in the form
of real-valued scores specifying their closeness in
meaning between 0 (completely unrelated) and 1
(maximally related).

## Corpus/Data Description                    
| Language|  Training | Testing|
|---------|:----------|--------:|
|English |5500 |2600|
|Marathi |1200 |300|
|Telugu |1170| 300|
|Augmented Hindi |7870 |3200|

Languauge count mean min max
English 5500 0.50 0.00 1.0
Marathi 1200 0.47 0.03 1.00
Telugu 1170 0.49 0.08 0.88
Augmented
Hindi
5500 0.50 0.00 1.00

# Model Finetuned
E5
LaBSE
XLNet
IndicBERT
IndicSBERT
