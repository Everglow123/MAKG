# Introduction of model UIE

## Linkage
The source linkage of git：https://github.com/universal-ie/UIE

## environmental requirements
- OS：Ubuntu 20.04
- Python version：3.7
- Dependencies：
  - torch>=1.10,<2.0
  - transformers>=4.18,<5.0
  - numpy>=1.21
  - packaging
  - tqdm
  - sentencepiece
  - protobuf==3.19.0
  - onnxruntime  

1. clone：
    ```bash
    git clone git：https://github.com/universal-ie/UIE.git
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
1. Finetune the model：
    ```bash
    python finetune.py -t data/train.txt -d data/dev.txt -b 16 --save_dir ./checkpoint/model
    ```
    Remark:  For files and parameter settings, please see the finetune.py

2. Evaluate the model：
    ```bash
    python evaluate.py     --model_path ./checkpoint/model_best     --test_path ./data/dev.txt
    ```
    Remark:  For files and parameter settings, please see the evaluate.py
