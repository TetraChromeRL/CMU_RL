# **LSTM-CRF-Ensemble**

The goal of this investigation is to extract **COMPONENT**, **LOCATION**, **CONDITION**, **ACTION**, **RESULT** from logbook data using **LSTM-CRF-Ensemble** combined with CRF Features.

-----
- [Overview](#overview)
- [F1-Score, Precision, Recall](Scores.md)


-----

## Overview

### **Motivation**
#### a. Reason for Choosing LSTM
1.  Lack of domain-specific knowledge on doing feature engineering
2.  Small supervised training corpus
3.  Large unsupervised training corpus

#### b. Reason for Combining CRF Features
1. Deep learning can achieve good performance without handcraft features. It can automatically extract features from sentence context. 
2. However, without domain knowledge further improvement will be hard from model side. Further enhancement on model will increase model complexity. Considering exist dataset size, put more effort back to feature side will be efficient. 
3. We try to incorporate CRF features (mostly explored by Matt) into current LSTM-CRF model. Log linear model like CRF model offer us a good opportunity to add domain knowledge. 
4. We build a new combined model named LSTM-CRF Ensemble Based on these motivation


### Model Structure:
1.  Word embedding: capture spelling error etc. Use untagged data for pretrain.
2.  Bidirectional LSTM
3.  CRF layer instead of softmax. (relate previous tag and next tag rather than independent classification)
4.  In general: Word Embedding ---  Bidirectional LSTM --- CRF architecture

  
### **Experiment Data**

1. UAL ATA24 COMPLAINT
2. UAL ATA24 ACTION

### **Experiment Goal for CMU Word Embedding Team**
  Test whether there is a significant improvement using new Word Embedding technique


