# Introduction of model BERT+BiLSTM+CRF

## Linkage
The source linkage of git：https://github.com/kingglory/BERT-BILSTM-CRF-NER-Pytorch-Chinese

## environmental requirements
- OS：Ubuntu 20.04
- Python version：3.7
- Dependencies：
  - torch==1.8.0
  - pytorch_crf==0.7.2
  - numpy==1.17.0
  - transformers==4.9.0
  - tqdm==4.62.0
  - PyYAML==5.4.1
  - tensorboardX==2.4
  
1. clone：
    ```bash
    git clone https://github.com/kingglory/BERT-BILSTM-CRF-NER-Pytorch-Chinese.git
    cd yourproject
    ```

2. create environment&activate：

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3. install Dependencies：

    ```bash
    pip install -r requirements.txt
    ```

## Data Preparation
1. Download Dataset：
   The names of our dataset are listed as follows.
    The partition ratio is 73
    The partition ratio is 82
    The partition ratio is 91
    
## Experiment
1. Run the model：
    ```bash
    cd torch_ner/source/
    python train.py
    ```
2. Remark:  For files and parameter settings, please see the config.py
