# AWS-Infrastructure-Python-Automation
This repository contains links to my AWS infrastructure automation provisioning and python appplication deployment repositories. In this project I tried to separate my application , infrastructure code and lambda function code in separate respositories as per the best deployment practices and utilized the github actions to create and end to end deployment cycle for my application.
Below are the repository names and links to them -
1. Infrastructure - https://github.com/sagar-malhotra/infrastructure
( The infrastructure repositor contains the cloud function template the is being used to deploy all the AWS infrastructure elements needed for the python application deployment and security. Please visit the link for more information on the repository)

2. WebApp - https://github.com/sagar-malhotra/webapp
( The webapp repository cotains the python application code to be deployed along with the github action workflows. For more information on the webapp and deployment please visit the link attached above)

3. Serverless - https://github.com/sagar-malhotra/serverless
( The Serveless repository contains the lambda function code responsible for handling the user verfication process after sign up and the github action workflow responsible for deploying the lambda function. For more information please visit the repository from the link attached above)
