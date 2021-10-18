# Azure k8s cluster manual control

## Simple kubectl connection:
run ./k8env to get credentials first
export KUBECONFIG=./azurek8s

## To delete namespace
k8stop prod|dev
