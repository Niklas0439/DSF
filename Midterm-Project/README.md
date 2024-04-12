# Machine Learning Project: Kinase Activity Prediction

## Introduction

This project aims to develop a machine learning model to predict the activity of kinase enzymes based on publicly available data. Kinases play a crucial role in various cellular processes, and their dysregulation has been implicated in various diseases, making them an important target for drug discovery efforts.

## Project Goals

1. **Learn about Machine Learning**: Gain theoretical knowledge and practical experience in machine learning concepts, algorithms, and techniques.

2. **Learn about Basic Linux Usage**: Develop proficiency in using Linux operating systems, which are widely used in scientific computing and data analysis.

3. **Explore Resources at UniBe**: Familiarize yourself with the resources available at the University of Bern (UniBe) for conducting computational research projects.

4. **Build a Kinase Activity Prediction Model**: Utilize publicly available data to train and validate a machine learning model capable of predicting the activity of kinase enzymes based on their structural and chemical properties.

## Getting Started

### 1. Read and run the Tutorial

The tutorial to be followed is [TeachOpenCADD](https://projects.volkamerlab.org/teachopencadd/talktorials/T022_ligand_based_screening_neural_network.html).

The used training set differs from the one used in the tutorial and is provided by the [DSF Course](https://cloud-new.gdb.tools/index.php/s/ZfZM7itQf3rm6Sw).

The Tutorial was run and documented in a [Jupyter Notebook](Tutorial.ipynb)

#### **Questions regarding the Tutorial:**

- **What is in the training set, how big is it?** The training set consists of approximately 125,000 data points from the kinase dataset, which represents 70% of the total data.

- **What modifications do you need to do to the data set to perform the tutorial?** To perform the tutorial, modifications need to be made to the dataset. pIC50 values need to be calculated as only IC50 values are provided. Infinite pIC50 values (where IC50 was 0) need to be replaced with NaN values.

- **What is a test set?** A test set is a portion of the dataset that is held out from the training process and used exclusively to evaluate the performance of a machine learning model. Here we used 30% of the total data. It is used to assess how well the trained model generalizes to new, unseen data by comparing the model's predictions on the test set with the actual labels or outcomes.

- **Are there any other data sets?** Besides the test set, a training set and a validation set are typically required.
    - **Training Set:** The training set is used to train the machine learning model. It consists of examples with known inputs and corresponding outputs. The model learns from this data to make predictions or decisions.

    - **Validation Set:** The validation set is used to fine-tune hyperparameters of the model and to prevent overfitting. It is typically used during the training process to evaluate the model's performance on data that it hasn't seen before. Different models or configurations can be compared based on their performance on the validation set. For this tutorial no validation set was provided. 

### 3. Access Ubelix HPC Cluster
Gain access to the Ubelix HPC cluster by following the [documentation](https://hpc-unibe-ch.github.io/).

To access the Cluster SSH is used. The used commands can be found [here](Midterm-Project/Ubelix/Documentation.ipynb)

#### **Questions regarding Ubelix:**

- **What is Ubelix?** Ubelix is the high performance computing (HPC) cluster at the University of Bern, consisting of approximately 320 compute nodes. It serves as a resource for researchers to conduct various computational tasks such as theses, projects, and research.

- **How do you gain access?** To gain access to Ubelix, one needs to have a Campus Account and activate it by sending a request through the provided [link](https://serviceportal.unibe.ch/hpc). Once the account is activated, users can establish an SSH connection to one of the submit nodes from within the university network.

- **Who can have access?** Access to Ubelix is available to anyone with a Campus Account, including students, staff, and external researchers collaborating with the University of Bern. External researchers can apply for a Campus Account to gain access to the cluster.

- **What resources are available there?** Ubelix provides both storage and computational resources for users. Additionally, it offers the capability to create workspaces to facilitate collaboration within research projects, enhancing the productivity and efficiency of collaborative efforts.

- **How do you submit a job?** Jobs can be submitted to Ubelix based on the [Slurm framework](https://slurm.schedmd.com/overview.html). The used code can be found [here](Midterm-Project/Ubelix).


### 4. Run Training on Ubelix
Modify the code from the tutorial to run the relevant part (training) on the Ubelix HPC cluster. 

The Python code, subission script and output can be found here [Ubelix](Ubelix)

