# **Information Extraction**

This project aims to gain insight into problematic maintenance areas in the interior sections of aircraft by examining logbook records which contain issues that are not self-reporting, i.e. not maintenance messages or flight-deck effects.  The original premise is to get better "electronic eyes" on the problems and areas, the solution being dubbed "Tetrachrome" after Tetrachromacy, the ability to distinguish many more colors than would typically be viewed by normal human eyes.


The project at this point consists of the original experimentation on DISC_CMPLNT_TX (Complaint) from Logbook and further experimentation on MAINT_ACT_TX (Action) from Logbook.  

-----
- [Overview](#overview)
- [NER Tagging Rules](docs/taggingRule.md)
- [Project setup (To Be Finished)]()
- [Proposal](docs/proposal.pdf)
- [Baseline](docs/LSTM-CRF-Ensemble/Scores.md)

-----

## Overview
### **Phase 1: Pretrained Word Embedding (CMU)**

Pre-train word embedding from both word and character level, performed as input features for LSTM-CRF Ensemble Model. This phase is implemented separately from LSTM-CRF Ensemble Model, using LSTM and CNN, unsupervised evaluated by perplexity.
 
- [Pretrained Word Embedding](docs/wordEmbedding/README.md)


### **Phase 2: LSTM-CRF Ensemble Model (Boeing)**

Implement LSTM model with CRF layer on the most top. Given pre-trained word embedding, feed into bi-directional LSTM to generate independent tagging probabilities, then combine CRF Features (domain knowledge) into LSTM Model. Use Forward/Backward Table to combine LSTM  and CRF probabilities to give a sentence based NER prediction.

- [LSTM-CRF-Ensemble](docs/LSTM-CRF-Ensemble/README.md)