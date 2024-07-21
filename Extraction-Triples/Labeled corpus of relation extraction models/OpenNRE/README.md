# Introduction of model OpenNRE

## Linkage
The source linkage of git：https://github.com/thunlp/OpenNRE

## environmental requirements
- OS：Ubuntu 20.04
- Python version：3.7
- Dependencies：
  - torch==1.6.0
  - transformers==3.4.0
  - pytest==5.3.2
  - scikit-learn==0.22.1
  - scipy==1.4.1
  - nltk>=3.6.4
  
1. clone：
    ```bash
    git clone git：https://github.com/thunlp/OpenNRE.git
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
1. Run the model of bert：
    ```bash
    python example/train_bag_bert.py
    ```
    Remark:  For files and parameter settings, please see the example/train_bag_pcnn.py

2. Run the model of pcnn：
    ```bash
    python example/train_bag_cnn.py
    ```
    Remark:  For files and parameter settings, please see the example/train_bag_pcnn.py
