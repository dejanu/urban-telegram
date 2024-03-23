# urban-telegram

## Create Kubernetes cluster in Azure, AWS or GCP, using Pulumi or Terraform:

* Set up a K8S cluster with the latest stable version, with RBAC enabled.
* The Cluster should have 2 services deployed – Service A and Service B:
* Service A is a WebServer written in C#, Go or Python that exposes the following:
* Current value of Bitcoin in USD (updated every 10 seconds taken from an API on the web, like https://min-api.cryptocompare.com/data/price?fsym=BTC&tsyms=USD).
* Average value over the last 10 minutes.
* Service B is a REST API service, that exposes a single controller that responds 200 status code on GET requests.
* Cluster should have NGINX Ingress controller deployed, and corresponding ingress rules for Service A and Service B.
* Service A should not be able to communicate with Service B.
 

## General Guidelines:

* The following cluster buildout should be secure, repeatable, and automated as much as possible.
 
