# Introduction of model SpERT

## Linkage
The source linkage of git：https://github.com/lavis-nlp/spert

## environmental requirements
- OS：Ubuntu 20.04
- Python version：3.7
- Dependencies：
  - Jinja2==2.11.3
  - numpy==1.17.4
  - tensorboardX==1.6
  - torch==1.4.0
  - tqdm==4.55.1
  - transformers[sentencepiece]==4.1.1
  - scikit-learn==0.24.0
  - spacy==3.0.1
  
1. clone：
    ```bash
    git clone https://github.com/lavis-nlp/spert.git
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
    python main.py
    ```
2. Remark:  For files and parameter settings, please see the config/train or config/test
