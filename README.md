This repository provides implementation of our paper **SF-PATE: Scalable, Fair, and Private Aggregation of Teacher Ensembles**

## 1. Introduction
The project is to develope a scalable private fair training framework that aims to protect the group labels of training data. The motivation of the paper comes from the limitation of previous work. For example, PF-LD which has  showed significant improvement over baseline methods but could not be scalable on huge data or infeasible to be trained on very deep networks such as Resnet50. 

To overcome these limitations, we provide two private fair training framework based on PATE. See more at Papernot, et al, Semi-supervised Knowledge Transfer for Deep Learning from Private Training Data
The short description of two proposed models are follows:
- SF<sub>S</sub>-PATE: Each teacher will be classifier to predict the group labels A here. The ensembler of these teachers will provide group labels via a private channel (e.g., GNMAX) to a student. The student will be a fair models over these private group labels. 

- SF<sub>T</sub>-PATE: Each teacher will be a fair classifier but to predict the class labels Y here. The fairness knowledge of these teachers can be transfered to students via their predictions. For this model, the student just need to be a regular classifier.

## 2. Codes


## 3. Datasets

- We uploaded all tabular datasets into folder `./data`.  All tabular datasets were already pre-processed (e.g, standardlization) for immediate usage. 
- Regarding UTKFace, we clone the dataset directly from the following [UTKFace repo](https://github.com/aicip/UTKFace)

## 4. Requirements
- We ran all experiments on Python 3.7, Pytorch 1.10.
- To compute the spent privacy budget in PATE and PF-LD, we use the [tensorflow_privacy repo](https://github.com/tensorflow/privacy)  

