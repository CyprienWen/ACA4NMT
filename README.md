# ACA4NMT
This is the code for our paper *Decoding History Based Adaptive Control of Attention for Neural Machine Translation*, https://arxiv.org/abs/1802.01812

## Preprocess
```
python3 preprocess.py -load_data path_to_data -save_data path_to_store_data 
```
Remember to put the data into a folder and name them *train.src*, *train.tgt*, *valid.src*, *valid.tgt*, *test.src* and *test.tgt*, and make a new folder inside called *data*

## Training
```
python3 train.py -log log_name -config config_yaml -gpus id
```

# Evaluation
```
python3 train.py -log log_name -config config_yaml -gpus id -restore checkpoint -mode eval
```
