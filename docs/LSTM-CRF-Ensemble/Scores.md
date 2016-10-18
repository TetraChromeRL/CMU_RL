# Scores

Metric of 5-fold cross validation to extract **COMPONENT**, **LOCATION**, **CONDITION**, **ACTION**, **RESULT** from logbook data ATA24 using **LSTM-CRF-Ensemble** with Word Embedding within Boeing. We will treat them as Baseline for CMU Word Representation team, for experiments on further improvement.

-----

- [ATA24 Complaint](#1-ata-24-complaint-lstm-crf-ensemble-crf-weight-04)
- [ATA24 Action](#2-ata-24-action-lstm-crf-ensemble-crf-weight-04)

-----

## 1.  ATA 24 Complaint (LSTM-CRF-ENSEMBLE (CRF Weight = 0.4))
||FOLD 1|FOLD 2|FOLD 3|FOLD 4|FOLD 5|AVG|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|Component Precision|0.88615|0.92515|0.95531|0.90428|0.92050|0.91828|
|Component Recall|0.93905|0.91951|0.90476|0.92169|0.91595|0.92019|
|Component F1|0.91184|0.92232|0.92935|0.91291|0.91822|0.91893|
|||||||||
|Location Precision|0.90753|0.92135|0.91873|0.93227|0.93115|0.92221|
|Location Recall|0.92013|0.87544|0.90278|0.84173|0.90735|0.88949|
|Location F1|0.91379|0.89781|0.91068|0.88469|0.91909|0.90521|
|||||||||
|Condition Precision|0.85377|0.82726|0.87643|0.78311|0.88608|0.84533|
|Condition Recall|0.79560|0.81321|0.83442|0.81087|0.82677|0.81617|
|Condition F1|0.82366|0.82017|0.85491|0.79675|0.85540|0.83018|
|||||||||
|TOTAL F1|0.88310|0.88010|0.89831|0.89478|0.89757|0.89077|

## 2.  ATA 24 Action (LSTM-CRF-ENSEMBLE (CRF Weight = 0.4))
||FOLD 1|FOLD 2|FOLD 3|FOLD 4|FOLD 5|AVG|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|Component Precision|0.91915|0.93323|0.92084|0.91995|0.89710|0.91805|
|Component Recall|0.93426|0.91791|0.92206|0.91570|0.91153|0.92029|
|Component F1|0.92665|0.92551|0.92145|0.91782|0.90426|0.91914|
|||||||||
|Location Precision|0.96889|0.93488|0.94309|0.95964|0.93489|0.94828|
|Location Recall|0.91213|0.93489|0.88889|0.85600|0.85169|0.88872|
|Location F1|0.93966|0.93488|0.91519|0.90486|0.89135|0.91719|
|||||||||
|Condition Precision|0.78543|0.78715|0.78495|0.67945|0.79916|0.76723|
|Condition Recall|0.70290|0.70758|0.67385|0.72941|0.57357|0.67746|
|Condition F1|0.74187|0.74525|0.72517|0.70355|0.66783|0.71673|
|||||||||
|Action Precision|0.89749|0.89819|0.88140|0.86613|0.86920|0.88248|
|Action Recall|0.86214|0.82881|0.84787|0.84387|0.81159|0.83886|
|Action F1|0.87946|0.86211|0.86431|0.85485|0.83940|0.86003|
|||||||||
|Result Precision|0.80631|0.85806|0.85350|0.83710|0.75833|0.82266|
|Result Recall|0.79556|0.71123|0.67337|0.79741|0.71937|0.73939|
|Result F1|0.80089|0.77778|0.75281|0.81678|0.73834|0.77732|
|||||||||
|TOTAL F1|0.85771|0.84910|0.83578|0.83957|0.80824|0.83808|
