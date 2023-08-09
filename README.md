# Key Information Extraction of Scanned Receipt Using PP-Structure of PaddleOCR
* Use of SROIE dataset

receipt
## Introduction

## Data Preparation

## Fine Tuning PP-Structure

* Prepare Environment
Using google colab
Colab Link: https://colab.research.google.com/drive/1Vm-o4nbitV5muoxlJJ03B0pAWqYYg5K_?usp=sharing
Cloning files from GitHub repositories
```
# Cloning GitHub repositories from PaddleOCR
!git clone https://github.com/PaddlePaddle/PaddleOCR.git
# Cloning GitHub repositories from KIE-on-scanned-receipt-
!git clone https://github.com/fahmi97rosli/KIE-on-scanned-receipt-.git
```
Download requirements and libraries to use PaddleOCR
```
# Download requirement
%cd PaddleOCR
!pip install -r requirements.txt
!pip install -r ppstructure/kie/requirements.txt
```
```
# Download paddleocr and paddlepaddle library
!pip install paddleocr -U
!pip install paddlepaddle
```
Download and check GPU with PaddlePaddle program
```
# Download GPU with PaddlePaddle program
!pip install paddlepaddle-gpu==2.4.0.post112 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/stable.html
```
```
# Check GPU availability
import paddle
paddle.utils.run_check()
```

* Loading Dataset
Data formatting for using PP-Structure
Dictionary file and label
Make directory and loading data
```
!mkdir train_data
%cd train_data
# download and uncompress the dataset
# SROIE data final
!wget https://www.dropbox.com/s/wvgcv4czqyfpako/wildreceipt.tar?dl=0 && tar -xf wildreceipt.tar?dl=0
```

* Fine Tuning Model

## Testing Model
