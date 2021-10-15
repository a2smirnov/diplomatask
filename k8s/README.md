# Azure k8s cluster manual control

## Simple kubectl connection:
run ./k8env to get credentials first
export KUBECONFIG=./azurek8s

## To delete namespace
k8stop prod|dev

## To get url to site:
echo "Use link http://"$(kubectl -n kube-system get svc addon-http-application-routing-nginx-ingress --output jsonpath='{.status.loadBalancer.ingress[0].ip}')" to access web application"
