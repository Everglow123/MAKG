# Introduction of model DeepKE

## Linkage
The source linkage of git：https://github.com/zjunlp/deepke

## environmental requirements
- OS：Ubuntu 20.04
- Python version：3.7
- Dependencies：
  - torch>=1.5,<=1.11
  - hydra-core==1.0.6
  - tensorboard==2.4.1
  - matplotlib==3.4.1
  - transformers==4.26.0
  
1. clone：
    ```bash
    git clone https://github.com/zjunlp/deepke.git
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
    cd example/re/standard
    python run.py
    ```
2. Remark:  For files and parameter settings, please see the conf
