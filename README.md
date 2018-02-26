# Machine Learning Practical

This repository contains the code and report for the work done on top of codebase from the University of Edinburgh [School of Informatics] course [Machine Learning Practical]

This assignment-based course is focused on the implementation and evaluation of machine learning systems. It works on Convulation Neural Network with VGG model on CIFAR-10 and CIFAR-100 dataset.

Transfer learning has proven itself to be an incredibly useful area in deep learning, not only by facilitating those with limited access to resources such as data and time, but also by driving a deeper understanding of neural network features in general. Like all areas of machine learning these methods come with their own set of difficulties and heuristic methods in tow. In this paper we shall motivate and further detail a project to investigate the use of Bayesian methods to automatically optimize these heuristically tuned parameters and potentially alleviate some of the methods well known symptoms.

The code in this repository is split into:
1. notebooks: 
    1. Introduction_to_tensorflow: Introduces students to the basics of tensorflow and lower level operations.
    2. Introduction_to_tf_mlp_repo: Introduces students to the high level functionality of this repo and how one 
    could run an experiment. The code is full of comments and documentation so you should spend more time 
    reading and understanding the code by running simple experiments and changing pieces of code to see the impact 
    on the system.
2. utils: 
    1. network_summary: Provides utilities with which one can get network summaries, such as the number of parameters and names of layers.
    2. parser_utils which are used to parse arguments passed to the training scripts.
    3. storage, which is responsible for storing network statistics.
3. data_providers.py : Provides the data providers for training, validation and testing.
4. network_architectures.py: Defines the network architectures. We provide VGGNet as an example.
5. network_builder.py: Builds the tensorflow computation graph. In more detail, it builds the losses, tensorflow summaries and training operations.
6. network_trainer.py: Runs an experiment, composed of training, validation and testing. It is setup to use arguments such that one can easily write multiple bash scripts with different hyperparameters and run experiments very quickly with minimal code changes.
    
    
