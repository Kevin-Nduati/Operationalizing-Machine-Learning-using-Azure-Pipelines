# General Overview
The aim of this project was to create a machine learning model on Microsoft Azure Ml then consume it through an endpoint. 
The dataset contains information about clients. 

# Architecture Design
<img src="https://github.com/Kevin-Nduati/Operationalizing-Machine-Learning-using-Azure-Pipelines/blob/master/images/00-Architecture.png">


# Authentification
After installing az and login has succeeded
<img src="https://github.com/Kevin-Nduati/Operationalizing-Machine-Learning-using-Azure-Pipelines/blob/e98e017a2ba9ebd01b17d243ac0b9c03559da465/images/01-Authentication.png">

# Automated ML Experiment
I then created an automl experiment using the Bank Market Dataset, to perform classification.
Here is a screenshot of the uploaded dataset.
<img src="https://github.com/Kevin-Nduati/Operationalizing-Machine-Learning-using-Azure-Pipelines/blob/master/images/02-Upload%20Dataset.png">

Here is  a screenshot of the completed experiment
<img src="https://github.com/Kevin-Nduati/Operationalizing-Machine-Learning-using-Azure-Pipelines/blob/e98e017a2ba9ebd01b17d243ac0b9c03559da465/images/03-Experiment%20Complete.png">

Here is a screenshot of the best model.
<img src="https://github.com/Kevin-Nduati/Operationalizing-Machine-Learning-using-Azure-Pipelines/blob/e98e017a2ba9ebd01b17d243ac0b9c03559da465/images/04-Model_summary.png">

# Deploy the Model
After selecting the best model from the Automated ML, it was deployed using the Azure Container Instance. Deploying the best model will allow it to interact with the HTTP API server and interact with the model by sending data over POST requests.

The model was deployed, application insights were enabled and the logs were also retrieved. The screenshots are as follows:
<img src="https://github.com/Kevin-Nduati/Operationalizing-Machine-Learning-using-Azure-Pipelines/blob/e98e017a2ba9ebd01b17d243ac0b9c03559da465/images/05-deployed_model.png">

Logs:
<img src="https://github.com/Kevin-Nduati/Operationalizing-Machine-Learning-using-Azure-Pipelines/blob/master/images/05-Logs.png">
