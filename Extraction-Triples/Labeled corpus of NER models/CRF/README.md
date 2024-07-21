# Introduction of model CRF

## Linkage
The source linkage of git：https://github.com/scofield7419/sequence-labeling-BiLSTM-CRF

## environmental requirements
- OS：Ubuntu 20.04
- Python version：3.7
- Dependencies：
  - tensorflow==1.15.2
  - numpy==1.15.4
  - pandas==0.20.3
  - Django==1.11.29
  - jieba==0.39

1. clone：
    ```bash
    git clone https://github.com/scofield7419/sequence-labeling-BiLSTM-CRF.git
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
    请按照个人需求进行下载
    
## Experiment
1. Run the model：
    ```bash
    python main.py
    ```
2. Remark:  For files and parameter settings, please see the system.config
