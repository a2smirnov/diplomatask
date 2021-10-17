
[![Build Status](https://dev.azure.com/asmirnov51/Diploma%20Demo/_apis/build/status/a2smirnov.diplomatask?branchName=master)](https://dev.azure.com/asmirnov51/Diploma%20Demo/_build/latest?definitionId=10&branchName=master)
# DevOps course diploma task demo
# Deployment strategy to be defined...
Infrastructure (Azure MySQL, ACR, Azure k8s) should be deployed via terraform first
(a2smirnov/diplomatask/terraform)

# Pipline prerequisites:
Project service connection 'ascicdacr' to ACR should be actual

Project service connection 'as-cicd-k8s' to AKS via KubeConfig (terraform output -raw kube_config) should be actual

Pipeline variables should be set:

DB_HOST, DB_NAME (terrafrom output -raw credentials)

Pipeline Secrets DB_USERNAME and DB_PASSWORD should be set (terrafrom output -raw credentials)

SonarCloud service endpoint should be set and connected

## Aleksei Smirnov
