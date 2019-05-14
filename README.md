# Analyzing the Impact of Language Models for Portuguese Named Entity Recognition


State-of-The-Art results


Results for the Total Scenario (HAREM)

| Approach   |    Precision   | Recall |   F1   |
|:----------:|:--------------:|:------:|:------:|
| BiLSTM-CRF+FlairBBP |     **74.91%**     | **74.37%** | **74.64%** |
| BiLSTM-CRF [(Castro, et al.)](https://www.researchgate.net/publication/326301193_Portuguese_Named_Entity_Recognition_using_LSTM-CRF) |     72.28%     | 68.03% | 70.33% |
|   CharWNN [(dos Santos, et al.)](https://arxiv.org/pdf/1505.05008.pdf)  |     67.16%     | 63.74% | 65.41% |



Results for the Selective Scenario (HAREM)

| Approach   |    Precision   | Recall |   F1   |
|:----------:|:--------------:|:------:|:------:|
| BiLSTM-CRF+FlairBBP|       **83.38%**       | **81.17%** | **82.26%** |
| BiLSTM-CRF [(Castro, et al.)](https://www.researchgate.net/publication/326301193_Portuguese_Named_Entity_Recognition_using_LSTM-CRF) |       78.26%       | 74.39% | 76.27% |
|   CharWNN [(dos Santos, et al.)](https://arxiv.org/pdf/1505.05008.pdf) |       73.98%       | 68.68% |    65.41%    |

## Language Models

### Flair Embeddings - FlairBBP
You can download our Flair Embeddings models (FlairBBP) in the following links:
* **Backward:** [FlairBBP-Backward](http://grupopln.inf.pucrs.br/health/flairBBP_backward-pt.pt)
* **Forward:** [FlairBBP-Forward](http://grupopln.inf.pucrs.br/health/flairBBP_forward-pt.pt)

### Word Embeddings
You can download our Word Embedding models in the following links, note that all models were trained in 300 dimensions:


| Algorithm  | Architecture | Downloads |
| ------------- | ------------- | ------------- |
| Word2Vec  | Skip-Gram  | [Word2Vec_skpg_300d](http://grupopln.inf.pucrs.br/health/bbp_word2vec_skpg_300d.zip) |
| Word2Vec  | CBOW  | [Word2Vec_cbow_300d](http://grupopln.inf.pucrs.br/health/bbp_word2vec_cbow_300d.zip) |
| FastText   | Skip-Gram  | [Fasttext_skpg_300d](http://grupopln.inf.pucrs.br/health/bbp_fasttext_skpg_300d.zip) |
| FastText   | CBOW  | [Fasttext_cbow_300d](http://grupopln.inf.pucrs.br/health/bbp_fasttext_cbow_300d.zip) |


### NILC Word Embeddings
You can download the Word Embeddings provided by NILC in the following link: http://nilc.icmc.usp.br/embeddings

## Language Models Corpora

### BlogSet-BR
BlogSet-BR is a large corpus built from millions of sentences taken from Brazilian Portuguese web blogs.
* Paper: BlogSet-BR: A Brazilian Portuguese Blog Corpus [(Santos, et al.)](http://www.lrec-conf.org/proceedings/lrec2018/summaries/10.html)
* [Download Here!](http://www.inf.pucrs.br/linatural/wordpress/recursos-e-ferramentas/blogset-br/)

### brWaC
brWaC is another portuguese large corpus.
* Paper: The brWaC Corpus: A New Open Resource for Brazilian Portuguese[(Filho, et al.)](https://www.researchgate.net/publication/326303825_The_brWaC_Corpus_A_New_Open_Resource_for_Brazilian_Portuguese)
* [Download Here!](http://www.inf.ufrgs.br/pln/wiki/index.php?title=BrWaC)

### ptwiki-20190301
ptwiki-20190301 is a corpus formed by texts from wikipedia in Portuguese.
* [Download Here!](https://dumps.wikimedia.org/ptwiki/20190301/)


Language Model Corpora Size Details (after pre-processing):

|      Corpus     |  Sentences  |     Tokens    |
|:---------------:|:-----------:|:-------------:|
|      brWaC      | 127,272,109 | 2,930,573,938 |
|    BlogSet-BR   |  58,494,090 | 1,807,669,068 |
| ptwiki-20190301 |  7,053,954  |  162,109,057  |
|   All Corpora   | 192,820,153 | 4,900,352,063 |
