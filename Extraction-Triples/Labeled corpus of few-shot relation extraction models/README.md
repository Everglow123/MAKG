# Introduction of model FewRel

## Linkage
The source linkage of git：https://github.com/thunlp/FewRel

## environmental requirements
- OS：Ubuntu 20.04
- Python version：3.7
- Dependencies：
  - torch==1.10
  - transformers
  - numpy
  - tqdm 

1. clone：
    ```bash
    git clone git：https://github.com/thunlp/FewRel.git
    cd yourproject
    ```

2. create environment&activate：

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

## Data Preparation
1. Download Dataset：
   The names of our dataset are listed as follows.
    The partition ratio is 73
    The partition ratio is 82
    The partition ratio is 91
    
## Experiment
1. Finetune the model：
    ```bash
    python train_demo.py
    ```
2. Remark:  For files and parameter settings, please see the train_demo.py