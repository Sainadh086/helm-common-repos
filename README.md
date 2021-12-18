# Helm chart for regular use

### Installation
    - helm repo add common-chart https://sainadh086.github.io/helm-common-repos/
    - helm install --name my-chart common-chart/webapp

## Why?

When you are trying to deploy a container in Kubernetes, you have to create multiple kubernetes manifests.
We always need to create a deployment, service, and ingress manifest. In some usecases we may not need to create a statefulset, pv, pvc manifests also.

So to reuse all the kubernetes manifests, we can create a helm chart. 

This chart helps you to deploy the container in Kubernetes without writing any extra kubernetes manifest files and you can reuse it in CD pipelines.

## Usecase

- This is a simple helm chart for deploying a container in Kubernetes and exposing with ingress.
- This chart is used in CD pipelines.


By default ngnix will be installed. Will be update with new version including many more usecases.
