# Identify-and-remove-bias-from-AI-models-using-Watson-Studio

## Step 1: Create an IBM Cloud account

Login/Sign-up for IBM Cloud Account: 

## Step 2: Create Watson Studio service

Go to your IBM Cloud Dashboard, type in search box "Watson studio" select the service, on the service page click create

<img width="540" alt="1" src="https://user-images.githubusercontent.com/16270682/130227865-a245e3e9-e1b4-46d5-8048-f8809d846446.PNG">

<img width="910" alt="2" src="https://user-images.githubusercontent.com/16270682/130227908-5a72177b-2fda-4a8f-8d70-fd4f8761c36a.PNG">


## Step 3: Create a new Watson Studio project

Click on get started it will take you to a "Cloud Pak for Data" Dashboard. 

<img width="490" alt="3" src="https://user-images.githubusercontent.com/16270682/130227947-ead78d84-75e2-48ad-b489-18939abfdc46.PNG">

<img width="837" alt="4" src="https://user-images.githubusercontent.com/16270682/130227980-2aa2c5b4-65f7-4b39-b5a0-96fbd559536e.PNG">


Select create a project

<img width="580" alt="5" src="https://user-images.githubusercontent.com/16270682/130228261-90016159-e276-416c-af47-d3337baa4edb.PNG">

Click on create an empty project

<img width="916" alt="6" src="https://user-images.githubusercontent.com/16270682/130228274-2dcd1641-f504-43d6-aaee-ce62a942ab02.PNG">


Give your project a unique name and click on create 

<img width="930" alt="7" src="https://user-images.githubusercontent.com/16270682/130228284-6c2d3a6b-fe41-4d4a-abba-c2223443e233.PNG">

## Step 4: Add Data

Go to https://github.com/IBM/bias-mitigation-of-machine-learning-models-using-aif360 and download code in zip file. Un-zip the folder.

<img width="692" alt="8" src="https://user-images.githubusercontent.com/16270682/130228304-fea200fc-8508-4510-81fb-7a2a76eb90d4.PNG">


Click on Assets and select Browse and add fraud_data.csv file from your file system. Repeat the step and add the Pipeline_LabelEncoder-0.1.zip file as an asset.

<img width="918" alt="9" src="https://user-images.githubusercontent.com/16270682/130228315-b24224e9-a3c1-4710-9f35-6caf48bc9c3a.PNG">

## Step 5:  Create the notebook


### Note: You will create three Notebooks here by repeating the below steps. 

From IBM Watson Dashboard click on "Add to project" and select "Notebook"

<img width="750" alt="10" src="https://user-images.githubusercontent.com/16270682/130228834-fb48f7fb-14f5-4cc5-9da6-15d770e9d16e.PNG">

<img width="548" alt="11" src="https://user-images.githubusercontent.com/16270682/130228859-7f3ad65d-1e87-4ee3-beaf-562ebf60bbda.PNG">

Create a  Pre-processing Notebook. Select the "From URL" tab and Enter a name for the notebook. Select the runtime (2 vCPU and 8 GB RAM.)
Enter this Notebook URL for Pre-processing : https://github.com/IBM/bias-mitigation-of-machine-learning-models-using-aif360/blob/main/notebooks/Pre-processing.ipynb

<img width="953" alt="12" src="https://user-images.githubusercontent.com/16270682/130231839-5dff0600-943b-4231-9a12-c7f061a37ffd.PNG">


After the noteboob is imported, click on Not Trusted and select the option to trust the source of the notebook.

<img width="861" alt="13" src="https://user-images.githubusercontent.com/16270682/130231849-db8293d5-7543-4458-b62e-c85d428e23b2.PNG">


Repeat the above steps for in-processing and Post-processing 

Enter this Notebook URL for In-processing : https://github.com/IBM/bias-mitigation-of-machine-learning-models-using-aif360/blob/main/notebooks/In-processing.ipynb
Enter this Notebook URL for Post-processing : https://github.com/IBM/bias-mitigation-of-machine-learning-models-using-aif360/blob/main/notebooks/Post-processing.ipynb

## Step 6:


