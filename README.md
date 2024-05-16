# ML-Final
Final Project for CSCI 425 - Python Machine Learning

## Collaborators
Abraham Avila\
Klaus King

## Collaborators Contact
Author | Contact
 --- | --- 
 Abraham Avila | Email: aaavila@mavs.coloradomesa.edu
 Klaus King | Email: kmking2@mavs.coloradomesa.edu

## Abstract
In our Machine Learning Project, we will be exploring a variety of different machine learning 
solutions to well-established datasets from the Canadian Institute for Cybersecurity (CIC). Specifically, we will be examining the domain of malware where we will classify a malignant or benign program as well as defining what category of malware of the program if it is malicious. The preferred dataset that we will be using for these tasks is the CICMalMem-2022 made and provided by CIC. Methodology will be done by testing the machine learning algorithms to first classify a binary classification task (Benign vs. Malignant) before we test the machine learning models on classifying the types of malwares (Ransomware, Trojan, Spyware, vs. Benign). The goal with this project is to determine the performance of each model, and determine the champion model that performed the best from the sought-out tasks.

## Experiment Layout
To replicate the experiment from the proposed research, you will see that each model has their own directory which contains at least two jupyter-notebooks to run the experiment, where each notebook is running the same model but different task. For example, the XGBoost model should have two notebooks where one is a binary task (i.e. Class) and the other being multi-class (i.e. Category). There might be other notebooks within the same directory that are either their for furture reference for other projects or to show the learning process in creating these experiments. As for the other directories that are named after a specified model, these directories are to show the other parts of the project like Feature Engineering, documentation of tasks, and figures saved and used for the final paper within this repo. Now the most important aspect of this repo is the notebook called "report.ipynb", which is a juypter-notebook that runs each model on the cleaned dataset and makes graphics to help visualize the comparative performance for each model. Additionally, the other most important aspect that is included in this repo is the original paper proposing this dataset. We encourage the reader to look into this paper prior to running these experiments to get a good idea why we did the experiment the way we did. However, it is not reqired to read this paper in order to understand this experiment. We have included the dataset to this repo to allow those who are intereested in interacting or doing your own experiements with this dataset. Lastly, we have included a yaml-file to allow anyone who is interested in running these experiments to install this environment through the anaconda application or CLI. If on the CLI use the command `conda env cretae -f malware_ml.yml` then `conda activate malware_ml` to have all the dependencies ready to run these experiments. 

## Final Paper Location
https://github.com/KlausKingsman/ML-Final/tree/main/showcase-grades
