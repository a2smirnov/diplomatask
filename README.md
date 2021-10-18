
[![Build Status](https://dev.azure.com/asmirnov51/Diploma%20Demo/_apis/build/status/a2smirnov.diplomatask?branchName=master)](https://dev.azure.com/asmirnov51/Diploma%20Demo/_build/latest?definitionId=10&branchName=master)
# DevOps course diploma task demo
# Deployment strategy to be defined...
Infrastructure (Azure MySQL, ACR, Azure k8s) deployed via terraform first
./infra-start

# Pipline prerequisites:
Project service connection 'ascicdacr' to ACR should be actual

Project service connection 'ascicdk8s' to AKS should be actual (with admin rights)

Project service connection 'SonarCloud' service should be actual

Pipeline variable group 'Diploma' variables should be set

Application variable group 'Application' variables should be set:
DB_HOST, DB_NAME (terrafrom output -raw credentials)
Secrets DB_USERNAME and DB_PASSWORD should be set (terrafrom output -raw credentials)


## Aleksei Smirnov
