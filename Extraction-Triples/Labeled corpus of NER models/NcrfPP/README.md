# Introduction of model NCRFpp

## Linkage
The source linkage of git：https://github.com/jiesutd/NCRFpp

## environmental requirements
- OS：Ubuntu 20.04
- Python version：3.7
- Dependencies：
  - torch==1.8.0
  
1. clone：
    ```bash
    git clone https://github.com/jiesutd/NCRFpp.git
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
1. Run the model：
    ```bash
    python main.py --config demo.train.config
    ```
2. Remark:  For files and parameter settings, please see the config/demo.train.config
