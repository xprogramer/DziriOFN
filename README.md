# DziriOFN Corpus (Dziri Offensive corpus) v1.0

Dziri refers to the name of the Algerian dialectal Arabic. DziriOFN is a new corpus dedicated to offensive language detection on this under-resourced language. Dziri dialect if known as a complex socio-linguistic situation, where the latter is known by the code-switching phenomenon and borrowed words from several languages (e.g. Turkish, Berber, French, Spanish, etc.). The corpus is crawled from Facebook social media, because the latter is the common used social media network by the Algerian community. In overall, the corpus contains 8.7k texts manually annotated as normal, offensive and abusive, where it was annotated by five different native speakers. The texts are written in Arabic script, and some of them are written in Latin script (i.e. Arabizi).


Table 1. DziriOFN corpus description

|  | #texts |
| ------------- | ------------- |
| offensive texts | 3,227 |
| abusive texts | 1,334 |
| normal texts | 4,188 |
| total | 8,749 |


Table 2. Inter-agreement annotation between different annotators

| Category | 1st vs 2nd | 1st vs 3rd | 2nd vs 3rd |
| ------------- | ------------- | ------------- | ------------- |
| offensive | 2,341 | 583 | 305 |
| normal | 3,449 | 3,603 | 4,008 |
| abusive | 1,108 | 85 | 141 |

In Table 2, the 3rd, 4th and 5th annotators are considered as a single annotator (3rd annotator). For more details, check the technical article.

# Evaluation

We have experimented with some ML and DL classifiers as a baseline using two-labels (abusive and offensive merged together) and three-labels.


Table 3. Test results of ML models trained with two and three labels.

| | SVM | Multinomial NB |
| ------------- | ------------- | ------------- |
| two-class | 0.744 | 0.752 |
| three-class | 0.669 | 0.662 |

Table 4. Test results of DL models trained with two and three labels.

| | CNN | BiLSTM | FastText |
| ------------- | ------------- | ------------- | ------------- |
| two-class | 0.523 | 0.520 | 0.716 |
| three-class | 0.347 | 0.400 | 0.648 |


# Citation

Boucherit, O., & Abainia, K. (2022). Offensive Language Detection in Under-resourced Algerian Dialectal Arabic Language. arXiv preprint arXiv:2203.10024.
