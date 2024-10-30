# Deep Text Project

This project is in the scope of the course Deep Text at Unica. The aim of this project is to generate new dinosauer name given a dataset of existing dinosaur name. We have to implement 2 models:
1. The n-gram model
2. A deep learning model of any kind

We have implemented the two model. For n-gram we have implemented:
- unigram (1-gram)
- bigram (2-gram)
- trigram (3-gram)
- 4-gram
- 5-gram
- 6-gram

For a deep learning model we choose to implement a model that given a sequence of length __seq_len__ predict the next letter. The next letter can be [a-z] or special token \<END>. You would find more details about each method in the notebook.

In our work, we have special token \<START> and \<END> that represent respectively the start of a name and the end of a name. In prediction we feed \<START> to our model to start prediction and the model give us \<END> to indicates that it has finish generating the sequence.

## Structure of the project

```bash
.
├── data
├── model
└── plots
```
- `./data/` contains the dataset use for the project
- `./model/` contains the save of the weights of the deep learning model. You can load it instead of training it. You should just de-comment the appropriate cell in the jupyter notebook
- `./plots/` conatins all the plots generated

## Install dependencies

You should create a virtual environment and install python 3.10.5 and install dependencies with the command `pip install -r requirements.txt`


## References

[1] Medium, Code Diaries: Text Prediction (n-grams), https://medium.com/analytics-vidhya/code-diaries-text-prediction-n-grams-e3aa4d5325a2

[2] Medium, NLP : Génération de texte par n-grams, https://beranger.medium.com/nlp-génération-de-texte-par-n-grams-3894187f6cd4

[3] Medium, N-grams in NLP, https://medium.com/@abhishekjainindore24/n-grams-in-nlp-a7c05c1aff12

[4] Obscure Dinosaur Facts, https://obscuredinosaurfacts.com/blog/post/2019/09/05/dinosaur-word-roots.html