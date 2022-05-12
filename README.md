This repository collects scripts for data preparation, training, inference and 
deploying **BERT** model using **AWS SageMaker**. 
Scripts can be used as a part of **SageMaker Pipelines** or as standalone, 
separately for data preparation, training and inference

Scripts are run via SageMaker notebooks. 

All scripts are stored in the `/scr` directory.

`config.json` - configuration file for BERT model. Uses for training and inference

`requirements.txt` - required packages for training and inference

`prepare_data.py` - data preparation scripts that clean data, split on train,  
validation, and test, and optionally store data to AWS FeatureStore

`train.py` - training script for train BERT model. By default, are used `roberta-base` 
model from huggingface. Any model can be used instead

`inference.py` - inference script
