# Universal Language Model Fine-tuning (ULMFiT) for Text Classification

## Motivation 
#### Before inventing universal language model fine-tuning, existing approaches in NLP still require task-specific modifications and training from scratch

#### Q1: What are the disadvantages of those approaches? (hint: time and resource)

## How ULMFit solve above problems
#### ULMFiT is an effective transfer learning method that can be applied to any task in NLP. Transfer learning is a machine learning method where a model developed for a task is reused as the starting point for a model on a second task.
<img src='Figure/transfer_learning.png' width='500'>

#### The specific logic of applying transfer learning in ULMFiT is pretraining a language model (LM) on a large general-domain corpus and fine-tunes it using the data of target task

## Architecture
<img src='Figure/ULMFiT.png' width='800'>
