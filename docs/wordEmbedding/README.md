# **Word&Character Embedding**
The goal of this investigation is to use unsupervised corpus to train word embedding.

-----
- [Overview](#overview)
- [Baseline](#baseline)
- [Word Embedding Results](errAnalysis.md)


-----

## Overview

### **Embedding Training Data**

1.  **UAL logbook complaint data after 2012**

    **2,256,642** sentences, **673,615** vocabulary size

2.  **UAL logbook complaint data after 2012 reduce form**

    replace all numbers(**0-9**) with **0**
    
    **2,256,642** sentences, **209427** vocabulary size

## Baseline
###  Perplexity
   *  train data: **15.86**
   *  test data : **27.96** (PPL with Penn Treebank: **92.3**)

