## A Neural Multi-digraph Model for Chinese NER with Gazetteers

This repository implements the multi-digraph model for incorporating gazetteers in Chinese NER. The dataset in the e-commerce domain and 7 NE gazetteers of products and brands are proposed.

## Requirement
Python 3.6, Pytorch >= 0.4, hb-config, dill, tqdm, numpy (or using pip -r requirements.txt)

## Usage
python -m src.main --config graph_ecommerce
turn on/off the gpu mode in config/graph_ecommerce.yml
remove gazetteers in config/graph_ecommerce.yml to run trivial GraphNER


To reproduce results in paper, you need to retrain and replace demo embeddings in data/embeddings (including char embedding and bichar embedding trained on Chinese wiki)
