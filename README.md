# cnnClassifier



# Problem Statement:
- classify whether images contain either a dog or a cat.  This is easy for humans, dogs, and cats. Your computer will find it a bit more difficult.


# Dataset Description
- training archive contains 25,000 images of dogs and cats. Train your algorithm on these files and predict the labels for test1.zip (1 = dog, 0 = cat).


- In short, if you cheat by hand labeling your predictions, expect to do it all over again, possibly many    times.  Thanks in advance for a fair competition and have fun.  



# End To End DL Project With Deployment

# Steps:


- 1 Data Ingestion 
- 2 Data Transformation
- 3 Model Trainer 
- 4 Model Evaluation 
- 5 Model Deployement




# CI/CD Pipelines- AWS DEPLOYEMENT with Github Actions




# step by step we have created directory structure 

- by createing workflow iof directory strure in template.py
- After that you have to run  python template.py

-  will create directory structure for project


# Diagram of folder Structure


# Create an Virtual Enviroment by using below command:

    - conda create -n cnncls python=3.8  -y
    - conda activate cnncls


    - then updated Requirements.txt 

    - install all libraries which updated in requirements.txt by using command


    -pip install -r  requirements.txt


# After that in src/utils
    - Updated and written code in constructuctor __init__.py
    - Created Common.py file




## Workflows 

    - 1 Update config.yaml
    - 2 Update secrets.yaml  [Optional]
    - 3 Updates params.yaml
    - 4 Update entity
    - 5 Update the configuration manager in src/config
    - 6 Update components
    - 7 Update pipeline
    - 8 Update main.py


- in this we are creating another py file called data_ingestion.py
- created another py file in entity called config_entity.py

- We have completed  Stage 1 Data Ingestion Part
        - Updated Data Ingestion in components
        - Update  config_entity.py


- Stage 2 We have  Prepared   an Base Model
    - Added paremeters in params.yaml
    - updated config.yaml 
    - BY adding code prepare base_model
- Code"
prepare_base_model:
   root_dir: artifacts/prepare_base_model
   base_model_path: artifacts/prepare_base_model/base_model.h5
   updated_base_model_path: artifacts/prepare_base_model/base_model_updated.h5







