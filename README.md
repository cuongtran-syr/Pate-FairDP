This repository provides implementation of our paper **SF-PATE: Scalable, Fair, and Private Aggregation of Teacher Ensembles**

## 1. Introduction
The project is to develope a scalable private fair training framework that aims to protect the group labels of training data. The motivation of the paper comes from the limitation of previous work. For example, PF-LD which has  showed significant improvement over baseline methods but could not be scalable on huge data or infeasible to be trained on very deep networks such as Resnet50. 

## 2. Codes


## 3. Datasets

- We uploaded all tabular datasets into folder `./data`.  All tabular datasets were already pre-processed (e.g, standardlization) for immediate usage. 
- Regarding UTKFace, we clone the dataset directly from the following [UTKFace repo](https://github.com/aicip/UTKFace)

## 4. Requirements
- We ran all experiments on Python 3.7, Pytorch 1.10.
- To compute the spent privacy budget in PATE and PF-LD, we use the [tensorflow_privacy repo](https://github.com/tensorflow/privacy)  

