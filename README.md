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
@inproceedings{zhu-hudelot-2022-towards,
    title = "Towards Job-Transition-Tag Graph for a Better Job Title Representation Learning",
    author = "Zhu, Jun  and
      Hudelot, Celine",
    booktitle = "Findings of the Association for Computational Linguistics: NAACL 2022",
    month = jul,
    year = "2022",
    address = "Seattle, United States",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.findings-naacl.164",
    doi = "10.18653/v1/2022.findings-naacl.164",
    pages = "2133--2140",
    abstract = "Works on learning job title representation are mainly based on \textit{Job-Transition Graph}, built from the working history of talents. However, since these records are usually messy, this graph is very sparse, which affects the quality of the learned representation and hinders further analysis. To address this specific issue, we propose to enrich the graph with additional nodes that improve the quality of job title representation. Specifically, we construct \textit{Job-Transition-Tag Graph}, a heterogeneous graph containing two types of nodes, i.e., job titles and tags (i.e., words related to job responsibilities or functionalities). Along this line, we reformulate job title representation learning as the task of learning node embedding on the \textit{Job-Transition-Tag Graph}. Experiments on two datasets show the interest of our approach.",
}



