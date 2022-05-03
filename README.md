# Introduction

This repository contains code for our paper [Towards Job-Transition-Tag Graph for a Better Job Title Representation Learning](https://openreview.net/forum?id=d8xNE_8SsR-) accepted by Findings of NAACL 2022. Our implementation is based on the [DGL package](https://www.dgl.ai/):



# Requirements

Python packages required:
- Python 3.7
- PyTorch 1.11.0
- dgl
- scikit-learn

# Dataset
## CareerBuilder12 (CB12) 
- Raw data downloaded from (https://www.kaggle.com/competitions/job-recommendation/data) 
- Raw job transition data obtained from ```user_history.tsv```
- Job title label assignment used [O*Net-SOC AutoCoder](https://www.onetsocautocoder.com/)

### Steps of generating graph ###
- Generating job transition data: An example is given in ```1.Prepare/1.Prepare_transition_cb12.ipynb```
- Preprocessing job title and generating tags: An example is given in ```1.Prepare/2.Preprocessing_cb12.ipynb```
- Prepare graph files for homogeneous or heterogeneous graph: An example is given in ```1.Prepare/3.Create_graph_*.ipynb```

# Job classification
- Examples are given in ```2.Node_classification```


# Reference
Please cite our paper if you use our data or code:



