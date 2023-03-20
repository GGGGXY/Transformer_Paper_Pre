# Universal Language Model Fine-tuning (ULMFiT) for Text Classification

## 1. Motivation 
#### Before inventing universal language model fine-tuning, existing approaches in NLP still require task-specific modifications and training from scratch

#### Q1: What are the disadvantages of those approaches? (hint: time and resource)

## 2. How ULMFit solve above problems
#### ULMFiT is an effective transfer learning method that can be applied to any task in NLP. Transfer learning is a machine learning method where a model developed for a task is reused as the starting point for a model on a second task.
<img src='Figure/transfer_learning.png' width='500'>

#### The specific logic of applying transfer learning in ULMFiT is pretraining a language model (LM) on a large general-domain corpus and fine-tunes it using the data of target task 
##### 1. Faster only needs to adapt to the idiosyncrasies of the target data
##### 2. Robust LM even for small datasets

## 3. Architecture
<img src='Figure/ULMFiT.png' width='800'>

#### ULMFiT consists of three stages:
##### 1. General-domain LM pretraining
##### 2. Target task LM fine-tuning
##### 3. Target task classifier fine-tuning

## 3.1 Stage one: General-domain LM pretraining
#### In this stage, the LM is trained on a general-domain corpus to capture general features of the language.
#### 1. Wikitext-103 consisting of 28595 preprocessed Wikipedia articles and 103 million words.
#### 2. This stage only needs to be performed once and improves preformance and convergence of downstream models. 
