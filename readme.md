# Pulumi AKS Typescript

This repo contains a walkthrough for getting started with [Pulumi](https://www.pulumi.com) on Azure, creating a Kubernetes cluster (aka AKS) utilizing TypeScript.

Pulumi is a Infrastructure As Code Framework, that allows to build, deploy and manage modern cloud applications and infrastructure using familiar languages.  

## Prerequisites
* [Install Pulumi](https://www.pulumi.com/docs/get-started/install/)
* [Signup to Pulumi](https://app.pulumi.com/signup)
* Install [Node.js](https://nodejs.org/en/download/)
* Install [TypeScript](https://www.typescriptlang.org/download)
* Install [Azure CLI](https://docs.microsoft.com/de-de/cli/azure/install-azure-cli) and login using `az login`

## Deploy stack
* `pulumi login`
* `cd infra && pulumi up`

## Connect to k8s 
* `pulumi stack output kubeconfig --show-secrets > kubeconfig.yaml`
* `export KUBECONFIG=./kubeconfig.yaml`


## Destroy stack
* `pulumi destroy`