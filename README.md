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


- Stage 2 We have  Prepared   an Base Model in research to test and preparing an basemodel called st_02.ipynb
    - Added paremeters in params.yaml
    - updated config.yaml 
    - BY adding code prepare base_model
- Code"
prepare_base_model:
   root_dir: artifacts/prepare_base_model
   base_model_path: artifacts/prepare_base_model/base_model.h5
   updated_base_model_path: artifacts/prepare_base_model/base_model_updated.h5

- Stage 3 Creating an callbacks 

- Stage 4 using callbacks 
          - creating training

          to see tensor board in locahost:
         command: tensorboard --logdir=artifacts/prepare_callbacks/tensorboard_log_dir/  </b>
- Stage 5 Training a Model
- Stage 6: Evaluating an Model

# UI and Prediction:
        - Updates app.py
        - Created templates/index.html Added UI components

# Deployment (AWS)

    - Building an Docker image of source code
    - Push your docker image to ECR
    - Launch your EC2
    - Pull Your Image from ECR in EC2 
    - Launch your docker image in EC2

    - Create an Docker file
    - Create an github/workflows  in main.yaml

# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console.

## 2. Create IAM user for deployment

	#with specific access

	1. EC2 access : It is virtual machine

	2. ECR: Elastic Container registry to save your docker image in aws


	#Description: About the deployment

	1. Build docker image of the source code

	2. Push your docker image to ECR

	3. Launch Your EC2 

	4. Pull Your image from ECR in EC2

	5. Lauch your docker image in EC2

	#Policy:

	1. AmazonEC2ContainerRegistryFullAccess

	2. AmazonEC2FullAccess

	
## 3. Create ECR repo to store/save docker image
    - Save the URI: 192228779581.dkr.ecr.us-east-1.amazonaws.com/catdog

	
## 4. Create EC2 machine (Ubuntu) 

## 5. Open EC2 and Install docker in EC2 Machine:
	
	
	#optional

	sudo apt-get update -y

	sudo apt-get upgrade
	
	#required

	curl -fsSL https://get.docker.com -o get-docker.sh

	sudo sh get-docker.sh

	sudo usermod -aG docker ubuntu

	newgrp docker
	
# 6. Configure EC2 as self-hosted runner:
    setting>actions>runner>new self hosted runner> choose os> then run command one by one


# 7. Setup github secrets:

    AWS_ACCESS_KEY_ID=

    AWS_SECRET_ACCESS_KEY=

    AWS_REGION = us-east-1

    AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

    ECR_REPOSITORY_NAME = simple-app








