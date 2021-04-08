# NARRE

This is the implementation for the paper:



*Chong Chen, Min Zhang, Yiqun Liu, and Shaoping Ma. 2018. [Neural Attentional Rating Regression with Review-level Explanations.](http://www.thuir.cn/group/~YQLiu/publications/WWW2018_CC.pdf) 
In WWW'18.*

**Please consider to cite the paper if you use its codes.**

```
@inproceedings{chen2018neural,
  title={Neural Attentional Rating Regression with Review-level Explanations},
  author={Chen, Chong and Zhang, Min and Liu, Yiqun and Ma, Shaoping},
  booktitle={Proceedings of the 2018 World Wide Web Conference on World Wide Web},
  pages={1583--1592},
  year={2018},
}
```

Author: Chong Chen (cstchenc@163.com)

## Environments

- python 2.7
- Tensorflow (version: 0.12.1)
- numpy
- pandas


## Dataset

The author, in his experiments, used the datasets from Amazon 5-core(http://jmcauley.ucsd.edu/data/amazon) and Yelp Challenge 2017(https://www.yelp.com/dataset_challenge).
In mine, I used a personal dataset built ad hoc by my repo [URB-RS](https://github.com/AndreaMercanti/URB-RS.git) and set it in the `data/film` folder, previously made. 
Besides, the codes use a Google's vector of pretrained words weights, so download and unzip it in the `data` folder from [here](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit).
Then change its name simply into `google.bin` and you're ready to go!

## Example to run the codes

The folowing commands must be run from the root folder `NARRE`.

```
mkdir data/film
```

Data preprocessing:

```
cd pro_data
python loaddata.py	
python data_pro.py
```

Train and evaluate the model:

```
cd model
python train.py
```


Last Update Date: April 8, 2021
